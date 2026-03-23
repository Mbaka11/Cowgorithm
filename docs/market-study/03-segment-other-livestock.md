# Segment Analysis: Other Livestock

> Quebec's non-dairy livestock segments — sheep, goats, hogs, and poultry. Virtual fencing applicability varies significantly by species. Sheep and goats are the most promising sub-segments; hogs and poultry have limited relevance.

---

## 1. Quebec Livestock Landscape

### Sheep & Goats

| Metric                     | Value          | Source                                         |
| -------------------------- | -------------- | ---------------------------------------------- |
| Number of farms (QC, 2021) | ~617           | Census 2021: 2.1% of 29,380                    |
| Share of QC farm revenue   | 0.8%           | Census 2021                                    |
| Estimated sheep head (QC)  | ~285,000       | QC agriculture data estimates                  |
| Estimated goat head (QC)   | ~40,000–50,000 | QC agriculture data estimates                  |
| Average flock size (sheep) | ~100–150 ewes  | Industry estimates; growing with consolidation |

**Industry trends**:

- Growing demand for locally-produced lamb (QC imports significant lamb from NZ/Australia)
- Goat dairy (chèvre) is a growing niche adjacent to organic/artisanal food trends
- Quebec accounts for the largest share of sheep farms in eastern Canada
- Many sheep/goat operations use **pasture-based** production — high virtual fencing relevance
- Smaller operations, often less capitalized than dairy, but passionate and innovation-friendly

### Hogs

| Metric                             | Value                             | Source                      |
| ---------------------------------- | --------------------------------- | --------------------------- |
| Number of farms (QC, 2021)         | ~1,263                            | Census 2021: 4.3% of 29,380 |
| Share of QC farm revenue           | 15.7%                             | Census 2021                 |
| QC share of national hog inventory | 29.6%                             | Census 2021                 |
| Average number of pigs per farm    | Growing (+5.1% from 2016 to 2021) | Census 2021 QC Profile      |

**Key characteristics**:

- Quebec = second-largest pork producer in Canada (after Ontario)
- **Almost entirely indoor, confinement-based production** — very limited outdoor/pasture hog operations
- Large, concentrated operations — a small number of farms produce the majority of hogs
- Strict environmental regulations (manure management, phosphorus loading) affect farm expansion
- Virtual fencing has **virtually no applicability** to indoor hog operations

### Poultry & Eggs

| Metric                     | Value | Source                      |
| -------------------------- | ----- | --------------------------- |
| Number of farms (QC, 2021) | ~911  | Census 2021: 3.1% of 29,380 |
| Share of QC farm revenue   | 13.1% | Census 2021                 |

**Key characteristics**:

- Supply-managed (chicken, turkey, eggs) — quota-holders are well-capitalized
- **Almost entirely indoor barn production** — no pasture-based mainstream poultry in QC
- GPS collars are **not practical for poultry** (size, form factor, behavior)
- Some niche free-range/organic poultry could benefit from geofencing but market is very small
- **Excluded from Cowgorithm's addressable market**

---

## 2. Virtual Fencing Applicability by Species

| Species     |     Pasture-Based?      |   Collar Feasible?   |                            Virtual Fencing Value                             |   Priority   |
| ----------- | :---------------------: | :------------------: | :--------------------------------------------------------------------------: | :----------: |
| **Sheep**   | Yes — extensive grazing | Yes — Nofence proven |   **High** — escapes are constant, fencing is expensive for large pastures   |    **A**     |
| **Goats**   | Yes — browsing/pasture  | Yes — Nofence proven | **High** — goats are notorious escape artists; virtual fencing very valuable |    **A**     |
| **Hogs**    |    No — indoor (QC)     | Technically possible |          **Very low** — no pasture use in QC commercial operations           |    **D**     |
| **Poultry** |    No — indoor (QC)     |    Not practical     |             **None** — collar form factor doesn't work for birds             | **Excluded** |

### Sheep: Proven Virtual Fencing Use Case

Nofence (Norway) has a dedicated **sheep and goat collar** that is commercially available:

- Smaller, lighter collar than the cattle version
- Solar-powered GPS with audio warning + mild electric pulse as backup
- Active primarily in Norway, UK, and parts of Europe
- Sheep grazing on open hillsides (commons grazing) is a classic use case
- In Quebec: sheep on pasture benefit from virtual fencing for **rotational grazing, predator management** (keeping flocks together), and **reducing labor** on multi-paddock operations

### Goats: High Escape Behavior = High Value

- Goats are notorious for escaping physical fences, making them a strong fit for virtual fencing
- Goat dairy (chèvre production) is a growing QC niche
- Several Boer goat meat operations also use extensive pasture
- Collar form factor works well on goats

---

## 3. Existing Solutions

| Company         | Species              | Region                      | Product                         | Pricing                 | Notes                                                                                         |
| --------------- | -------------------- | --------------------------- | ------------------------------- | ----------------------- | --------------------------------------------------------------------------------------------- |
| **Nofence**     | Cattle, sheep, goats | Norway, UK, expanding to US | GPS collar with virtual fencing | Subscription + hardware | Only proven multi-species virtual fencing; has sheep/goat collar; solar-powered; HerdNet mesh |
| **Digitanimal** | Cattle, sheep, goats | Spain, Europe               | GPS ear tag / collar tracker    | ~€5–8/animal/month      | GPS tracking and geofence alerts — not active virtual fencing (notification only)             |
| **Farmbrite**   | General livestock    | US/Canada                   | Farm management software        | SaaS subscription       | Software only — no hardware; herd record-keeping                                              |
| **Gallagher**   | All                  | Worldwide (NZ-based)        | Traditional electric fencing    | Hardware purchase       | Physical fencing; no virtual component; well-known brand                                      |

