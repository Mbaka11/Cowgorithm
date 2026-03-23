---
name: competitor-analysis
description: >
  Skill for conducting competitor analysis in the ag-tech, pet-tech, and sport-tech spaces.
  Use when researching companies like Halter, Nofence, Catapult, Fi, Tractive, or evaluating
  new competitors. Provides frameworks for feature comparison, pricing analysis, and
  differentiation strategy.
applyTo: "docs/market-study/**"
---

# Competitor Analysis Skill

## Purpose

Provides structured frameworks for analyzing competitors across Cowgorithm's four market segments: livestock, pets, and human sport performance.

## Analysis Framework

### Per-Competitor Profile

For each competitor, gather:

1. **Company basics**: Founded, HQ, funding, valuation, employee count
2. **Product**: What hardware + software they offer
3. **Pricing**: Hardware cost, subscription model, enterprise vs. consumer
4. **Target market**: Which segments, geographies, farm/team sizes
5. **Technology**: GPS, cellular, sensors, ML capabilities, indoor/outdoor
6. **Strengths**: What they do well, market position, brand
7. **Weaknesses**: Gaps, limitations, geographic restrictions
8. **Canada presence**: Available in Canada? French-language support? Cold-weather tested?

### Comparison Matrix

Use this format for side-by-side comparison:

```markdown
| Feature              | Cowgorithm (Planned) | Competitor A | Competitor B |
| -------------------- | -------------------- | ------------ | ------------ |
| Virtual fencing      | Yes                  | Yes          | No           |
| GPS tracking         | Yes                  | Yes          | Yes          |
| Health monitoring    | Planned              | Yes          | Basic        |
| Cold-weather rated   | -40°C target         | Unknown      | N/A          |
| French language      | Yes                  | No           | No           |
| Canadian presence    | QC-first             | No           | Limited      |
| Price per unit/month | TBD                  | $30/mo       | $8/mo        |
```

### Differentiation Strategy

For each segment, identify:

- **Must-have features**: Table stakes that every competitor offers (can't skip these)
- **Differentiators**: Features that set Cowgorithm apart (cold-weather, bilingual, multi-species)
- **Won't-compete**: Areas where established players are too dominant (e.g., individual endurance wearables)

## Key Competitors by Segment

### Livestock

- **Halter** (NZ) — see `research/case-studies/halter.md` for detailed analysis
- **Nofence** (Norway) — first virtual fencing for sheep/goats
- **Vence** (US/Merck) — enterprise cattle virtual fencing
- **DeLaval** (Sweden) — dairy herd management (not virtual fencing)
- **Lely** (Netherlands) — dairy automation

### Pets

- **Fi** (US) — GPS smart collar for dogs
- **Tractive** (Austria) — GPS tracker for dogs/cats, affordable
- **Whistle** (US/Mars) — GPS + health monitoring

### Human Sport Performance

- **Catapult / STATSports** (Australia) — dominant in team sport analytics
- **Kinexon** (Germany) — UWB-based indoor + outdoor tracking
- **Polar** (Finland) — HR + GPS team monitoring
- **Garmin** (US) — individual athlete GPS watches
- **Whoop** (US) — subscription wearable, recovery focus

## IP / Patent Considerations

When researching competitors, also check:

- Google Patents for key filings (virtual fencing, animal collar, GPS tracking)
- WIPO for international patent applications
- Focus on: method patents (how virtual fencing works), hardware patents (collar design), software patents (ML algorithms)
- Goal: ensure freedom-to-operate for Cowgorithm's design
