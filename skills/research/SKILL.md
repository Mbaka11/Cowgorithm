# Research Skill — Cowgorithm Market & Opportunity Research

## Purpose

Conduct structured market research for the Cowgorithm project. This skill covers:
- Market sizing (TAM/SAM/SOM) with explicit assumptions
- Competitor analysis with current pricing and feature data
- Regulatory and compliance scanning for Canadian markets
- Adjacent market exploration and opportunity discovery
- Source collection and verification

## Methodology

### Market Sizing

Use bottom-up calculations with verifiable inputs:

```
TAM = Total addressable units × Annual revenue per unit
SAM = TAM × Serviceable % (geographic + product fit filters)
SOM = SAM × Realistic capture rate (Year 1-3, benchmarked to comparables)
```

Always show:
- The source for each input number
- The assumptions behind each filter
- Conservative / Base / Optimistic scenarios

### Competitor Analysis

For each competitor, capture:
| Field            | Description                                    |
|------------------|------------------------------------------------|
| Company          | Name, HQ, founding year                        |
| Product          | What they sell (hardware, SaaS, both)          |
| Geography        | Where they operate; Canada presence (yes/no)   |
| Pricing          | Monthly/annual, per-unit or flat               |
| Technology       | GPS, LoRa, cellular, UWB, etc.                 |
| Funding          | Total raised, last round, investors            |
| Strengths        | What they do well                              |
| Weaknesses       | Gaps we could exploit                          |
| Canada threat    | Likelihood of entering Canadian market (1-5)   |

### Opportunity Scoring

Use the 5-factor framework established in the market study:

| Factor                    | Weight | Scale |
|---------------------------|--------|-------|
| Market size (TAM in CAD)  | 25%    | 1-5   |
| Competitive gap           | 25%    | 1-5   |
| Technology transfer       | 20%    | 1-5   |
| Regulatory fit            | 15%    | 1-5   |
| Strategic alignment       | 15%    | 1-5   |

Score = Weighted average. Threshold: ≥3.5 = pursue, 2.5-3.5 = monitor, <2.5 = deprioritize.

### Source Requirements

Every research output must:
1. Cite sources inline using `[Source Name, Year](URL)` format
2. Add each new source to `research/sources.md`
3. Mark verification status: **Verified** / **Unverified** / **Estimated**
4. Prefer Canadian government databases (StatCan, MAPAQ, ISED, CFIA)
5. Cross-reference at least 2 sources for any key statistic

### Adjacent Market Exploration

When scanning for new opportunities:
1. Start from hardware capabilities (GPS + accelerometer + cellular modem)
2. List all categories where location + motion tracking adds value
3. Filter by Canadian market size ≥ $5M TAM
4. Filter by competitive gap (no dominant Canadian player)
5. Score using the 5-factor framework
6. Write up promising finds in `research/explorations/{topic-slug}.md`

## Output Conventions

- Write research outputs as Markdown files in the appropriate `docs/` subfolder
- Use tables for structured data, not paragraphs
- Include a "Key Findings" summary at the top of each document
- Include a "Recommended Actions" section at the bottom
- All dollar figures in CAD unless explicitly noted otherwise
