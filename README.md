# BoatAutonomy

Toward calmer docking and smarter marine assistance, one evidence-gated
subsystem at a time.

BoatAutonomy is a public-safe view into a private, owner-built autonomy lab
around a recreational boat. The working shorthand is "teaching my boat how to
dock itself." The more precise public claim is narrower and more important:
build the telemetry, replay, edge compute, safety policy, and multi-agent
review harness needed before a real vessel can responsibly move from passive
observation toward supervised docking-assist experiments.

This repository is intentionally curated. It does not publish the private
implementation, live topology, raw vessel data, credentials, repair procedures,
or operational runbooks.

## Why Read This

Docking is one of the most stressful and least forgiving moments in
recreational boating. Wind, current, visibility, crew coordination, close
quarters, spectators, and expensive hardware all converge at low speed.

That human problem is simple to understand, but technically hard to address
responsibly. A useful system has to observe before it estimates, replay before
it recommends, and earn trust before it gets anywhere near authority.

BoatAutonomy is worth reading because it treats that problem as a real
physical-system challenge, not a demo script. It asks how a small team, aided
by governed AI agents, can build a serious autonomy substrate while preserving
safety, evidence, review, and owner control.

## What This Is

BoatAutonomy is a public-facing project surface for a private applied-autonomy
lab. For now, it is a portfolio and credibility surface for relevant technical
work. If the project matures, this same surface may eventually support
conversations with marine partners, advisors, technical collaborators, or
funding sources.

That is not the current posture. This repo is not a product certification,
pitch deck, securities offering, live-system runbook, or claim that autonomous
docking is complete. It is a controlled way to show the technical thesis,
builder context, safety posture, and evidence discipline behind the private
project.

Current public scope:

- Marine telemetry capture and replay using SeaTalk NG / NMEA 2000 concepts.
- SignalK-style normalized data paths and dashboard-driven inspection.
- Edge and cluster operations for repeatable lab, staging, and field workflows.
- Evidence records that separate observed facts, assumptions, risks, and
  approvals.
- A governed multi-agent development loop where implementation, review,
  research, and owner approval are deliberately separate.

This repository does not claim unattended autonomous docking. It does not
publish live vessel-control code, actuator wiring, raw capture files, endpoint
details, secrets, or enough operational detail to reproduce the private system.

## How It Works

![BoatAutonomy platform pattern](assets/diagrams/boat-autonomy-platform.png)

Editable source: [boat-autonomy-platform.svg](assets/diagrams/boat-autonomy-platform.svg).

BoatAutonomy is organized as a replay-first, evidence-gated platform around a
real recreational vessel. Marine signals enter as captured observations. Edge
and cluster services normalize, replay, inspect, and test those observations.
AI, dashboards, and agents may help interpret evidence or propose work, but
human authority, physical override, and safe-state behavior remain explicit.

Kubernetes and agentic tooling are useful around the system: recording,
monitoring, replay, perception experiments, observability, and deployment
repeatability. They are not the hard real-time safety controller and do not
receive direct actuator authority.

The public story follows this order:

- Shape the system before naming tools.
- State the safety boundary before implying capability.
- Show evidence discipline before asking for trust.
- Add technical and agentic breadcrumbs only after the boundary is clear.

The best starting sequence is:
[architecture.md](docs/architecture.md),
[safety-boundary.md](docs/safety-boundary.md),
[evidence.md](docs/evidence.md), then
[technical-platform.md](docs/technical-platform.md).

<table>
  <tr>
    <td width="33%">
      <a href="docs/architecture.md">
        <img src="assets/diagrams/architecture-boundary.png" alt="System shape thumbnail" width="240">
      </a>
      <br>
      <a href="docs/architecture.md"><strong>System shape</strong></a>
      <br>
      Staged architecture, hard boundary, and human authority.
    </td>
    <td width="33%">
      <a href="docs/technical-platform.md">
        <img src="assets/diagrams/development-field-pipeline.png" alt="Technical platform thumbnail" width="240">
      </a>
      <br>
      <a href="docs/technical-platform.md"><strong>Technical platform</strong></a>
      <br>
      Edge operations, replay, GitOps, telemetry, and field workflow.
    </td>
    <td width="33%">
      <a href="docs/ai-and-agentic-collaboration.md">
        <img src="assets/diagrams/agentic-collaboration-harness.png" alt="AI and agentic collaboration thumbnail" width="240">
      </a>
      <br>
      <a href="docs/ai-and-agentic-collaboration.md"><strong>AI and agentic collaboration</strong></a>
      <br>
      Claude Code, Codex, Grok, tmux, GitLab records, review, and reconciliation.
    </td>
  </tr>
</table>

## Why It Matters

BoatAutonomy has value because it combines an intuitive market problem with a
serious engineering method.

