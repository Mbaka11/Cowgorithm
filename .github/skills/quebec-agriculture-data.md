---
name: quebec-agriculture-data
description: >
  Skill for finding and interpreting Quebec agriculture data. Use when you need Quebec-specific
  farming statistics, dairy industry data, livestock counts, or agricultural economic indicators.
  Knows which government sources to check and how to interpret supply management and quota systems.
applyTo: "docs/market-study/**"
---

# Quebec Agriculture Data Skill

## Purpose

Provides guidance for finding and interpreting Quebec-specific agricultural data, particularly around the supply management system, dairy industry metrics, and livestock statistics.

## Key Data Sources

### Primary Statistics

- **Statistique Canada — Census of Agriculture**: Conducted every 5 years (2016, 2021). Table 32-10-0\* series.
  - Farm count by type and province: Table 32-10-0403-01
  - Livestock count by province: Table 32-10-0130-01
  - Farm operating revenue: Table 32-10-0136-01
- **MAPAQ Profil sectoriel**: Annual sector profiles for dairy, beef, pork, poultry, sheep
  - URL pattern: `quebec.ca/agriculture.../profils-sectoriels`
- **PLQ (Producteurs de lait du Québec)**: Dairy-specific stats
  - Number of dairy farms, average herd size, total production
  - Quota values and transfer data
- **UPA**: Aggregate farming statistics, member surveys, policy positions

### Quebec Dairy Industry Key Facts

- Quebec produces ~36% of Canada's milk (largest provincial share)
- ~9,500 dairy farms in QC (number declining, herd size increasing)
- Average herd size: ~75-85 cows (growing)
- Supply management: dairy production controlled by quota system
- Quota value: ~$24,000-$30,000 per kg of butterfat/day (very expensive → farmers are well-capitalized)
- Cooperative structure: most farmers are members of coops (Agropur, Sollio)

### Quebec Livestock Key Facts

- Beef cattle: ~150,000-200,000 head across ~7,000-8,000 farms
- Hogs: ~4.2M head, ~2,900 farms (concentrated, large operations)
- Sheep: ~285,000 head, ~1,100 farms (growing niche)
- Poultry (broilers + layers): supply-managed, large operations

## Interpreting Supply Management

The supply management system (dairy, poultry, eggs) is critical context:

- **Production quotas** limit output but guarantee prices → farmers have stable, predictable income
- **Quota is extremely valuable** → dairy farmers are typically asset-rich and can invest in technology
- **Entry barrier**: new entrants need to buy or lease quota (very expensive)
- **Implication for Cowgorithm**: QC dairy farmers have the financial capacity to subscribe to a per-cow service; they are used to data-driven management

## Data Quality Notes

- Census of Agriculture data is most reliable but only every 5 years (2021 is latest)
- MAPAQ sector profiles are updated more frequently
- Always note the data year when citing statistics
- PLQ membership data may differ slightly from StatCan (different counting methodology)
