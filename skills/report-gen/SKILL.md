# Report Generation Skill — Summaries, PDFs, and Briefs

## Purpose

Generate polished output documents from the research and analysis in this repo.
Supports multiple output formats for different audiences:

- **WhatsApp briefs** — Short summaries for quick founder updates
- **Executive summaries** — 1-2 page overviews for stakeholders
- **Full reports** — Comprehensive documents with data, charts, and recommendations
- **PDF export** — Convert markdown to PDF via pandoc (in sandbox)

## WhatsApp Brief Format

For sending research updates via WhatsApp, use this template:

```
📊 *{Topic}* — {Date}

*Key findings:*
• {Finding 1 — one sentence with a number}
• {Finding 2}
• {Finding 3}

*What changed:*
{1-2 sentences on what's new since last update}

*Action needed:*
{Question or decision for the founder, if any}

📄 Full report: {filename in repo}
```

Rules:
- Max 250 words per message
- Use WhatsApp-compatible formatting (*bold*, _italic_, ```code```)
- One topic per message — don't bundle unrelated updates
- Ask ONE question at a time

## Executive Summary Format

Write to `docs/summaries/{topic-slug}-summary.md`:

```markdown
# {Topic} — Executive Summary
> Generated: {date} | Source docs: {list of source filenames}

## Bottom Line
{2-3 sentences: the main takeaway and recommended action}

## Key Numbers
| Metric | Value | Source |
|--------|-------|--------|
| ...    | ...   | ...    |

## Opportunities
1. {Opportunity with brief rationale}
2. ...

## Risks
1. {Risk with mitigation}
2. ...

## Recommended Next Steps
1. {Concrete action}
2. ...
```

## Full Report Compilation

For comprehensive reports, compile from existing docs:

1. Read all source documents from `docs/market-study/` and `docs/business-planning/`
2. Extract key data points and findings
3. Synthesize across segments — don't just concatenate
4. Add cross-cutting analysis (e.g., which segments share technology)
5. Write to `docs/reports/{report-name}.md`

## PDF Generation

When the user requests a PDF:

```bash
# In the sandbox, use pandoc if available
pandoc docs/reports/{report}.md \
  -o docs/reports/{report}.pdf \
  --pdf-engine=weasyprint \
  -V geometry:margin=1in \
  -V fontsize=11pt \
  --toc
```

If pandoc is not available, note this in the WhatsApp message and provide the
markdown file path instead.

## Progress Report (Scheduled)

For cron-triggered progress reports, compile:

1. What was completed since the last report
2. What's in progress
3. What's blocked or needs input
4. Any interesting discoveries from exploration scans
5. Updated completion percentage for each phase

Write to `docs/reports/progress-{date}.md` and send a WhatsApp brief.