**Competitive gap**: Same as cattle — **no virtual fencing solutions are available in Canada for sheep or goats.** Nofence is the only multi-species virtual fencing company and has not entered Canada.

---

## 4. Market Size (TAM / SAM / SOM)

### Sheep & Goats (Combined)

| Parameter                              | Value                                             |
| -------------------------------------- | ------------------------------------------------- |
| Total addressable animals (QC)         | ~325,000–335,000 head (285K sheep + 40–50K goats) |
| Subscription pricing (smaller animals) | ~$15–20 CAD/animal/month                          |
| Hardware cost (smaller collar)         | ~$150–200 CAD/animal                              |

**TAM Calculation** (Quebec, sheep & goat segment):

```
Annual subscription: 330,000 × $17.50/month × 12 = ~$69M/year
Including hardware (Year 1): 330,000 × ($175 + $210) = ~$127M
```

> **Sheep & Goat TAM (QC): ~$69M/year**

**SAM** (Applying realistic filters):

| Filter                        | Multiplier |
| ----------------------------- | ---------- |
| Pasture-based operations      | ×0.85      |
| Minimum flock size (>50 head) | ×0.50      |
| Connectivity coverage         | ×0.70      |
| **SAM multiplier**            | **×0.30**  |

```
SAM = $69M × 0.30 = ~$21M/year
```

**SOM** (Years 1–3):

Sheep/goat farms are smaller and less capitalized than dairy. Adoption will be slower:

| Year   | Penetration | Farms | Animals | Revenue |
| ------ | :---------: | ----: | ------: | ------: |
| Year 1 |    0.3%     |    ~2 |    ~200 |   ~$42K |
| Year 2 |    1.0%     |    ~6 |    ~700 |  ~$147K |
| Year 3 |    2.5%     |   ~15 |  ~2,000 |  ~$420K |

> **SOM (Year 3): ~$420K/year** — a small but viable addition to the primary dairy segment.

### Hogs

**TAM**: Not meaningful. Virtually all QC hog production is indoor/confinement. Some niche pasture-raised pork exists (~10–20 operations), but too small to pursue.

### Poultry

**TAM**: Zero. GPS collars are not applicable to poultry.

---

## 5. Opportunity Assessment

### Sub-Segment Scoring

| Sub-Segment |    Market Size     | Feasibility | Competition | ROI for Farmer | **Total (1–5)** |
| ----------- | :----------------: | :---------: | :---------: | :------------: | :-------------: |
| **Sheep**   |         3          |      4      |      5      |       3        |    **3.75**     |
| **Goats**   |         2          |      4      |      5      |       4        |    **3.75**     |
| Hogs        | 4 (large industry) |      1      |     N/A     |       1        |    **1.50**     |
| Poultry     | 3 (large industry) |      0      |     N/A     |       0        |    **0.75**     |

### Recommended Priority

1. **Sheep & Goats**: Viable secondary segment. Pursue **after** dairy collar is proven. The same core technology (GPS, cellular, virtual fencing) applies with a smaller form-factor collar. Nofence has already validated the concept globally.

2. **Hogs**: Not a target. Indoor production in Quebec means virtual fencing adds no value. Some monitoring sensors (environmental, activity) could apply eventually, but this is a different product.

3. **Poultry**: Excluded from Cowgorithm's strategy. Form factor and species behavior make GPS collars impractical.

### Strategic Recommendation

- **Do not develop a sheep/goat collar simultaneously with the cattle collar.** Focus resources on dairy first.
- **Design the platform (cloud, app, dashboard) to be species-agnostic** from Day 1 — adding sheep/goat as a second collar hardware SKU should be a straightforward extension, not a redesign.
- Sheep/goat can be marketed as a **"Phase 2 product"** once the dairy business is established (~Year 2–3).

---

## 6. Data Sources

| #   | Source                                       | URL                                                                        | Data Used                                                   | Status   |
| --- | -------------------------------------------- | -------------------------------------------------------------------------- | ----------------------------------------------------------- | -------- |
| 1   | Statistics Canada — Census 2021 (QC Profile) | https://www150.statcan.gc.ca/n1/pub/96-325-x/2021001/article/00005-eng.htm | Farm counts by type, revenue shares, hog trends             | Verified |
| 2   | Nofence — Products page                      | https://nofence.com/products/                                              | Sheep/goat collar availability, HerdNet mesh, solar-powered | Verified |
| 3   | Quebec Agriculture Data Skill                | .github/skills/quebec-agriculture-data.md                                  | Livestock estimates (sheep, goat, hog head counts)          | Internal |
| 4   | TAM Calculation Skill                        | .github/skills/tam-calculation.md                                          | Market sizing methodology                                   | Internal |

---

> **Document Status**: Draft — populated with Census 2021 data and competitor research. Head count estimates for sheep/goats/hogs need verification against MAPAQ profils sectoriels.
>
> **Last Updated**: Phase 2C — Market Study