For boaters and marine operators, the possible value is calmer close-quarters
handling, better situational awareness, better training feedback, and more
useful evidence from existing marine electronics.

For technologists, the deeper signal is that this is not a single demo script.
It is an emerging platform pattern with several mature pieces being exercised:

- Data and replay: raw marine signals become normalized, replayable sessions
  that can be inspected before new behavior is trusted.
- Edge operations: lab, staging, production, and field-style environments
  support repeatable deployment and evidence collection.
- AI-assisted engineering: multiple agents work in bounded roles for research,
  implementation, review, and evidence, with the owner retaining approval.
- Safety and governance: model output is treated as advice to a bounded
  system, not direct physical authority.
- Transferability: the same pattern may apply to other markets where physical
  systems need telemetry, replay, edge intelligence, and human-centered
  control boundaries.

The AI story has two layers. One layer is how the project is built: Claude
Code, Codex, Grok, tmux, GitLab records, review findings, and owner decisions
are coordinated so speed does not erase accountability. The other layer is
future model-assisted behavior, which remains bounded by replay, shadow mode,
operator enablement, and safety review.

Read [ai-and-agentic-collaboration.md](docs/ai-and-agentic-collaboration.md)
for the conceptual overview and
[agentic-engineering.md](docs/agentic-engineering.md) for the GitLab-centered
workflow with YAML and Markdown examples.

## Where It Is Going

The capability order still comes first:
[roadmap.md](docs/roadmap.md) describes progression from governance and
passive telemetry toward replay, estimation, shadow mode, and supervised
assist before any higher autonomy research.

The market lens is intentionally ambitious but bounded:

- Make docking and close-quarters handling calmer for recreational boaters.
- Turn raw marine electronics into useful, replayable operating evidence.
- Build retrofit-friendly capabilities that respect existing vessels,
  owners, marinas, service yards, and safety expectations.
- Use AI and agents to accelerate engineering, analysis, and support while
  keeping physical authority bounded.
- Preserve a path beyond recreational docking if the same telemetry, replay,
  and safety-gated assistance patterns prove useful elsewhere.

Read [market-vision.md](docs/market-vision.md) for the product intuition and
[future-business-direction.md](docs/future-business-direction.md) for the
cautious future business framing. The latter is explicitly not a current
fundraising solicitation or product-readiness claim.

## How We Can Help

The project started as curiosity and skill-building. It now defines a useful
intersection of the builder's career: embedded and real-time systems,
communications-traffic analysis, secure cloud architecture, isolated
environments, data resiliency, Kubernetes, edge operations, and AI-assisted
software delivery.

It also reflects commercial and founder-side business experience: consulting,
business development, customer delivery, CFO / CIO support, and long-running
small-business operations.

This project is a portfolio surface for relevant work opportunities and future
partner conversations. It makes visible a combination of systems engineering,
cloud-to-edge operations, AI-assisted delivery, governance, and business
judgment that can help adjacent physical-system and autonomy efforts.

See [RESUME.md](RESUME.md) for the public resume,
[docs/relevant-work.md](docs/relevant-work.md) for the kinds of work this
project is meant to make legible, and
[docs/portfolio-narrative.md](docs/portfolio-narrative.md) for the through-line
connecting the project to prior systems work.

## Repository Map

- [docs/architecture.md](docs/architecture.md) - staged system architecture
  and safety/control-plane split.
- [docs/safety-boundary.md](docs/safety-boundary.md) - what the project does
  and does not authorize.
- [docs/evidence.md](docs/evidence.md) - sanitized examples of evidence the
  private project records before promoting work.
- [docs/technical-platform.md](docs/technical-platform.md) - deeper technical
  platform view for technologists.
- [docs/ai-and-agentic-collaboration.md](docs/ai-and-agentic-collaboration.md) -
  AI, agent collaboration, replay, model boundaries, and governance.
- [docs/agentic-engineering.md](docs/agentic-engineering.md) - how the
  multi-agent build/review/research loop is governed, with YAML and Markdown
  examples.
- [docs/roadmap.md](docs/roadmap.md) - capability progression from passive
  telemetry to supervised assistance.
- [docs/market-vision.md](docs/market-vision.md) - market-facing product
  intuition without product-readiness claims.
- [docs/future-business-direction.md](docs/future-business-direction.md) -
  cautious future business direction, explicitly not a current solicitation.
- [docs/relevant-work.md](docs/relevant-work.md) - professional positioning
  and opportunity fit.
- [docs/portfolio-narrative.md](docs/portfolio-narrative.md) - why this
  project is a credible continuation of the builder's career arc.
- [RESUME.md](RESUME.md) - public resume context.
- [demos/synthetic-nmea/](demos/synthetic-nmea/) - small synthetic telemetry
  example for public demos and screenshots.

## Public Review Status

Draft only. The private project owner must approve content before any GitHub
repository, profile, release, screenshot, or demo is made public.
