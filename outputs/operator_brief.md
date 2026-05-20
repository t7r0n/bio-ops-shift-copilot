# Operator Brief: Nyad

Nyad gets a local, deterministic pressure test around wastewater, operators, and reason. The useful part is the repeatable evidence path from fixture to failure to operator action.

## Highest-leverage checks

- wastewater evidence replay -> block release until cited evidence is regenerated (wastewater_coverage, evidence ev_0088).
- biological operator packet -> accept only if decision claims cite fixture evidence (operators_risk, evidence ev_0099).
- reason regression harness -> open a regression issue with trace and benchmark delta (reason_precision, evidence ev_0022).
- operators boundary probe -> route to reviewer with evidence packet (biological_latency, evidence ev_0121).

## What makes this useful

The workflow is intentionally local and deterministic. A reviewer can run the same fixture set, inspect the evidence IDs, open the dashboard, and see exactly why a recommendation passed, went to review, or blocked.
