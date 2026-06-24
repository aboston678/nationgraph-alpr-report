# The RFP Is the Last Signal — NationGraph Public-Safety Market Brief

A single-page, NationGraph-branded data report on license-plate readers. **Positioning:** NationGraph reconstructs the *buying motion before the RFP* — council minutes, capital budgets, grants, sole-source letters — vs. reactive bid/spend tools that start when the RFP posts.

## Thesis
"The RFP is the last signal. NationGraph finds the ones before it." By the time an ALPR bid posts, the buying motion has usually been visible for months in non-bid public records.

## Structure
Hero → the pain → **one deal timeline (North Port, FL — 5 yrs of dated breadcrumbs before the bid feed saw it)** → six-stage buying-signal lifecycle + NationGraph-vs-tools table → proof set (167/82/29) → Fact 1 (RFP is late) · Fact 2 (buyer is hidden, ~65% municipal) · Fact 3 (demand contestable, 154/13) · Fact 4 (timing decides winnability) · Fact 5 (long tail, median 53k) → US map → Signal Library → Validation (timing, independent sources) → signal-to-action workflow → vendor playbook → CTA.

## Honesty guardrails (load-bearing)
- **North Port, not Cincinnati**, is the pre-RFP example. Cincinnati's $300K LPR budget line is dated 2025-07-01 — *after* its RFPs — so it cannot illustrate "budget before RFP." Removed.
- **~65%** (municipal record), not ~90% — sheriffs and state police are law-enforcement records.
- **No "average X months early" headline** — the data supports the signal *types* and named real trails (North Port, Coeur d'Alene), not a market-wide lead-time average.
- Counts not dollars; solicitations are the conservative floor; every breadcrumb links to a real dated source.

## Stack
Static `index.html`, no build. Interactive US map via d3 + public-domain us-atlas. Deployed on Vercel → nationgraph-alpr-report.vercel.app.
