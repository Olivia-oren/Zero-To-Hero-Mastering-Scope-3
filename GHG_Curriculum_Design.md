# GHG Inventory Mastery — Curriculum Design

**Owner:** Olivia Paul (Oren)
**Goal:** Become an expert in GHG inventory consulting — Scope 1, 2, 3 classification and calculation, across all sectors, framework-agnostic (GHG Protocol-pure).
**Date:** 2026-05-03

---

## Format

- **Modular teaching** — module-by-module, each with theory → worked example → quiz
- **Permanent reference document** — `GHG_Inventory_Master_Reference.md`, populated as we progress
- **Quizzes** — 8–12 sector-tagged classification scenarios per module; build classification reflexes
- **Framework-agnostic** — GHG Protocol Corporate Standard + Scope 2 Guidance + Scope 3 Standard + Scope 3 Calculation Guidance as authoritative sources; PCAF only where GHG Protocol defers to it (Cat 15)
- **Sectoral coverage** — balanced across heavy industry, manufacturing, FMCG, services, financial, energy/utilities

---

## Source Documents

1. **`ghg-protocol-revised.pdf`** — GHG Protocol Corporate Accounting and Reporting Standard (Revised Edition) — *the foundational doc; covers inventory process, boundaries, Scope 1, Scope 2, basics of Scope 3*
2. **`Scope 2 Guidance.pdf`** — GHG Protocol Scope 2 Guidance (2015 update) — *introduces market-based method, dual reporting, contractual instrument hierarchy*
3. **`Corporate-Value-Chain-Accounting-Reporing-Standard.pdf`** — Corporate Value Chain (Scope 3) Standard — *defines the 15 Scope 3 categories, classification rules, minimum boundaries*
4. **`Scope3_Calculation_Guidance.pdf`** — Technical Guidance for Calculating Scope 3 Emissions — *per-category calculation methods, formulas, data sources*

---

## Module Structure

### M0: GHG Inventory Process *(orientation — light)*
- The 6 steps of an inventory: business goals → boundaries → categorize sources → calculate → QA/QC → report
- Where errors enter (boundary mistakes, double-counting, missed Scope 3 cats, GWP version mismatches, time period misalignment)
- The PDF ecosystem — which doc applies when, how they nest
- The activity data × emission factor × GWP backbone

### M1: Boundaries *(foundational)*
- **Organizational boundary** — Equity share / Financial control / Operational control. Decision tree, defaults, how the choice changes Scope 1 vs Scope 3
- **Operational boundary** — assigning consolidated entities' emissions across S1/S2/S3
- **Edge cases:** JVs, minority stakes, operating vs finance leases, franchises, subsidiaries with different parents, recent M&A, divestitures, base year recalculation triggers
- Leased asset puzzle — interactions with Cat 8 / Cat 13 depending on control approach

### M2: Scope 1 *(deep)*
- **Stationary combustion** — boilers, furnaces, kilns, on-site generators
- **Mobile combustion** — owned/leased fleet (vehicles, aircraft, ships, off-road equipment)
- **Process emissions** — sector deep dives: cement calcination, chemicals (ammonia, ethylene, F-gas production, nitric/adipic acid), steel (BF-BOF), aluminum (PFCs), pulp & paper, fertilizer, glass
- **Fugitive emissions** — F-gases (HFCs, PFCs, SF6, NF3), methane leaks (oil & gas, coal mining, landfills), CO2 from fire suppression
- Sector traps: cement, chemicals, oil & gas, data centers, food cold chain, power generation
- Worked example: cement plant full Scope 1 calculation

### M3: Scope 2 *(deep)*
- Definition: indirect emissions from purchased electricity, steam, heat, cooling
- **Location-based** vs **market-based** methods
- Quality Criteria hierarchy for market-based (RECs/GOs/I-RECs → PPAs → supplier-specific → residual mix → grid-average)
- Mandatory dual reporting rule (2015 Scope 2 Guidance update)
- Edge cases: on-site solar PV, behind-the-meter, virtual PPAs, sold renewables, exported electricity, district heating, T&D losses (Cat 3, not Scope 2)
- Sector traps: data centers, services firms, IT/SaaS

