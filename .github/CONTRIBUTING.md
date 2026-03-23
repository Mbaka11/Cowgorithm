# Contributing to Cowgorithm

## Getting Started

1. Clone the repo
2. Copy `.env.example` to `.env` and fill in values (when applicable)
3. Read the [README](../README.md) for project overview and phase status

## Branch Strategy

- `main` — stable, reviewed content
- `research/<topic>` — market study research branches
- `feature/<name>` — product features (future)
- `docs/<name>` — documentation improvements

## Document Standards

### Market Study Documents
- Every factual claim must cite a source from [sources.md](../research/sources.md)
- Use Quebec-specific data when available (not just Canadian averages)
- TAM/SAM/SOM calculations must show their math and assumptions
- Mark document status in the research plan when updating

### Commit Messages
```
type(scope): short description

docs(market-study): add QC dairy farm count from StatCan 2021
research(halter): add patent analysis section
chore(repo): update .gitignore for hardware tools
```

Types: `docs`, `research`, `chore`, `feat`, `fix`

## Review Process

- Market study sections: reviewed by at least one team member before merging
- Financial projections: reviewed by all team members
- All data claims must be traceable to a listed source

## Language

- Technical docs and code: English
- Product-facing content: French-first for QC agriculture segments
