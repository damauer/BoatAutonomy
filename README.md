# BoatAutonomy

Teaching a boat to dock itself, with evidence before authority.

BoatAutonomy is a public-safe view into a private, owner-built autonomy lab
around a recreational boat. The working shorthand is "teaching my boat how to
dock itself." The more precise public claim is narrower and more important:
build the telemetry, replay, edge compute, safety policy, and multi-agent
review harness needed before a real vessel can responsibly move from passive
observation toward supervised docking-assist experiments. The near-term method
is an instrumented survey of the boat and its electronics, feeding the
developing digital twin needed to simulate and develop against observed vessel
behavior before consuming live vessel time.

This repository is intentionally curated. It is a discussion surface, not a
contribution project: read, comment, and ask questions, but there is no implied
pull-request workflow until a later license and contribution policy exist. It
does not publish the private implementation, live topology, raw vessel data,
credentials, repair procedures, or operational runbooks.

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

Read [problem-and-opportunity.md](docs/problem-and-opportunity.md) for the
problem statement and opportunity framing.

## What This Is

BoatAutonomy is a public-facing project surface for a private applied-autonomy
lab. For now, it is a portfolio and credibility surface for relevant technical
work. If the project matures, this same surface may eventually support
conversations with marine partners, advisors, technical collaborators, or
funding sources.

The lab is young, started in May 2026. Its evidence and governance plane is
ahead of any assistive behavior.

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

Read [scope-and-safety.md](docs/scope-and-safety.md) for the public/private
boundary and [evidence.md](docs/evidence.md) for the evidence posture.

## How It Works

![BoatAutonomy platform pattern](assets/diagrams/boat-autonomy-platform.png)

Editable source: [boat-autonomy-platform.svg](assets/diagrams/boat-autonomy-platform.svg).

BoatAutonomy is organized as a replay-first, evidence-gated platform around a
real recreational vessel. Marine signals enter as captured observations. Edge
and cluster services normalize, replay, inspect, and test those observations.
AI, dashboards, and agents may help interpret evidence or propose work, but
human authority, physical override, and safe-state behavior remain explicit.

The instrumented survey is the bridge between the real vessel and the
development environment. Surveyed electronics, telemetry, and operating
context become replayable sessions and simulation inputs for a developing
digital twin. This is not a completed high-fidelity physics model or an
assistive-control claim; it is the practical substrate for finding interface,
timing, and behavior issues before field time is spent on them.

Kubernetes and agentic tooling are useful around the system: recording,
monitoring, replay, perception experiments, observability, and deployment
repeatability. They are not the hard real-time safety controller and do not
receive direct actuator authority.

The public story follows this order:

- Shape the system before naming tools.
- State the safety boundary before implying capability.
- Show evidence discipline before asking for trust.
- Add technical and agentic breadcrumbs only after the boundary is clear.

Read [system-platform.md](docs/system-platform.md) for the system shape,
staged architecture, delivery pipeline, and technical breadcrumbs.

<table>
  <tr>
    <td width="33%">
      <a href="docs/scope-and-safety.md">
        <img src="assets/diagrams/safety-boundary.png" alt="Scope and safety thumbnail" width="240">
      </a>
      <br>
      <a href="docs/scope-and-safety.md"><strong>Scope and safety</strong></a>
      <br>
      Public scope, non-claims, and the physical authority boundary.
    </td>
    <td width="33%">
      <a href="docs/system-platform.md">
        <img src="assets/diagrams/development-field-pipeline.png" alt="Technical platform thumbnail" width="240">
      </a>
      <br>
      <a href="docs/system-platform.md"><strong>System platform</strong></a>
      <br>
      Edge operations, replay, GitOps, telemetry, and field workflow.
    </td>
    <td width="33%">
      <a href="docs/evidence.md">
        <img src="assets/evidence/grafana-marina-telemetry-public-safe.png" alt="Evidence thumbnail" width="240">
      </a>
      <br>
      <a href="docs/evidence.md"><strong>Evidence</strong></a>
      <br>
      Sanitized examples, replay evidence, and public-safe dashboard artifacts.
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
- Instrumented survey and digital twin: measured vessel and electronics
  behavior becomes a replay and simulation substrate for offline development.
- Edge operations: lab, staging, field-prep, and field-style environments
  support repeatable deployment and evidence collection.
- AI-assisted engineering: multiple agents work in bounded roles for research,
  implementation, review, and evidence, with the owner retaining approval.
- Safety and governance: model output is treated as advice to a bounded
  system, not direct physical authority.
- Transferability: the same pattern may apply to other markets where physical
  systems need telemetry, replay, edge intelligence, and human-centered
  control boundaries.

The cost and schedule benefit is direct: more defects can be found in replay,
simulation, and review, and fewer debugging cycles have to wait for scarce
boat time, weather windows, marina conditions, or one-off field setups.

The AI story has two layers. One layer is how the project is built: Claude
Code, Codex, Grok, tmux, GitLab records, review findings, and owner decisions
are coordinated so speed does not erase accountability. The other layer is
future model-assisted behavior, which remains bounded by replay, shadow mode,
operator enablement, and safety review.

Read [agentic-engineering.md](docs/agentic-engineering.md) for the agentic
collaboration harness, GitLab-centered workflow, YAML policy example, and
review Markdown example.

## Where It Is Going

The capability order still comes first:
[roadmap-and-business.md](docs/roadmap-and-business.md) describes progression
from governance and passive telemetry toward replay, estimation, shadow mode,
and supervised assist before any higher autonomy research.

The market lens is intentionally ambitious but bounded:

- Make docking and close-quarters handling calmer for recreational boaters.
- Turn raw marine electronics into useful, replayable operating evidence.
- Build retrofit-friendly capabilities that respect existing vessels,
  owners, marinas, service yards, and safety expectations.
- Use AI and agents to accelerate engineering, analysis, and support while
  keeping physical authority bounded.
- Preserve a path beyond recreational docking if the same telemetry, replay,
  and safety-gated assistance patterns prove useful elsewhere.

That same page also captures the product intuition and cautious future business
framing. It is explicitly not a current fundraising solicitation or
product-readiness claim.

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

See [builder-profile.md](docs/builder-profile.md) for the project/career
through-line and [RESUME.md](RESUME.md) for the public resume.

## Story Guide

The supporting files are grouped by the same questions the README answers.
Read straight down for the narrative, or jump to the part that matches the
conversation you want to have.

| Story Beat | Reader Question | Supporting Pages |
| --- | --- | --- |
| Why read this | What problem makes this worth attention? | [problem-and-opportunity.md](docs/problem-and-opportunity.md) |
| What this is | What is public, what is private, and what is not being claimed? | [scope-and-safety.md](docs/scope-and-safety.md), [evidence.md](docs/evidence.md), [synthetic demo data](demos/synthetic-nmea/) |
| How it works | What is the system shape and technical approach? | [system-platform.md](docs/system-platform.md) |
| Why it matters | Why is the evidence/control plane ahead of assistive behavior? | [agentic-engineering.md](docs/agentic-engineering.md), [evidence.md](docs/evidence.md) |
| Where it is going | What is the capability path and future business hypothesis? | [roadmap-and-business.md](docs/roadmap-and-business.md) |
| How we can help | What skills, experience, and judgment does this make visible? | [builder-profile.md](docs/builder-profile.md), [RESUME.md](RESUME.md) |

## Public Review Status

Draft only. The private project owner must approve content before any GitHub
repository, profile, release, screenshot, or demo is made public.