### M4: Scope 3 Framework *(medium)*
- Why Scope 3 dominates most companies' footprint (>70% typical)
- The 15 categories at a glance — 8 upstream (Cat 1–8), 7 downstream (Cat 9–15)
- Methodology hierarchy: supplier-specific → hybrid → average activity-based → spend-based
- Materiality screening (sector relevance)
- Minimum boundaries per category
- Common databases: ecoinvent, EXIOBASE, EPA SPEND, DEFRA/BEIS, GaBi, IDEA
- Pedigree matrix (data quality 1–5)
- Time period alignment, double-counting risks, recalculation triggers, biogenic CO2 / avoided emissions / offsets handling

### M5: Scope 3 Upstream (Cat 1–8) *(heaviest module — likely split into 2 sessions)*
- **Cat 1** Purchased Goods & Services — methods, EF databases, allocation
- **Cat 2** Capital Goods — boundary with Cat 1
- **Cat 3** Fuel & Energy — WTT + T&D losses; the most-missed category
- **Cat 4** Upstream T&D — inbound logistics; double-count traps
- **Cat 5** Waste — treatment-specific methods; avoided emissions trap
- **Cat 6** Business Travel — distance-based vs spend-based; RFI for flights
- **Cat 7** Commuting — survey vs proxy; WFH energy
- **Cat 8** Upstream Leased Assets — interaction with control approach

### M6: Scope 3 Downstream (Cat 9–14) *(deep)*
- **Cat 9** Downstream T&D — outbound transport not paid by you
- **Cat 10** Processing of Sold Products — for intermediate goods
- **Cat 11** Use of Sold Products — direct vs indirect use phase; oil & gas / autos / appliances / SaaS
- **Cat 12** End-of-Life of Sold Products — disposal mix × treatment EFs
- **Cat 13** Downstream Leased Assets — lessor perspective (mirror of Cat 8)
- **Cat 14** Franchises — franchisors aggregate franchisees' S1+S2

### M7: Scope 3 Special Cases *(hardest)*
- **Cat 15 Investments / Financed Emissions** — PCAF asset class methodologies; attribution factors; data quality 1–5
- **Avoided emissions** (Scope 4) — never in inventory
- **Biogenic CO2** — memo item; LUC exception
- **Carbon offsets** — never reduce inventory totals
- **GWP version choice** — AR5 vs AR6
- **Recalculation triggers** — structural changes, methodology updates
- Sector-specific guidance pointers (ICAO/IATA, ISO 14064, GHG Protocol sector standards)
- Final boss quiz: 12–15 hardest scenarios

---

## Quiz Format

After each module: 8–12 sector-tagged classification scenarios. Format:
> **Scenario:** ABC Cement operates a kiln burning pet coke (combustion) and converting limestone to clinker (calcination). They run a captive 5MW coal power plant feeding only their own grinding mills. The kiln uses ammonia-based NOx control. They lease (operating lease) a fleet of 30 cement trucks for delivery. They use F-gases in office HVAC.
>
> **Classify each emission stream — which scope, which category if Scope 3, calculation method.**

Olivia answers; Claude corrects/refines; we discuss. Scenarios stored with answer keys in master reference doc.

---

## Reference Document Structure

**File:** `GHG_Inventory_Master_Reference.md` (Markdown; convertible to Word later)

Per module:
- Concept summary
- Decision rules / decision trees
- Calculation method ranking with formulas
- Per Scope 3 category: definition box, minimum boundary, methods ranked, EF databases, common errors, sector applicability matrix
- Sector trap callouts
- Worked examples
- Quiz scenarios + answer keys
- PDF citations

---

## PDF Grounding Strategy

- Reference PDFs as authoritative; don't read all 4 cover-to-cover up front
- Teach with expert knowledge + cite PDF chapter/page where relevant
- For controversial / edge-case rules, read the relevant PDF section to ground in actual text
- Verbatim extraction available on request

---

## Pacing

- M0 + M1: light + foundational — can pair in one session
- M2, M3: one module each
- M4: medium framework
- M5: heaviest — likely split into 2 sub-sessions (Cat 1–4 and Cat 5–8)
- M6: one module
- M7: deepest, dedicated session
- ~9 effective sessions total
