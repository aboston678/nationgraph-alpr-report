# Pre-RFP Lead-Time Analysis — Gate Result

**Verdict: ❌ GATE FAILS. Do not ship the lead-time report.**

Genuine, dated, ALPR-specific signals that *predate* the agency's own RFP exist for **~9 of 82 agencies** (≤13 even counting weak/ambiguous cases). The gate threshold was ~15. The data does **not** currently back a "NationGraph surfaces the average ALPR buyer X months before the RFP" claim.

Method: pulled budgets, council/board meeting minutes, press releases, and grants for all 82 resolved ALPR agencies, filtered to ALPR text, read the snippets to drop false positives (parking-management LPR, "vigilant tax collection," "flock of flamingos," moped-DMV plates, operational news), and matched each genuine signal's date against that agency's earliest ALPR RFP due date.

## Matched pre-RFP cases (every one we could find)

| Agency | Earliest pre-RFP signal | Type | RFP (due) | Lead (days) | Quality |
|---|---|---|---|---|---|
| Coeur d'Alene, ID | 2024-06-18 | council minutes — sole-source ALPR trailer | 2024-07-10 | 22 | clean |
| East Ridge, TN | 2024-01-11 | council minutes — install/operate fixed ALPR | 2024-03-13 | 62 | clean |
| Mequon, WI | 2023-12-31 | budget — Flock camera expansion | 2024-05-01 | 122 | clean |
| Sayreville, NJ | 2025-09-23 | minutes — Flock contract award | 2025-11-16 | 54 | ambiguous (award before "RFP") |
| San Marcos, TX | 2025-01-31 | minutes — Flock contract amendment | 2026-02-13 | 378 | ongoing program |
| Genesee County, MI | 2023-04-01 | grant — Byrne earmark (broad LPR mention) | 2024-06-25 | 451 | weak (multi-item earmark) |
| Ormond Beach, FL | 2023-10-01 | grant — JAG to procure LPRs | 2025-01-17 | 474 | clean-ish |
| Dunnellon, FL | 2024-01-03 | minutes — LPR discussion | 2026-02-09 | 768 | possibly a different item |
| North Port, FL | 2020-06-18 | minutes — ALPR presentation | 2025-08-01 | 1,870 | multi-cycle (5-yr program) |

**Clean, same-procurement pre-RFP signals: only 3** (Coeur d'Alene, East Ridge, Mequon). The rest are ongoing-program renewals, broad federal earmarks, or plausibly a different procurement than the matched RFP. No defensible median; the "clean" three are 22 / 62 / 122 days.

## Two showcase cases run BACKWARD (important)
- **Cincinnati, OH** — the celebrated "$300,000 Fixed License Plate Reader Cameras" capital-budget line is dated **2025-07-01**, *after* Cincinnati's ALPR RFPs (2022-11, 2023-10, 2024-10). The budget funds the *next* phase; it is **not** a pre-RFP signal. The "Anatomy of a Deal" breadcrumb is chronologically reversed.
- **Cedar Rapids, IA** — the only genuine ALPR budget hit (FY2026, 2025-07-01, "begun procurement of the FLOCK camera system") postdates its 2024-05 RFP. Post-RFP.

## What NationGraph captures vs. misses (signal coverage, n=82)
- **Meeting minutes** — richest pre-RFP source, but ingested for only ~14/82 agencies; ~7 had genuine ALPR content. This is where the real lead-time signal lives.
- **Budgets / CIP** — keyword hits for ~21/82, but mostly (a) generic annual budgets, (b) **parking-management** LPR, (c) decade-old 2009–2013 lines, or (d) post-RFP. Several had **null document dates** (unusable per "no undated signals"). Genuine + dated + pre-RFP: ~2–3.
- **Grants** — present but broad (JAG/Byrne earmarks bundling LPRs with boats, tasers, radios); only ~2 weak matches.
- **Press releases** — effectively zero useful pre-RFP procurement signal (dominated by moped-DMV-plate notices, "citizens flocked to libraries," operational "ALPR alert located suspect").
- **RFI / sources-sought / notice-of-intent** — not captured as a distinct, dated signal type at all.

## To make the lead-time claim true, NationGraph would need to ingest:
1. **Council/commission AGENDAS** (not just minutes) for all agencies — the earliest dated pre-RFP signal, and present for far more agencies than currently covered.
2. **CIP/capital-budget line items with reliable dates** — many budget docs have null `document_date`; undated = unusable.
3. **RFIs / sources-sought / notices of intent** as a distinct, dated signal type.
4. **De-noising**: separate police ALPR from parking LPR; disambiguate vendor "Vigilant/Flock" from "vigilance / flock of birds."
5. **Cross-institution program linkage**: join a PD's procurement to its city/county budget+minutes (the same filing blindspot the report is about), and resolve signals→RFP at the *program* level so first-buys are distinguishable from renewals.

## Separate correction (applies regardless)
The report's "~90% of buyers aren't a 'police agency' record" overclaims — sheriffs and state police *are* law-enforcement records. The defensible figure is **~65%** filed under non-LE **municipal** records (77 of 119 named buyers = 65%). Use 65%.
