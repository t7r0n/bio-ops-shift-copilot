# Failure Matrix: Bio Ops Shift Copilot

| Scenario | Failure mode | Metric | Gate | Evidence |
| --- | --- | --- | --- | --- |
| wastewater evidence replay | wastewater_drift | wastewater_coverage | block release until cited evidence is regenerated | ev_0000 |
| biological operator packet | biological_blindspot | biological_latency | accept only if decision claims cite fixture evidence | ev_0007 |
| biological operator packet | biological_blindspot | biological_latency | accept only if decision claims cite fixture evidence | ev_0011 |
| reason regression harness | reason_misroute | reason_precision | open a regression issue with trace and benchmark delta | ev_0014 |
| operators boundary probe | operators_gap | operators_risk | route to reviewer with evidence packet | ev_0021 |
| reason regression harness | reason_misroute | reason_precision | open a regression issue with trace and benchmark delta | ev_0022 |
| wastewater evidence replay | wastewater_drift | wastewater_coverage | block release until cited evidence is regenerated | ev_0028 |
