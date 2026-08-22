# Agentic Collaboration Harness

This diagram shows the management system around the technical work: agents,
reviews, research, observable sessions, GitLab records, and publication
boundaries.

![Agentic collaboration harness](../assets/diagrams/agentic-collaboration-harness.png)

Editable source:
[agentic-collaboration-harness.svg](../assets/diagrams/agentic-collaboration-harness.svg).

## What It Shows

The implementation loop uses Claude Code for bounded implementation, observable
tmux sessions for long-running work, GitLab work records for merge requests,
tasks, milestones, commits, reviews, and reconciliation notes, and Codex for
iterative independent review.

The research loop uses Grok for domain and build research. Codex reviews fit,
governance, and risk before implementation proceeds. Tower is represented as
a private local model lane for local LLM and model-training experiments.

The persistence layer matters. Local and edge GitLab repos hold operational
truth. GitLab.com backs up durable records. GitHub mirrors approved
public-facing artifacts.

## Why It Matters

The point is not simply that multiple AI tools are used. The point is that the
work is managed:

- Research, implementation, review, governance, and approval are separate.
- Findings are reconciled into fixes, deferrals, blockers, or owner decisions.
- Observable sessions reduce hidden work.
- Git-backed records make the project auditable across machines and time.
- Private implementation stays separate from public positioning.

## Public Boundary

This page describes process shape. It does not expose credentials, endpoints,
private repository contents, session transcripts, raw data, or operational
runbooks.
