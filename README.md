# 9 of 10 Government Buyers Are Invisible to Your Prospect List — NationGraph Public-Safety Market Brief

A single-page, NationGraph-branded data report. The flagship finding: vendors selling to public safety filter prospect lists to "police agency" records and silently miss ~90% of the buying authority, which sits in **city and county procurement**. Automated license-plate readers (ALPR) are the **proof case**.

**Spine:** The market leader isn't the problem — your filters are. We mapped every public-safety plate-reader RFP we could find and checked how the buyers are classified.

## Key figures (Jan 2024 – Jun 2026)
- **~90%** of buyers are not filed under a "police agency" record type
- **≥167** unique plate-reader solicitations (deduplicated) from **≥82** agencies across **29** states
- **92%** open to competitive bid · only **8%** sole-source (rare in every year, never above ~10%)
- Buyer composition: municipal PD 77 · county/sheriff 19 · state LE 10 · police agency 8 · federal/other 5
- Among the 48 municipal buyers with population on record: median jurisdiction ~53,000; two-thirds under 100k

## Method
- Public-safety buyers only (parking, housing authorities, transit, schools, universities filtered out)
- **Counts, not dollars** — the cleanest demand signal
- Deduplicated by normalized source URL; unresolved records excluded → every figure is a floor
- **Solicitations (buying intent), not award records** — we measure how deals are opened and structured, not who wins

## Stack
Static single-file site (`index.html`), no build step. Deployed on Vercel.
