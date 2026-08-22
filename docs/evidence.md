# Evidence

The private project records evidence before treating work as complete. Public
evidence is summarized and sanitized. It is meant to show engineering
discipline, not to publish live operational details.

## Evidence Types

- Checklists that separate planned gates from completed gates.
- Review records that lead with findings, blockers, and residual risk.
- Soak-test summaries with scope, duration, restarts, caveats, and excluded
  incident windows.
- Replay artifacts tied to schema versions, timestamps, and checksums.
- Screenshots or dashboards generated from synthetic or redacted data.
- Decision records that distinguish accepted design from advisory research.

## Sanitized Examples

| Area | Public-Safe Summary |
| --- | --- |
| Telemetry capture | Marine-network captures were decoded into normalized telemetry paths and replayed into dashboards for inspection. |
| Soak testing | Edge telemetry stacks were soak-tested with documented restarts, resource behavior, incident windows, and unresolved caveats. |
| Cluster migration | Infrastructure changes were reviewed against live evidence before promotion, including discovery, network identity, and control-plane behavior. |
| Agent review | Independent review caught real defects before live changes, including assumptions that did not match runtime interfaces. |
| Data handling | Raw telemetry, packet captures, credentials, and large artifacts stay out of public Git; public demos use synthetic data. |

## Public Demo Data

The sample under [demos/synthetic-nmea](../demos/synthetic-nmea/) is synthetic.
It is shaped like normalized marine telemetry but is not from a real vessel,
marina, route, customer, or field session.
