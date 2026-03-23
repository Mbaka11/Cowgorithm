# Cowgorithm

**Smart livestock management for Canadian farms** — GPS-enabled smart collars with virtual fencing, health monitoring, and grazing optimization, built for Quebec's climate and agricultural reality.

---

## Vision

Canadian agriculture is ripe for a technology leap. Inspired by Halter (NZ, ~$2B valuation), Cowgorithm aims to bring GPS-enabled smart collars and virtual fencing to Quebec farms — starting with dairy and cattle, then expanding to other livestock, pets, and sport/performance markets. Built from day one for Canadian winters, bilingual (FR/EN), and designed around the unique structure of Quebec agriculture (supply management, cooperatives, UPA).

## Project Status

**Phase**: Pre-build — Market Study & Business Planning

We are currently conducting a Quebec-focused market study across four segments before writing any product code. This repo holds all planning documents and will later contain the product source code and hardware designs.

## Team

Small team (2–3 people) · Bootstrapping · Based in Quebec

---

## Repository Structure

```
cowgorithm/
├── README.md                              ← You are here
├── docs/
│   ├── market-study/                      ← Quebec market research
│   │   ├── 01-quebec-agriculture-overview
│   │   ├── 02-segment-cattle-dairy
│   │   ├── 03-segment-other-livestock
│   │   ├── 04-segment-pets
│   │   ├── 05-segment-sport-performance
│   │   ├── 06-competitive-landscape
│   │   └── 07-market-study-summary
│   ├── business-planning/                 ← Business model & strategy
│   │   ├── business-model-canvas
│   │   ├── value-propositions
│   │   ├── financial-projections
│   │   ├── regulatory-compliance
│   │   └── go-to-market-strategy
│   ├── technical/                         ← Technical pre-feasibility
│   │   ├── technical-feasibility
│   │   └── product-requirements
│   └── pitch/                             ← Pitch & grant materials
│       └── pitch-deck-outline
├── research/                              ← Bibliography & progress tracking
│   ├── sources.md
│   └── research-plan.md
├── src/                                   ← (future) product code
└── hardware/                              ← (future) schematics & BOM
```

---

## Document Index

### Market Study

| #   | Document                                                                           | Description                                                   | Status      |
| --- | ---------------------------------------------------------------------------------- | ------------------------------------------------------------- | ----------- |
| 01  | [Quebec Agriculture Overview](docs/market-study/01-quebec-agriculture-overview.md) | QC agriculture landscape, tech adoption, government programs  | Not started |
| 02  | [Cattle & Dairy Segment](docs/market-study/02-segment-cattle-dairy.md)             | TAM/SOM, competitors, willingness to pay, QC-specific factors | Not started |
| 03  | [Other Livestock Segment](docs/market-study/03-segment-other-livestock.md)         | Sheep, goats, poultry, hogs — applicability & market size     | Not started |
| 04  | [Pet Segment](docs/market-study/04-segment-pets.md)                                | Dogs & cats — GPS trackers, differentiation, consumer market  | Not started |
| 05  | [Sport & Performance Segment](docs/market-study/05-segment-sport-performance.md)   | Equestrian, athletes, working dogs — derivative potential     | Not started |
| 06  | [Competitive Landscape](docs/market-study/06-competitive-landscape.md)             | Competitor matrix, white-space analysis, IP landscape         | Not started |
| 07  | [Market Study Summary](docs/market-study/07-market-study-summary.md)               | Segment ranking, primary recommendation, derivative roadmap   | Not started |

### Business Planning

| Document                                                                   | Description                                           | Status      |
| -------------------------------------------------------------------------- | ----------------------------------------------------- | ----------- |
| [Business Model Canvas](docs/business-planning/business-model-canvas.md)   | Key partners, activities, revenue streams per segment | Not started |
| [Value Propositions](docs/business-planning/value-propositions.md)         | Customer personas, jobs/pains/gains per segment       | Not started |
| [Financial Projections](docs/business-planning/financial-projections.md)   | Unit economics, 3-year P&L, break-even, runway        | Not started |
| [Regulatory & Compliance](docs/business-planning/regulatory-compliance.md) | ISED, MAPAQ, PIPEDA, Law 25, municipal regulations    | Not started |
| [Go-to-Market Strategy](docs/business-planning/go-to-market-strategy.md)   | Launch region, channels, pilots, pricing, expansion   | Not started |

### Technical

| Document                                                         | Description                                               | Status      |
| ---------------------------------------------------------------- | --------------------------------------------------------- | ----------- |
| [Technical Feasibility](docs/technical/technical-feasibility.md) | Hardware, connectivity, software, cold-weather challenges | Not started |
| [Product Requirements](docs/technical/product-requirements.md)   | MVP features, user stories, hardware/software specs       | Not started |

### Pitch & Grants

| Document                                               | Description                          | Status      |
| ------------------------------------------------------ | ------------------------------------ | ----------- |
| [Pitch Deck Outline](docs/pitch/pitch-deck-outline.md) | 12-slide structure, QC grant targets | Not started |

### Research

| Document                                             | Description                                    |
| ---------------------------------------------------- | ---------------------------------------------- |
| [Sources & Bibliography](research/sources.md)        | All data sources with verification status      |
| [Research Plan & Tracker](research/research-plan.md) | Master progress tracker for all research tasks |

---

## Phased Approach

| Phase                        | Focus                                     | Depends On | Target    |
| ---------------------------- | ----------------------------------------- | ---------- | --------- |
| **1. Repo Setup**            | Folder structure, stubs, README           | —          | **Done**  |
| **2. Market Study**          | Quebec-focused research across 4 segments | Phase 1    | Weeks 1–2 |
| **3. Business Planning**     | BMC, financials, regulatory, GTM          | Phase 2    | Weeks 2–3 |
| **4. Technical Feasibility** | Hardware/software pre-feasibility, PRD    | Phase 2    | Weeks 2–3 |
| **5. Pitch Deck**            | Team alignment, grant readiness           | Phases 2–4 | Week 3–4  |

---

## Key Decisions

- **All four segments studied equally** — the market study will rank them objectively
- **Bootstrapping first** — financial projections model lean scenarios; grants (Innov'Action, IRAP) as accelerators
- **Quebec-first launch** — French-first for agriculture segments, bilingual product from day one
- **Dual-purpose repo** — planning docs now, product code later in `src/` and `hardware/`

---

## License

TBD
