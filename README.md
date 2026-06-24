# Open Season on the Plate-Reader Market — NationGraph Public Safety Market Brief

A single-page, NationGraph-branded data report on automated license-plate-reader (ALPR) demand across U.S. public-safety agencies.

**Claim:** Since January 2024, at least **81 police departments, sheriff's offices, and state law-enforcement agencies** across **29 states** have put automated license-plate readers out to bid. Just **8%** were written as sole-source, no-bid awards — the other **92% are open, competitive solicitations**.

## Key figures (Jan 2024 – Jun 2026)
- **≥167** unique plate-reader solicitations from public-safety buyers (deduplicated)
- **≥81** distinct agencies in-market across **29** states
- **92%** open competitive bids vs **8%** sole-source
- Buyers: municipal PD (77) · county/sheriff (19) · state LE (10) · police agency (8) · federal/other (5)
- Named vendor: vendor-neutral 149 · Flock Safety 11 · Motorola/Vigilant 3 · Rekor 3 · Genetec 1

## Method
- Public-safety buyers only (parking, housing authorities, transit, schools, universities filtered out)
- **Counts, not dollars** — the cleanest demand signal
- Deduplicated by normalized source URL; unresolved records excluded → every figure is a floor
- Solicitations (buying intent), not award records

## Stack
Static single-file site (`index.html`), no build step. Deployed on Vercel.
