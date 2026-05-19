# Bio Ops Shift Copilot

A shift-level wastewater operations copilot that turns synthetic microscopy/process logs into explainable biological state, confidence bands, and operator handoff notes.

## Why This Exists

wastewater operators need AI help that can reason over biological process state without pretending sensor-free predictions are certain.

## What It Builds

- Replays synthetic `wastewater` and `operators` cases against the project's evidence rules.
- Scores `wastewater_coverage`, `operators_risk`, and `reason_precision` so regressions are visible in CSV and JSON.
- Plants `wastewater drift` and `operators gap` failures as negative controls.
- Writes citation-locked decision claims; unsupported claims fail verification.
- Exports a review dashboard and demo pack for `bio-ops-shift-copilot` without hosted services.

## Local Run

```bash
uv sync
uv run bio-ops-shift-copilot all
uv run pytest -q
uv run ruff check .
```

## Outputs

- `outputs/analysis.json`
- `outputs/scenario_report.csv`
- `outputs/decision_report.md`
- `outputs/evidence_packet.md`
- `outputs/dashboard.html`
- `outputs/demo_pack.zip`

## Sources

- https://www.nyad.ai/
- https://www.nyad.ai/about
- https://www.linkedin.com/company/nyad-ai

## Boundary

This repository uses synthetic fixtures only. It has no credentials, no customer data, no outreach data, and no dependency on a hosted API.
