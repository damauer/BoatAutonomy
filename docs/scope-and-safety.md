# Scope And Safety

BoatAutonomy is intentionally safety-gated. The project may explore
instrumentation, replay, state estimation, and supervised assistance. It may
not skip from demos to live vessel authority.

![BoatAutonomy safety boundary](../assets/diagrams/safety-boundary.png)

Editable source:
[safety-boundary.svg](../assets/diagrams/safety-boundary.svg).

## Public Scope

The public repo may show:

- Marine telemetry capture and replay using SeaTalk NG / NMEA 2000 concepts.
- SignalK-style normalized data paths and dashboard-driven inspection.
- Edge and cluster operations for repeatable lab, staging, and field workflows.
- Evidence records that separate observed facts, assumptions, risks, and
  approvals.
- A governed multi-agent development loop where implementation, review,
  research, and owner approval are deliberately separate.
- Synthetic demos, redacted screenshots, diagrams, and public-safe summaries.

The public repo does not publish the private implementation, live topology,
raw vessel data, credentials, repair procedures, endpoint details, or
operational runbooks.

## Current Claims

- The project can capture, decode, replay, and inspect marine telemetry.
- The project can use edge services and clusters for observability and
  repeatability.
- The project can use AI agents to help implement, review, and research
  bounded tasks.
- The project can document decisions, risks, assumptions, approvals, and
  evidence.

## Non-Claims

- No claim of unattended autonomous docking.
- No claim that AI agents may control a live vessel.
- No claim that Kubernetes is a safety controller.
- No claim that dashboards, models, or network services provide physical
  override.
- No publication of live actuator design, wiring, credentials, or operational
  procedures.

## Control Principle

Future assistive behavior must be bounded by deterministic control, operator
enable, heartbeat and freshness checks, sensor validity checks, rate limits,
safe-state behavior, and immediate physical override.

Until that boundary is explicitly designed, reviewed, and approved, public
work remains observation, replay, evidence, and architecture.

## Reader Takeaway

The project is ambitious, but the public claim is deliberately constrained:
BoatAutonomy is building a serious, reviewable substrate for staged autonomy
research and future marine assistance, not declaring that the boat already
docks itself.
