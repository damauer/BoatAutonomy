# Safety Boundary

BoatAutonomy is intentionally safety-gated. The project is allowed to explore
instrumentation, replay, state estimation, and supervised assistance. It is not
allowed to skip from demos to live vessel authority.

![BoatAutonomy safety boundary](../assets/diagrams/safety-boundary.png)

Editable source:
[safety-boundary.svg](../assets/diagrams/safety-boundary.svg).

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
  runbooks.

## Control Principle

Future assistive behavior must be bounded by deterministic control, operator
enable, heartbeat and freshness checks, sensor validity checks, rate limits,
safe-state behavior, and immediate physical override.

Until that boundary is explicitly designed, reviewed, and approved, public
work remains observation, replay, evidence, and architecture.
