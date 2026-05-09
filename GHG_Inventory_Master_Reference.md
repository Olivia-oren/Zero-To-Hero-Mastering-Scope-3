# GHG Inventory Master Reference

**Owner:** Olivia Paul (Oren) — sustainability consultant
**Purpose:** Personal expert-level reference for GHG inventory work across sectors. Built progressively through structured teaching modules.
**Authoritative sources:** GHG Protocol Corporate Standard, Scope 2 Guidance, Corporate Value Chain (Scope 3) Standard, Scope 3 Calculation Guidance.
**Started:** 2026-05-03

---

## Table of Contents

1. [Module 0 — GHG Inventory Process](#m0--ghg-inventory-process)
2. [Module 1 — Boundaries](#m1--boundaries)
3. [Module 2 — Scope 1 Deep Dive](#m2--scope-1)
4. [Module 3 — Scope 2 Deep Dive](#m3--scope-2)
5. [Module 4 — Scope 3 Framework](#m4--scope-3-framework)
6. [Module 5 — Scope 3 Upstream (Cat 1–8)](#m5--scope-3-upstream)
7. [Module 6 — Scope 3 Downstream (Cat 9–14)](#m6--scope-3-downstream)
8. [Module 7 — Scope 3 Special Cases (Cat 15 + Cross-Cutting)](#m7--scope-3-special-cases)
9. [Glossary](#glossary)
10. [References](#references)

---

## M0 — GHG Inventory Process

### What a GHG inventory is
A systematic accounting of the seven Kyoto greenhouse gases an organization emits — directly and indirectly — over a defined reporting period, expressed in tonnes of CO₂-equivalent (tCO₂e), classified into Scope 1, Scope 2, and Scope 3.

### The 7 GHGs
| Gas | Typical sources |
|-----|----------------|
| CO₂ | Fossil fuel combustion, calcination, deforestation |
| CH₄ | Oil & gas leaks, landfills, livestock, coal mines |
| N₂O | Agriculture (fertilizer), nitric/adipic acid, combustion |
| HFCs | Refrigeration, AC, foam blowing |
| PFCs | Aluminum smelting (anode effect), semiconductors |
| SF₆ | Electrical switchgear (insulator gas) |
| NF₃ | Semiconductor manufacturing (added 2013) |

### Calculation backbone
> **Emissions (tCO₂e) = Activity Data × Emission Factor × GWP**

Many EF databases (DEFRA, IEA, EPA) provide factors already in CO₂e (GWP pre-applied). Always check whether your EF is in CO₂ or CO₂e.

### AR5 100-yr GWPs (memorize cold)
| Gas | GWP |
|-----|-----|
| CO₂ | 1 |
| CH₄ | 28 |
| N₂O | 265 |
| HFC-134a | 1,300 |
| HFC-23 | 12,400 |
| SF₆ | 23,500 |
| NF₃ | 16,100 |

### The 6 steps of an inventory
1. Define purpose & set boundaries (org + operational)
2. Identify emission sources (S1, S2, S3 cats)
3. Select calculation methodology per source
4. Collect activity data
5. Apply emission factors + GWPs
6. Calculate, QA/QC, document, report

### The 5 GHG Protocol accounting principles
| Principle | Meaning |
|-----------|---------|
| **Relevance** | Inventory reflects emissions appropriately for decision-makers |
| **Completeness** | Account for all sources within boundaries; disclose exclusions |
| **Consistency** | Use consistent methods year-on-year so trends are real |
| **Transparency** | Clear audit trail; methodology and assumptions documented |
| **Accuracy** | Bias-free; uncertainty managed; verifiable |

### PDF ecosystem — which doc does what
| For… | Use this PDF |
|------|-------------|
| Inventory principles, base year, fundamentals | Corporate Standard |
| Org boundaries (equity/financial/op control) | Corporate Standard Ch 3 |
| Scope 1 calculation overview | Corporate Standard Ch 6 |
| Scope 2 — market-based, dual reporting, RECs/PPAs | Scope 2 Guidance |
| 15 Scope 3 categories — definitions, classification, minimum boundaries | Scope 3 Standard |
| Per-category Scope 3 calculation methods | Scope 3 Calculation Guidance |

### Reporting period & base year
- **Reporting period** — typically fiscal year. Activity data and EFs aligned to this period.
- **Base year** — fixed historical comparison year. Locked when targets set.
- **Recalculation triggers** (GHG-CS Ch 5):
  1. Structural changes (M&A, divestiture, outsourcing, insourcing) crossing threshold (commonly 5%)
  2. Methodology changes (spend → activity-based, EF updates, GWP version change)
  3. Significant data error corrections
- When triggered → recalculate base year + every intervening reporting year retrospectively
- **Trap:** Organic growth is NOT a recalculation trigger; only structural changes are.

### Common error catalogue
1. Boundary mistakes — wrong control approach, missing leased assets, missing JVs
2. Double-counting — Cat 1 cradle-to-gate including transport already in Cat 4
3. Missed Scope 3 cats — esp. Cat 3 (fuel & energy upstream), Cat 11 (use phase), Cat 15
4. GWP mismatches — mixing AR4 and AR5 within same inventory
5. Time period mismatches — FY24 activity data with FY22 EFs
6. Unit errors — kg CO₂ vs kg CO₂e; L vs kg fuel; MWh vs GJ
7. Biogenic confusion — see "Biomass rule" below
8. Offset errors — netting offsets against gross inventory (NEVER)
9. AR5 vs AR6 confusion — pick one, apply uniformly, disclose

### Biomass / biogenic rule (THE critical Scope 1 trap)
| Source | CO₂ | CH₄ | N₂O |
|--------|-----|-----|-----|
| Biomass / biofuel combustion | MEMO LINE (not in scopes) | IN Scope 1 ✓ | IN Scope 1 ✓ |
| Land use change (deforestation, drained wetlands) | IN scopes ✓ | IN scopes ✓ | IN scopes ✓ |
| Fossil fuel combustion | IN scopes ✓ | IN scopes ✓ | IN scopes ✓ |

**Why CO₂ is special for biomass:** Carbon was recently absorbed from atmosphere; combustion returns it. Net flux ≈ 0 if sustainably sourced. CH₄ and N₂O have no such offset.

**Sector-critical for:** pulp & paper, sugar, ethanol, biomass power, agriculture, food processing, palm oil, biomass district heating, carbon black.

### Offsets rule
- **Inventory totals are always GROSS** — never reduce by offsets
- Offsets disclosed **separately** as own line item
- Same rule for insets, avoided emissions (Scope 4), removals
- Correct phrasing: *"Gross inventory = X tCO₂e. We retired Y tCO₂e of offsets, reported separately, not netted."*
- Auditors and SBTi reject net-of-offset inventories

### Worked example — backbone in action
Mumbai office FY24:
| Source | Activity | EF | GWP | tCO₂e |
|--------|----------|----|----|-------|
| Diesel backup gen (Scope 1) | 500 L | 2.68 kg CO₂/L | 1 | 1.34 |
| CH₄ fugitive (Scope 1) | 10 kg | 1 | 28 | 0.28 |
| HFC-134a refrigerant (Scope 1) | 5 kg | 1 | 1,300 | 6.50 |
| Grid electricity (Scope 2) | 50,000 kWh | 0.71 kg CO₂e/kWh | already in EF | 35.50 |

**Lesson:** HFC-134a (5 kg, tiny by mass) generates 4× the diesel emissions. F-gas leaks dominate small-volume fugitive Scope 1 in absurd disproportion to mass.

### Quiz scenarios + answer keys
*Quiz Q0.1–Q0.6 covered: GWP math fluency, M&A base year recalc, GWP-version consistency, doc ecosystem, biomass/biogenic split, offsets netting. See chat transcript for full text and reasoning.*

---

## M1 — Boundaries

### Two boundary types (sequential)
| Type | Question |
|------|----------|
| **Organizational boundary** | Who is "the company"? Which entities consolidate into the inventory? |
| **Operational boundary** | For consolidated entities, which scope (S1/S2/S3) does each emission go into? |

### The 3 organizational boundary approaches
| Approach | Rule | Pick when… |
|----------|------|-----------|
| **Equity share** | % equity ownership × emissions | Material JV exposure; oil & gas, mining |
| **Financial control** | 100% if you have financial control (ability to direct financial + operating policies); 0% otherwise | Holdcos, investment firms, financial reporting alignment |
| **Operational control** | 100% if you operate (full authority to introduce + implement operating policies); 0% otherwise | Most companies globally; CDP default; manufacturers, FMCG, services |

### Single-JV illustration
Same JV, 30% equity, you're the operator, no clear financial control:
| Approach | Counts |
|----------|--------|
| Equity share | 30% |
| Financial control | 0 (no fin control) |
| Operational control | 100% (you operate) |

### Operational boundary — scope assignment
| Scope | Definition |
|-------|-----------|
| **Scope 1** | Direct emissions from sources owned/controlled (per chosen org approach). Combustion, process, mobile, fugitive. |
| **Scope 2** | Indirect from purchased electricity, steam, heat, cooling. |
| **Scope 3** | All other indirect (15 categories, value chain). |

### Leased asset matrix — LESSEE perspective
| Approach | Operating lease | Finance lease |
|----------|-----------------|--------------|
| Equity share | Cat 8 | S1/S2 |
| Financial control | Cat 8 | S1/S2 |
| Operational control | **S1/S2 if you operate, Cat 8 if not** | S1/S2 (you almost always operate finance leases) |

### Leased asset matrix — LESSOR perspective
| Approach | Operating lease | Finance lease |
|----------|-----------------|--------------|
| Equity share | S1/S2 (your equity) | Cat 13 (lessee's equity-like) |
| Financial control | S1/S2 (you keep fin control) | Cat 13 (lessee has fin control) |
| Operational control | **S1/S2 if you operate, Cat 13 if lessee operates** | Cat 13 |

**Mirror rule:** Whatever falls into Cat 8 (lessee's upstream) falls out of Cat 13 (lessor's downstream) — globally counted exactly once.

### Cat 4 vs Cat 8 — the consultant-killer distinction
| Category | When to use | Defining feature |
|----------|-------------|------------------|
| **Cat 4 — Upstream T&D** | You pay a 3PL for transport service. They own + operate trucks. | Buying *services* |
| **Cat 8 — Upstream Leased Assets** | You lease an asset and operate it yourself; lessor has financial control under fin control approach | Leasing *things* |

Decision question: *"Did I pay for transport (service) or lease an asset (thing)?"*

### JV decision flow under each approach
```
Is there a single operator with full authority?
├── YES — Op control: 100% to operator, 0% to others
│         Financial control: depends on contract terms (often = operator)
│         Equity share: % equity for each partner
└── NO — Joint operational control / shared governance
         Op control: strictly 0; disclose with rationale
         Fin control: depends on contractual rights
         Equity share: cleanest — % equity (dual report recommended)
```

### Sector reflexes
- **O&G majors:** dual-report op control + equity share (dense JV networks; investor alignment)
- **Real estate / REITs:** under op control, most building electricity is in tenant S2 + landlord Cat 13 (NOT landlord S2)
- **Cement/manufacturing:** op control standard; JVs without governance → Cat 15 if material
- **Banks:** branches operated directly = S1/S2; BC franchise branches = Cat 14
- **IT/services:** outsourcing of operations shifts S1/S2 → Cat 1 (purchased services), no base year recalc

### Other boundary cases
| Case | Treatment |
|------|-----------|
| Franchises (franchisor view) | Franchisees not in S1/S2; aggregate as **Cat 14** |
| Outsourcing/insourcing | Shifts S1/S2 ↔ Cat 1; **NO base year recalc** |
| M&A | Include from acquisition forward; recalc base year retroactively if structural change > threshold (typ. 5%) |
| Divestiture | Exclude from divestiture forward; recalc base year retroactively (subtract) |
| Internal restructuring (no change in legal control) | No recalc |
| Recently acquired sub with own inventory | Rebase to parent's policy; document methodology change |

### M&A / divestiture recalculation rules
| Trigger | Recalc base year? |
|---------|-------------------|
| Structural change (M&A, divestiture, outsource/insource) > threshold | YES (M&A: add; divest: subtract) |
| Methodology change (EF source, GWP version) | YES |
| Significant data error correction | YES |
| Organic growth (sales/production growth) | NO |
| Outsourcing/insourcing operations | **NO** (anti-gaming rule — voluntary scope shifts don't change real emissions) |

### Documentation must specify
1. Org boundary approach + rationale
2. Structural change threshold (typically 5%)
3. Treatment of each JV (with explicit per-approach call)
4. Treatment of leases (operating vs finance, lessee + lessor stance)
5. Treatment of franchises (if any)
6. Treatment of outsourced ops
7. List of consolidated entities + ownership % + control status
8. List of excluded entities + rationale
9. Date + change log

### Worked example — same company, 3 approaches
"OGEnergy" (O&G holdco):
| Entity | Stake | Operator | Em (tCO₂e) | Op Ctrl | Fin Ctrl | Equity |
|--------|-------|----------|-----------|---------|----------|--------|
| CemCo (100% sub) | 100% | OGE | 500,000 | 500,000 | 500,000 | 500,000 |
| DrillCo (60% JV, partner-operated) | 60% | Partner | 200,000 | 0 | 200,000 | 120,000 |
| ChemCo (30% JV, OGE-operated) | 30% | OGE | 300,000 | 300,000 | 0 | 90,000 |
| HQ Mumbai | 100% | OGE | 1,000 | 1,000 | 1,000 | 1,000 |
| Op-leased trucks (OGE operates) | — | OGE | 5,000 | 5,000 | 0 (Cat 8) | 0 (Cat 8) |
| Finance-leased warehouse (OGE operates) | — | OGE | 100 | 100 | 100 | 100 |
| Op-leased-out buildings (tenants operate) | 100% own | Tenants | 200 | 0 (Cat 13) | 200 | 200 |
| **S1+S2 total** | | | | **806,100** | **701,300** | **711,300** |

Spread = ~105,000 tCO₂e (>13%) on identical physical reality. Boundary choice = primary determinant of inventory size.

### Common errors to flag
1. Putting leased trucks/equipment you operate into Cat 4 (treating asset lease as service purchase)
2. Forgetting Cat 8 under fin control when you operate-but-don't-control assets
3. Counting leased-out building S2 in own S2 under op control (lessee operates → Cat 13)
4. Putting JV without operational control into S1+S2 under op control approach
5. Mixing approaches for different entities (consistency violation)
6. Recalculating base year for outsourcing (it's NOT a trigger)
7. NOT recalculating base year for material M&A
8. Confusing "structural change %" with "equity share %"

### Quiz scenarios + answer keys
*Quiz Q1.1–Q1.8 covered: JV math (3 approaches), HUL operating-leased trucks (Cat 4 vs Cat 8 trap), Embassy REIT per-asset op control, HDFC franchises, TataChem M&A base year, Infosys AWS outsourcing (no recalc rule), Reliance/bp 50-50 joint op control JV, DalmiaCem integration. See chat transcript for full reasoning.*

---

## M2 — Scope 1

### The 4 sub-types
| # | Sub-type | What | Sector dominance |
|---|----------|------|-----------------|
| 1 | Stationary combustion | Fuel in fixed equipment (boilers, kilns, gensets) | Power, cement, steel, chemicals, refineries |
| 2 | Mobile combustion | Fuel in owned vehicles (trucks, ships, aircraft, off-road) | Logistics, mining, construction, airlines |
| 3 | Process emissions | Chemical/physical reactions other than combustion | Cement, steel, aluminum, chemicals, lime |
| 4 | Fugitive emissions | Non-combustion releases (F-gas leaks, CH₄ leaks, CO₂ fire systems) | Refrigeration, O&G, coal, utilities, semiconductors |

### Stationary combustion EFs (DEFRA / IPCC)
| Fuel | Unit | CO₂ EF |
|------|------|--------|
| Diesel | L | 2.68 kg/L |
| Petrol | L | 2.31 kg/L |
| Natural gas | m³ | 1.89 kg/m³ |
| Natural gas | GJ | 56.1 kg/GJ |
| LPG | L | 1.51 kg/L |
| Furnace oil | L | 3.13 kg/L |
| Pet coke | t | 3,400 kg/t |
| Bituminous coal | t | 2,420 kg/t (varies — use ultimate analysis if available) |
| Lignite | t | ~1,400 kg/t |
| Biomass dry | t | 1,600 kg/t (CO₂ → MEMO; CH₄/N₂O → S1) |

### Tier methodology
| Tier | Approach | Use when |
|------|----------|---------|
| 1 | IPCC default EFs | Small sources |
| 2 | Country/region-specific EFs | Medium sources |
| 3 | Facility measurement (CEMS, ultimate analysis) | Large sources >100 ktCO₂/yr |

### Mobile combustion methods
- **Fuel-based** (preferred): L × kgCO₂/L
- **Distance-based** (proxy): km × kgCO₂/km by vehicle type
- Vehicle AC refrigerant = separate fugitive; don't bundle into combustion EF

### Process emissions — sector quick reference
| Sector | Process emission | Scale |
|--------|------------------|-------|
| **Cement** | CaCO₃ → CaO + CO₂ (calcination) | ~525 kg CO₂/t clinker; ~60% of S1 |
| **Steel BF-BOF** | Coke + iron ore reduction → CO₂ | ~1.8–2.0 t CO₂/t crude steel (process) |
| **Steel EAF** | Electrode oxidation + alloy additions | ~0.4 t CO₂/t (low S1, high S2) |
| **Steel DRI** | NG or coal reduction of iron ore | ~1.0 t CO₂/t (gas DRI), higher (coal DRI) |
| **Aluminum** | Anode oxidation (CO₂) + anode effect (CF₄, C₂F₆) | 1.5–1.7 t CO₂/t Al; PFCs add 30–50% |
| **Ammonia (NH₃)** | CH₄ reformer | ~1.6 t CO₂/t NH₃ (process) |
| **Hydrogen (SMR)** | Steam methane reforming | ~9–11 t CO₂/t H₂ (grey) |
| **Nitric acid** | NH₃ → HNO₃; **N₂O byproduct** | 6–9 kg N₂O/t HNO₃ uncontrolled (× 265 GWP = huge) |
| **Adipic acid** | Cyclohexanone oxidation → N₂O | Mostly abated post-2000s |
| **HCFC-22 production** | HFC-23 byproduct (12,400 GWP) | Ex-CDM cash cow |
| **Pulp & paper** | Lime kiln calcination | ~0.1–0.2 t CO₂/t pulp |
| **Glass** | Soda ash + limestone decomposition | ~85 kg CO₂/t glass (process) |
| **Lime** | CaCO₃ calcination (same as cement) | ~785 kg CO₂/t quicklime |

### Fugitive emissions — F-gas reference (AR5 GWPs)
| Gas | GWP | Use case |
|-----|-----|---------|
| HFC-134a | 1,300 | Domestic AC, vehicle AC, chillers |
| HFC-410A | 1,924 | Modern AC |
| HFC-404A | 3,943 | Commercial refrigeration |
| HFC-407C | 1,624 | Mid-tier AC |
| HFC-32 | 677 | Newer ACs (low-GWP) |
| HCFC-22 | 1,810 | Phase-out per Montreal Protocol |
| HFO-1234yf | <1 | New vehicle AC |
| Ammonia | 0 | Industrial refrigeration |
| CO₂ (R-744) | 1 | Eco refrigerant |
| HCs (R-290, R-600a) | 3 | Low-GWP alternatives |
| CF₄ | 6,630 | Aluminum PFC |
| C₂F₆ | 11,100 | Aluminum PFC |
| SF₆ | 23,500 | Electrical switchgear, magnesium |
| NF₃ | 16,100 | Semiconductor |

### Fugitive — refrigerant rule
**Activity data = top-up amount, NOT initial charge.** Charge stays in equipment. Only top-up represents leakage. End-of-life: residual charge counts as fugitive if not recovered.

### Sector trap reflexes
| Sector | Where S1 hides | Common error |
|--------|---------------|--------------|
| Cement | Calcination = 60% of S1 (process, fuel-independent) | Treating "decarbonize cement = clean fuel"; missing alternative cementitious lever |
| Steel BF-BOF | Coke reduction process ~70% of S1 | Confusing process vs combustion in C balance |
| Aluminum | PFCs (CF₄/C₂F₆) from anode effect | Reporting only CO₂ from anode oxidation; missing 30–50% of S1 |
| O&G | Methane fugitive can rival combustion | Using Tier 1 leak rates when actuals are 2–4× higher |
| Chemicals (HNO₃, adipic) | N₂O process | Treating N₂O as trace; often dominates |
| Power utilities | SF₆ from switchgear | Missing entirely; tiny mass, real impact |
| Refrigeration / cold chain | F-gas top-ups | Counting CHARGE instead of TOP-UP (10× overstatement in commissioning year) |
| Pulp & paper | Black liquor + biomass boilers | Putting biogenic CO₂ in S1 OR excluding biomass CH₄/N₂O |
| Cement (alt fuels) | Mixed biogenic/fossil RDF, tires | Treating all AF as one bucket without splitting fossil/biogenic |
| Data centers | Backup diesel + DG refrigerant + cooling F-gas | Missing refrigerant top-up |

### Cement plant — captive power treatment (ULTRA COMMON QUESTION)
- CPP serving cement plant only → **CPP coal = Scope 1 stationary** (you generate, you consume, you control)
- CPP also exports to grid → still S1 for operating company; sold portion is "sold electricity"
- **Trap:** Some treat CPP as Scope 2 because "it's electricity" — wrong. The fuel combustion is what counts; you control the CPP.

### Worked example — full cement plant Scope 1 (1 Mt clinker plant)
| Source | Activity | EF | tCO₂e | Sub-type |
|--------|----------|----|-------|---------|
| Calcination | 1,000,000 t clinker | 525 kg CO₂/t | 525,000 | Process (39%) |
| Kiln coal | 100,000 t | 2,420 kg CO₂/t | 242,000 | Stationary |
| Kiln pet coke | 30,000 t | 3,400 kg CO₂/t | 102,000 | Stationary |
| Captive PP coal | 200,000 t | 2,420 kg CO₂/t | 484,000 | Stationary |
| In-plant haul | 200,000 L diesel | 2.68 kg/L | 536 | Mobile |
| HFC-134a top-up | 50 kg | × 1,300 GWP | 65 | Fugitive |
| SF₆ leak | 2 kg | × 23,500 GWP | 47 | Fugitive |
| **TOTAL S1** | | | **~1,353,648** | |
| Biogenic memo | 5,000 t biomass | 1,600 kg CO₂/t | 8,000 | Memo |

### Cement plant — biomass / RDF biogenic-fossil split
- For each AF stream, lab-test for fossil vs biogenic carbon fraction
- Fossil portion CO₂ → S1 stationary
- Biogenic portion CO₂ → MEMO line
- All CH₄ + N₂O regardless of source → S1 stationary

| AF stream | Typical fossil/biogenic split |
|-----------|-------------------------------|
| Tire-derived fuel | ~70/30 |
| RDF (refuse-derived) | ~60/40 |
| Biomass (rice husk, ag waste) | ~0/100 |
| Sewage sludge | ~30/70 |

### Aluminum smelter — full process S1 example (500 kt Al/yr)
| Component | Calc | tCO₂e |
|-----------|------|-------|
| Anode CO₂ | 500,000 × 1.6 | 800,000 |
| CF₄ (anode effect) | 500,000 × 0.15 kg/t × GWP 6,630 / 1000 | 497,250 |
| C₂F₆ (anode effect) | 500,000 × 0.02 kg/t × GWP 11,100 / 1000 | 111,000 |
| **Total** | | **~1,408,250** |
| **PFCs as % of process** | | **~43%** |

> Aluminum smelters that miss PFCs understate S1 by 30–50%.

### Comprehensive sub-type drill (cement plant) — answer key
| Source | Sub-type / Scope |
|--------|------------------|
| Coal in main kiln | S1 Stationary |
| Limestone calcination | S1 Process |
| In-plant front-end loaders (diesel) | S1 Mobile |
| Refrigerant top-up office AC | S1 Fugitive |
| Coal in captive power plant | S1 Stationary |
| Fly ash purchased + added (no emissions from this addition) | NOT S1 (is in Cat 1 purchase) |
| Biomass rice husk **CO₂** | **MEMO** (biogenic, NOT in S1) |
| Biomass rice husk **CH₄/N₂O** | S1 Stationary |
| Contractor trucks delivering INBOUND limestone (you don't own/operate) | **Cat 4 Upstream T&D** (NOT S1; NOT downstream) |
| SF₆ leak from on-site substation | S1 Fugitive |
| Methane vented from owned/on-property landfill | **S1 Fugitive** (NOT Cat 5 — Cat 5 is third-party landfill) |
| CO₂ from fire suppression discharge | S1 Fugitive (NOT stationary — fire suppression is non-combustion release) |

### Quiz scenarios + answer keys
*Quiz Q2.1–Q2.8 covered: clinker Tier 1 vs Tier 3 (~3% spread), RDF biogenic/fossil split, refrigerant charge vs top-up trap, BF-BOF vs EAF S1 (37× spread), SF₆ utility leak math, O&G methane fugitive, aluminum PFC ~43% of process, cement plant 12-source sub-type drill. See chat transcript for full reasoning + worked numbers.*

---

## M3 — Scope 2

> *To be populated in Module 3*

---

## M4 — Scope 3 Framework

> *To be populated in Module 4*

---

## M5 — Scope 3 Upstream

> *To be populated in Module 5*

### Cat 1 — Purchased Goods & Services
### Cat 2 — Capital Goods
### Cat 3 — Fuel- and Energy-Related Activities (not in Scope 1 or 2)
### Cat 4 — Upstream Transportation & Distribution
### Cat 5 — Waste Generated in Operations
### Cat 6 — Business Travel
### Cat 7 — Employee Commuting
### Cat 8 — Upstream Leased Assets

---

## M6 — Scope 3 Downstream

> *To be populated in Module 6*

### Cat 9 — Downstream Transportation & Distribution
### Cat 10 — Processing of Sold Products
### Cat 11 — Use of Sold Products
### Cat 12 — End-of-Life Treatment of Sold Products
### Cat 13 — Downstream Leased Assets
### Cat 14 — Franchises

---

## M7 — Scope 3 Special Cases

> *To be populated in Module 7*

### Cat 15 — Investments (Financed Emissions, PCAF)
### Avoided Emissions (Scope 4)
### Biogenic CO2
### Carbon Offsets
### GWP Versions (AR4 / AR5 / AR6)
### Recalculation Triggers

---

## Glossary

> *Built progressively through modules*

---

## References

- **GHG-CS** — *GHG Protocol Corporate Accounting and Reporting Standard*, Revised Edition (`ghg-protocol-revised.pdf`)
- **GHG-S2** — *GHG Protocol Scope 2 Guidance* (`Scope 2 Guidance.pdf`)
- **GHG-S3** — *Corporate Value Chain (Scope 3) Accounting and Reporting Standard* (`Corporate-Value-Chain-Accounting-Reporing-Standard.pdf`)
- **GHG-S3-Calc** — *Technical Guidance for Calculating Scope 3 Emissions* (`Scope3_Calculation_Guidance.pdf`)
- **PCAF** — Partnership for Carbon Accounting Financials (referenced in M7 for Cat 15)
- **IPCC AR5/AR6** — IPCC Assessment Reports (source of GWP values)
- **DEFRA/BEIS** — UK Department for Environment, Food & Rural Affairs (annual EF database)
- **EPA eGRID** — US EPA grid emission factors
- **CEA** — Central Electricity Authority of India (Indian grid factors)
- **ecoinvent / GaBi / EXIOBASE / IDEA** — LCA emission factor databases
