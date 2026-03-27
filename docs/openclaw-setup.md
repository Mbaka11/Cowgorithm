# OpenClaw Setup Guide — Cowgorithm Autonomous Research Agent

This guide walks you through installing and configuring [OpenClaw](https://github.com/openclaw/openclaw) as an autonomous research agent for the Cowgorithm project. OpenClaw runs sandboxed against this repo, communicates via WhatsApp, and works through tasks on-demand — either via WhatsApp commands or CLI prompts.

---

## Prerequisites

- **Node.js 24+** — [Download](https://nodejs.org/)
- **Docker Desktop** — Required for sandbox mode. [Download](https://www.docker.com/products/docker-desktop/)
- **GitHub Copilot subscription** — Individual or Business plan
- **WhatsApp** on your phone

---

## 1. Install OpenClaw

```bash
npm install -g openclaw@latest
openclaw --version  # Confirm installation
```

## 2. Run Onboarding

```bash
openclaw onboard
```

This creates `~/.openclaw/` and the initial `openclaw.json` config.

## 3. Configure the Agent

Copy the template from this repo into your OpenClaw config:

```bash
# Windows (PowerShell)
Copy-Item .\openclaw.config.jsonc $env:USERPROFILE\.openclaw\openclaw.json

# macOS/Linux
cp openclaw.config.jsonc ~/.openclaw/openclaw.json
```

Then edit `~/.openclaw/openclaw.json` — search for **`CHANGE_ME`** (3 placeholders):

1. **`CHANGE_ME #1`** — `agent.workspace`: your local project path
2. **`CHANGE_ME #2`** — `docker.mounts`: same path (must match #1)
3. **`CHANGE_ME #3`** — `whatsapp.allowFrom`: your phone number in international format (e.g. `+15141234567`)
4. **Remove JSONC comments** — OpenClaw expects valid JSON. Strip all `//` comment lines.

> **Tip**: Use `openclaw doctor` to validate your config after editing.

## 4. Authenticate with GitHub Copilot

```bash
openclaw models auth login-github-copilot
```

This uses GitHub's device OAuth flow:
1. It will show a URL and a device code.
2. Open the URL in your browser, enter the code, and authorize.
3. OpenClaw exchanges your GitHub token for a Copilot API token automatically.

Verify the model works:

```bash
openclaw models test github-copilot/claude-sonnet-4.6
```

> **Model config**: The agent uses `claude-sonnet-4.6` (primary premium model) with automatic fallback to `gpt-4o` (free/unlimited) when the daily premium request limit is hit. Limits are configured in the config file under `limits`.

## 5. Set Up WhatsApp

```bash
openclaw channels setup whatsapp
```

1. A QR code will appear in the terminal.
2. Open WhatsApp on your phone → Settings → Linked Devices → Link a Device.
3. Scan the QR code.
4. Send a test message: "ping" — agent should reply.

> **Security**: The `dmPolicy: "pairing"` config means unknown numbers must enter a pairing code before the agent responds.

## 6. Verify Sandbox

```bash
openclaw doctor
```

Confirm these pass:
- ✅ Docker is running
- ✅ Sandbox mode: `always`
- ✅ Workspace mounted at `/workspace`
- ✅ Model authenticated

Test that the sandbox can't escape:

```bash
openclaw run --sandbox "ls /home"
# Should only see /workspace contents, not your host filesystem
```

## 7. Start the Agent

```bash
# Foreground (for initial testing)
openclaw start

# Background daemon (for production use)
openclaw start --daemon
```

The agent will:
- Read `AGENTS.md` and `SOUL.md` for project context and personality
- Load skills from `skills/`
- Listen for WhatsApp messages

## 8. First Test

Send via WhatsApp:

> "What's the current status of the Cowgorithm project? Read research/research-plan.md and summarize."

The agent should reply with a brief summary showing Phase 2 complete, Phases 3–5 not started.

---

## How to Give Tasks

The agent works **on-demand** — no cron schedules. You control when it works.

### Via WhatsApp

Send natural language commands:

```
"Work through the next incomplete task in research-plan.md"
"Complete all Phase 3 business planning tasks"
"Explore wildlife management as an adjacent market"
"Write the financial projections document"
"Scan for Halter/Nofence competitor news from the past month"
```

The agent reads `AGENTS.md` for context, checks `research/research-plan.md` for the backlog, and works until the task is done (or hits a question it needs your input on).

### Via CLI

```bash
# One-shot task
openclaw run "Complete the business-model-canvas.md document"

# Work through all remaining Phase 3 tasks
openclaw run "Read research/research-plan.md. Complete every 'Not started' task in Phase 3, one by one. Update the plan after each. Stop and message me if you need a decision."
```

### Completion behavior

The agent doesn't stop on a timer — it works until:
- The specific task is done
- It hits a question that needs your input (sends WhatsApp, waits)
- It hits the daily premium request limit (falls back to free model, continues)
- All tasks in the requested scope are marked "Done" in research-plan.md

---

## File Structure Added by This Setup

```
cowgorithm/
├── AGENTS.md                    ← Agent instructions (project context, rules)
├── SOUL.md                      ← Agent personality definition
├── openclaw.config.jsonc        ← Config template (copy to ~/.openclaw/)
├── docs/openclaw-setup.md       ← This file
├── skills/
│   ├── research/SKILL.md        ← Research methodology
│   └── report-gen/SKILL.md      ← Output formats & templates
├── research/explorations/       ← Agent writes adjacent market discoveries here
├── docs/summaries/              ← Agent writes WhatsApp-style briefs here
└── docs/reports/                ← Agent writes full reports here
```

---

## Troubleshooting

| Problem | Fix |
|---------|-----|
| `openclaw: command not found` | Ensure Node.js 24+ is installed, run `npm install -g openclaw@latest` |
| Docker sandbox fails | Start Docker Desktop, run `docker ps` to verify |
| WhatsApp QR expired | Run `openclaw channels setup whatsapp` again |
| Model auth fails | Run `openclaw models auth login-github-copilot` again, check Copilot subscription is active |
| Agent ignores AGENTS.md | Ensure `agent.workspace` in config points to the correct project path |
| Agent stops mid-task | Check premium request limits with `openclaw limits status`. Increase `maxPremiumRequestsPerSession` in config or let it fall back to gpt-4o |

---

## Security Notes

- **Sandbox**: Agent runs in Docker. It can only see `/workspace` (this project). No access to host filesystem, network credentials, or other projects.
- **WhatsApp**: Only numbers in `allowFrom` can interact. Unknown senders need a pairing code.
- **No secrets in repo**: The `openclaw.json` config with your phone number lives in `~/.openclaw/`, not in this repo. The `.gitignore` excludes OpenClaw credential files.
- **Tool restrictions**: `canvas`, `nodes`, `cron_delete`, and `gateway` tools are denied in the sandbox config.
