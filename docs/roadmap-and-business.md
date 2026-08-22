# Roadmap And Business Direction

BoatAutonomy may eventually become relevant to recreational boating,
marine-service, autonomy, edge-AI, or adjacent physical-system markets. This
page records that direction without claiming the project is ready for product,
customer, funding, or safety-certification conversations today.

## Capability Roadmap

This roadmap describes capability order, not delivery promises.

![BoatAutonomy staged roadmap](../assets/diagrams/roadmap-stages.png)

Editable source:
[roadmap-stages.svg](../assets/diagrams/roadmap-stages.svg).

### Stage 0 - Governance And Safety

Define what agents may do, what requires owner approval, how evidence is
recorded, and what must remain outside the public repo.

### Stage 1 - Passive Telemetry

Capture and decode marine-network data without writing to the vessel bus or
controlling anything physical.

### Stage 2 - Replay And Observability

Replay captured or synthetic telemetry into repeatable dashboards, queries,
and tests. Use replay to debug before touching the real vessel.

### Stage 3 - State Estimation

Estimate vessel state from sensors and environmental context. Compare
estimates against replayed sessions before considering live use.

### Stage 4 - Shadow Mode

Run assistive logic in observation-only mode. The system may predict what it
would request, but it does not influence control.

### Stage 5 - Supervised Docking Assist

Only after explicit design review and owner approval, test bounded assistive
behavior with operator enable, immediate physical override, deterministic
limits, watchdogs, and safe-state handling.

### Stage 6 - Higher Autonomy Research

Any higher-autonomy work remains research until it has passed safety analysis,
evidence gates, failure injection, and owner approval. The public repo should
not imply this stage exists in production.

## Market Hypothesis

![BoatAutonomy market and business fit](../assets/diagrams/market-business-fit.png)

Editable source:
[market-business-fit.svg](../assets/diagrams/market-business-fit.svg).

The first emotional product promise is simple: make docking feel less
intimidating. From there, the possible market expands carefully:

- Assistance for recreational boaters in close-quarters maneuvering.
- Replay and coaching tools that help owners learn from real outings.
- Better instrumentation for service yards, marinas, surveyors, and fleet
  operators.
- Retrofit-friendly telemetry and awareness systems for existing boats.
- Transferable patterns for other small vessels or edge autonomy use cases
  where safety, intermittent connectivity, and human authority matter.

The desired feeling is not "the robot took over." It is closer to:

- I understand what the boat is doing.
- I can replay what happened and learn from it.
- The system helps me see wind, current, heading, speed, depth, and control
  context more clearly.
- Assistance appears only after the sensing, replay, safety, and operator
  boundaries are proven.
- The owner remains in command.

## Why It Could Matter Later

- Recreational and small-commercial marine systems have real operational pain:
  docking stress, intermittent connectivity, noisy sensors, fragmented
  electronics, and limited observability.
- Modern AI and edge infrastructure make new assistance patterns possible, but
  the safety case matters more than the demo.
- A solo founder with governed agent support can cover more ground if scope,
  evidence, and approval boundaries are explicit.
- The builder brings cloud, embedded, protocol, operations, commercial, and
  founder-side experience to a project that needs all of those at once.

## Reasonable Public Conversation Now

- The public technical thesis.
- The staged roadmap from passive telemetry to replay, shadow mode, and
  supervised assistance.
- The builder's background and founder-side business context.
- The governance model for AI-assisted engineering.
- The safety boundary and why direct control remains private and gated.
- Synthetic demos and sanitized evidence summaries.
- The market vision as a hypothesis, not a product-readiness claim.

## Not Ready For Public Claims

- Product launch timing.
- Customer commitments.
- Revenue claims.
- Funding terms, valuation, or equity structure.
- Safety certification or real vessel-control readiness.
- Market-size claims not backed by separately reviewed evidence.
- Live topology, implementation repos, raw telemetry, vessel-specific details,
  private dashboards, or operational procedures.

## Current Status

Exploration-stage project. Public-facing technical surface. No current
fundraising solicitation. No product-readiness claim. Future business
conversations should require a separate, owner-approved private diligence
packet.
