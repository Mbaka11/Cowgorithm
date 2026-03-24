# Research Plan & Progress Tracker

> Master tracker for all research activities across the Cowgorithm pre-build phase.
> Updated as work progresses. Each task links to the document it feeds into.

---

## Phase 1: Repo Structure Setup

| #   | Task                                 | Document  | Status   | Notes                     |
| --- | ------------------------------------ | --------- | -------- | ------------------------- |
| 1.1 | Create folder structure & stub files | All       | **Done** | 17 files created          |
| 1.2 | Write README with vision & TOC       | README.md | **Done** | Full TOC + document index |

---

## Phase 2: Market Study

### 2A. Quebec Agriculture Overview

| #    | Task                                                | Document                          | Status   | Notes                                                           |
| ---- | --------------------------------------------------- | --------------------------------- | -------- | --------------------------------------------------------------- |
| 2A.1 | QC agriculture GDP, employment, farm count          | 01-quebec-agriculture-overview.md | **Done** | Census 2021: 29,380 farms, 42,265 operators                     |
| 2A.2 | Key stats: dairy, cattle, hog, poultry, sheep farms | 01                                | **Done** | Full farm type breakdown with revenue shares                    |
| 2A.3 | Technology adoption trends in QC farming            | 01                                | **Done** | 49.8% tech use, 902 robotic milking farms                       |
| 2A.4 | Rural cellular/internet coverage analysis           | 01                                | **Done** | LTE-M coverage mapped for dairy belt                            |
| 2A.5 | Government ag-tech programs inventory               | 01                                | **Done** | Fed + QC programs inventoried (IRAP, SCAP, Innov'Action, SR&ED) |
| 2A.6 | Farmer pain points (labor, costs, sustainability)   | 01                                | **Done** | Aging workforce, succession crisis, off-farm work data          |

### 2B. Cattle & Dairy Segment

| #    | Task                                          | Document                   | Status   | Notes                                          |
| ---- | --------------------------------------------- | -------------------------- | -------- | ---------------------------------------------- |
| 2B.1 | QC dairy cow count & avg herd size            | 02-segment-cattle-dairy.md | **Done** | ~500K dairy cows, ~3,400-4,400 farms           |
| 2B.2 | TAM / SAM / SOM calculation                   | 02                         | **Done** | TAM ~$252M/yr, SOM ~$4.7M/yr Y3                |
| 2B.3 | Competitor deep dive (Halter, Nofence, Vence) | 02                         | **Done** | No competitors active in Canada                |
| 2B.4 | Willingness to pay research                   | 02                         | **Done** | $29/cow/month recommended                      |
| 2B.5 | Quebec-specific factors (quota, UPA, coops)   | 02                         | **Done** | Supply management, coop channels, French-first |
| 2B.6 | Barriers to entry analysis                    | 02                         | **Done** | Cold weather, farmer trust, ISED certification |

### 2C. Other Livestock Segment

| #    | Task                                        | Document                      | Status   | Notes                                           |
| ---- | ------------------------------------------- | ----------------------------- | -------- | ----------------------------------------------- |
| 2C.1 | Sheep, goat, poultry, hog farm counts in QC | 03-segment-other-livestock.md | **Done** | ~617 sheep/goat, ~1,263 hog, ~911 poultry farms |
| 2C.2 | Virtual fencing applicability per species   | 03                            | **Done** | Sheep/goat = high; hog/poultry = excluded       |
| 2C.3 | Existing solutions research                 | 03                            | **Done** | Nofence, Digitanimal, Gallagher                 |
| 2C.4 | TAM / SOM estimates per sub-segment         | 03                            | **Done** | Sheep/goat TAM ~$69M; SOM ~$420K Y3             |

### 2D. Pet Segment

| #    | Task                                 | Document           | Status   | Notes                                                     |
| ---- | ------------------------------------ | ------------------ | -------- | --------------------------------------------------------- |
| 2D.1 | QC pet population data               | 04-segment-pets.md | **Done** | CAHI 2022: 7.9M dogs, 8.5M cats nationally; QC ~22% share |
| 2D.2 | Existing GPS tracker comparison      | 04                 | **Done** | Fi, Whistle, Tractive, AirTag, Garmin compared            |
| 2D.3 | Differentiation opportunity analysis | 04                 | **Done** | Active virtual fencing for dogs = key differentiator      |
| 2D.4 | Consumer willingness to pay          | 04                 | **Done** | $270–350 Year 1; invisible fence replacement angle        |
| 2D.5 | Regulatory (ISED, pet safety)        | 04                 | **Done** | Animal welfare risk flagged (vibration collar perception) |
| 2D.6 | TAM / SOM calculation                | 04                 | **Done** | TAM ~$43M; SOM ~$527K Y3; score 2.85/5.00                 |

### 2E. Sport & Human Performance Segment

| #    | Task                                              | Document                        | Status   | Notes                                                          |
| ---- | ------------------------------------------------- | ------------------------------- | -------- | -------------------------------------------------------------- |
| 2E.1 | Soccer: QC participation, clubs, player counts    | 05-segment-sport-performance.md | **Done** | ~200K+ registered players, 800+ clubs                          |
| 2E.2 | Hockey: QC participation, teams, player counts    | 05                              | **Done** | ~100K+ registered players, LHJMQ 18 teams                      |
| 2E.3 | Team sport wearable competitive analysis          | 05                              | **Done** | Catapult, Kinexon, Polar, Zebra (pro), Garmin/Whoop (consumer) |
| 2E.4 | Technology crossover analysis (ag collar → sport) | 05                              | **Done** | ~50% backend transfers; UWB + HR sensor new                    |
| 2E.5 | Indoor tracking feasibility (hockey arenas)       | 05                              | **Done** | UWB required, $100–200K R&D; defers hockey segment             |
| 2E.6 | Equestrian market in QC                           | 05                              | **Done** | ~50–70K horses; niche TAM ~$2–5M                               |
| 2E.7 | Working dog niche research                        | 05                              | **Done** | Sled dogs, SAR, K-9; very niche ~$0.5–1M TAM                   |
| 2E.8 | TAM / SOM estimates (per sub-segment)             | 05                              | **Done** | Total sport TAM ~$1.6M; SOM ~$86K Y3; score 2.60/5.00          |

### 2F. Competitive Landscape

| #    | Task                       | Document                    | Status   | Notes                                                   |
| ---- | -------------------------- | --------------------------- | -------- | ------------------------------------------------------- |
| 2F.1 | Complete competitor matrix | 06-competitive-landscape.md | **Done** | 13 companies across all 4 segments                      |
| 2F.2 | White-space analysis       | 06                          | **Done** | 7 major gaps identified; zero virtual fencing in Canada |
| 2F.3 | IP / patent landscape scan | 06                          | **Done** | Halter/Nofence/Vence patents flagged; FTO search needed |

### 2G. Market Study Summary

| #    | Task                           | Document                   | Status   | Notes                                                        |
| ---- | ------------------------------ | -------------------------- | -------- | ------------------------------------------------------------ |
| 2G.1 | Segment scoring & ranking      | 07-market-study-summary.md | **Done** | Cattle 4.55, Livestock 3.55, Pets 3.05, Sport 2.70           |
| 2G.2 | Primary segment recommendation | 07                         | **Done** | Cattle & dairy = primary; zero competitors in Canada         |
| 2G.3 | Derivative roadmap             | 07                         | **Done** | Phase 1→Cattle, 2→Sheep, 3→Pets, 4→Sport with tech map       |
| 2G.4 | Risk assessment                | 07                         | **Done** | 8 risks with mitigations; go/no-go framework with 7 criteria |

---

## Phase 3: Business Planning

| #   | Task                                   | Document                 | Status      | Notes                    |
| --- | -------------------------------------- | ------------------------ | ----------- | ------------------------ |
| 3.1 | Business Model Canvas (top 2 segments) | business-model-canvas.md | Not started | Depends on Phase 2       |
| 3.2 | Value Proposition Canvas per persona   | value-propositions.md    | Not started |                          |
| 3.3 | Unit economics calculation             | financial-projections.md | Not started |                          |
| 3.4 | 3-year P&L projections                 | financial-projections.md | Not started |                          |
| 3.5 | Bootstrapping runway analysis          | financial-projections.md | Not started |                          |
| 3.6 | Regulatory compliance roadmap          | regulatory-compliance.md | Not started | Can start during Phase 2 |
| 3.7 | Go-to-market strategy                  | go-to-market-strategy.md | Not started |                          |

---

## Phase 4: Technical Pre-Feasibility

| #   | Task                             | Document                 | Status      | Notes                      |
| --- | -------------------------------- | ------------------------ | ----------- | -------------------------- |
| 4.1 | Hardware architecture research   | technical-feasibility.md | Not started | Can start parallel Phase 3 |
| 4.2 | Connectivity coverage analysis   | technical-feasibility.md | Not started |                            |
| 4.3 | Cold-weather feasibility         | technical-feasibility.md | Not started |                            |
| 4.4 | Build vs buy vs partner analysis | technical-feasibility.md | Not started |                            |
| 4.5 | MVP feature set & PRD            | product-requirements.md  | Not started | Depends on Phase 2 + 4.1   |

---

## Phase 5: Pitch Deck

| #   | Task                               | Document              | Status      | Notes                 |
| --- | ---------------------------------- | --------------------- | ----------- | --------------------- |
| 5.1 | Draft pitch deck outline content   | pitch-deck-outline.md | Not started | Depends on Phases 2–4 |
| 5.2 | Grant program eligibility research | pitch-deck-outline.md | Not started |                       |

---

## Case Studies

| #    | Task                              | Document                | Status      | Notes                              |
| ---- | --------------------------------- | ----------------------- | ----------- | ---------------------------------- |
| CS.1 | Halter case study (initial draft) | case-studies/halter.md  | **Done**    | Business model, tech, NZ vs QC     |
| CS.2 | Verify Halter funding data        | case-studies/halter.md  | Not started | Source: Crunchbase, NZ media       |
| CS.3 | Halter patent research            | case-studies/halter.md  | Not started | Google Patents, WIPO               |
| CS.4 | Nofence case study (if needed)    | case-studies/nofence.md | Not started | Sheep/goat virtual fencing pioneer |

---

## Parallel Activities (Ongoing)

| #   | Task                                            | Status      | Notes                      |
| --- | ----------------------------------------------- | ----------- | -------------------------- |
| P.1 | Farmer interviews (5–10 informal conversations) | Not started | Run during Phase 2         |
| P.2 | Source verification & bibliography              | Not started | Ongoing, update sources.md |

---

> **Last updated**: 2026-03-23
