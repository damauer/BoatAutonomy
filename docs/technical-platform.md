# Technical Platform

BoatAutonomy is publicly framed around calmer docking, but the technical
platform is broader. It combines marine telemetry, replay, edge operations,
multi-agent engineering, governance, and safety boundaries into a pattern that
could matter to other physical-system projects.

This page is intentionally public-safe. It describes the shape of the system
without publishing private topology, live endpoints, raw telemetry, actuator
details, or operational runbooks.

## Platform Shape

![BoatAutonomy platform pattern](../assets/diagrams/boat-autonomy-platform.png)

Editable source:
[boat-autonomy-platform.svg](../assets/diagrams/boat-autonomy-platform.svg).

## Maturity Signals

The public repository does not expose the private implementation, but it can
show the shape of a mature platform:

- It is replay-first. New behavior should be tested against recorded or
  synthetic sessions before it is trusted near live vessel behavior.
- It is evidence-driven. Decisions, assumptions, reviews, and caveats are
  recorded as part of the engineering process.
- It has separation of duties. Implementation, review, research, and owner
  approval are distinct roles.
- It uses infrastructure deliberately. Kubernetes supports recording,
  monitoring, replay, orchestration, and supervisory services, not hard
  real-time safety control.
- It keeps data boundaries visible. Raw telemetry, private dashboards, live
  topology, and operational details stay outside the public repo.
- It treats autonomy as staged capability: capture, replay, observe, estimate,
  shadow, assist.

## Why Technologists Should Care

Many physical-system projects fail to separate a compelling demo from an
operable platform. BoatAutonomy is being shaped around the harder concerns
early:

- Can the system explain what happened after a session?
- Can a new behavior be replayed before it is trusted?
- Can AI-generated work be reviewed and governed?
- Can edge services tolerate intermittent connectivity?
- Can evidence survive across rebuilds, migrations, and incidents?
- Can model output be kept away from direct physical authority until a safety
  case exists?

That makes the project relevant beyond recreational docking. The same pattern
could apply to field robotics, small-vessel systems, industrial telemetry,
remote infrastructure, training systems, survey workflows, or other domains
where autonomy has to earn trust through evidence.

## Current Boundary

This is not a commercial product claim. It is not a safety certification. It
does not publish live control paths. The public claim is that the project is
building a serious, reviewable substrate for staged autonomy research and
future marine assistance.
