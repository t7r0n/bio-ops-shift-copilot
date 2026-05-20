# Bio Ops Shift Copilot

A shift-level wastewater operations copilot that turns synthetic microscopy/process logs into explainable biological state, confidence bands, and operator handoff notes.

![Bio Ops Shift Copilot working dashboard](outputs/project_working.svg)

## Why it exists

wastewater operators need AI help that can reason over biological process state without pretending sensor-free predictions are certain.

Most internal demos stop at a pretty chart. This repository is built around the harder part: a repeatable path from fixture, to failure, to evidence, to the operator action a serious team would actually trust.

## What is inside

- A deterministic replay harness tuned around wastewater, operators, and reason.
- Company-specific strategy code in `src/bio_ops_shift_copilot/strategy.py`, not just README-level customization.
- Citation-locked reports where every decision claim has to point back to a generated evidence ID.
- Two visual artifacts generated from the latest run: `outputs/project_working.svg` and `outputs/evidence_map.svg`.
- A portable demo pack with JSON, CSV, Markdown, HTML, SVG, and benchmark artifacts.

![Bio Ops Shift Copilot evidence map](outputs/evidence_map.svg)

## Signals it measures

- `wastewater coverage`
- `operators risk`
- `reason precision`
- `biological latency`

## Failure modes it plants

- wastewater drift
- operators gap
- reason misroute
- biological blindspot

## Run it locally

```bash
uv sync
uv run bio-ops-shift-copilot all
uv run pytest -q
uv run ruff check .
```

## Outputs worth opening

- `outputs/dashboard.html`
- `outputs/project_working.svg`
- `outputs/evidence_map.svg`
- `outputs/operator_brief.md`
- `outputs/decision_report.md`
- `outputs/strategy_model.json`
- `outputs/demo_pack.zip`

## Sources

- https://www.nyad.ai/
- https://www.nyad.ai/about
- https://www.linkedin.com/company/nyad-ai

## Boundary

Everything runs locally against synthetic fixtures. There are no credentials, no customer records, no outreach files, and no hosted API dependency.
