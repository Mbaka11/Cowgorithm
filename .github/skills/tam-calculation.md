---
name: tam-calculation
description: >
  Skill for calculating Total Addressable Market (TAM), Serviceable Addressable Market (SAM),
  and Serviceable Obtainable Market (SOM) for Cowgorithm's segments. Provides formulas,
  Quebec-specific multipliers, and validation approaches.
applyTo: "docs/market-study/**"
---

# TAM / SAM / SOM Calculation Skill

## Purpose

Provides standardized methodology for calculating market sizes across Cowgorithm's four segments, with Quebec-specific considerations.

## Definitions

- **TAM (Total Addressable Market)**: Total revenue opportunity if 100% of the target market adopted the product
- **SAM (Serviceable Addressable Market)**: Portion of TAM that is realistically reachable given product capabilities, geography, and go-to-market strategy
- **SOM (Serviceable Obtainable Market)**: Realistic revenue capture in the first 3 years given competition, resources, and adoption rates

## Formulas

### Livestock Segments (Cattle, Dairy, Sheep, Goats)

```
TAM = (Total head count in QC) × (Annual subscription per head) + (One-time hardware per head)
SAM = TAM × (% of farms with adequate connectivity) × (% of farms above minimum herd size threshold)
SOM = SAM × (Estimated market penetration in Year 1-3) × (Conversion rate from pilot to paid)
```

**Quebec-specific multipliers:**

- Connectivity factor: ~70-80% of QC farmland has adequate LTE-M coverage (verify with CRTC data)
- Minimum herd size: farms with <30 head may not see ROI → filter out
- Adoption rate: tech adoption in QC agriculture is ~15-25% for precision ag tools (verify)
- Dairy: higher willingness to adopt (quota farms are well-capitalized)

### Pet Segment

```
TAM = (Pet population in QC) × (% of owners who buy pet tech) × (Annual subscription + hardware)
SAM = TAM × (% in target demographic: urban/suburban, income bracket)
SOM = SAM × (Estimated Year 1-3 penetration)
```

**Quebec-specific multipliers:**

- Pet GPS tracker penetration in Canada: ~5-8% of dog owners (growing)
- QC pet spending: slightly below Canadian average but growing
- Urban concentration: Montreal, Quebec City, Gatineau = majority of pet owners

### Human Sport Performance Segment

```
TAM = (Registered athletes in QC) × (Device price + annual subscription) OR (Number of teams) × (Team subscription)
SAM = TAM × (% of teams/athletes willing to invest in performance tech)
SOM = SAM × (Year 1-3 penetration)
```

**Quebec-specific data points:**

- Soccer Quebec: ~200,000+ registered players
- Hockey Quebec: ~100,000+ registered players
- Team-based pricing may be more relevant than individual

## Validation Approaches

1. **Top-down**: Start from total market size and narrow down
2. **Bottom-up**: Start from unit pricing × realistic customer count
3. **Comparable**: Use Halter's NZ penetration rate as a proxy for what's achievable
4. Cross-check: top-down and bottom-up should be within 2x of each other

## Presentation Format

Always present TAM calculations as a table:

```markdown
| Metric                       | Value            | Assumption                  | Source  |
| ---------------------------- | ---------------- | --------------------------- | ------- |
| Total dairy cows in QC       | 350,000          | StatCan 2021                | [link]  |
| Annual subscription per cow  | $360 ($30/mo)    | Halter pricing as reference | —       |
| Hardware per cow (amortized) | $100/yr          | Estimated BOM               | —       |
| **TAM**                      | **$161M/yr**     | 350K × $460                 | —       |
| Connectivity filter          | 75%              | CRTC rural coverage         | [link]  |
| Minimum herd size filter     | 80%              | Farms >30 head              | StatCan |
| **SAM**                      | **$96.6M/yr**    | TAM × 0.75 × 0.80           | —       |
| Year 1-3 penetration         | 2-5%             | Conservative new entrant    | —       |
| **SOM**                      | **$1.9–4.8M/yr** | SAM × 0.02–0.05             | —       |
```
