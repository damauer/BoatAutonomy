# Publication Guidelines

This repo is designed to be public-facing, not automatically public. Owner
approval is required before publication.

## Allowed

- Architecture summaries.
- Safety-boundary language.
- Synthetic telemetry.
- Redacted dashboards.
- Public resume or portfolio wording approved by the owner.
- Sanitized evidence summaries that preserve caveats and residual risk.
- General references to SeaTalk NG, NMEA 2000, SignalK-style data models,
  Kubernetes, edge compute, and multi-agent workflows.

## Not Allowed

- Credentials, tokens, keys, kubeconfigs, or recovery material.
- Public IPs, private IPs, hostnames, tunnels, or topology details.
- Raw vessel telemetry, packet captures, videos, screenshots with location
  data, or routes.
- Marina, yard, vendor, quote, repair, serial, or equipment-specific packets.
- Live dashboards, operational endpoints, admin paths, or runbooks.
- Unreviewed claims that the boat docks itself unattended.
- Implementation details that materially reduce the safety or privacy of the
  private system.

## Review Before Publish

Before any commit becomes public, run a plain-text scan for addresses,
credentials, hostnames, serials, personal names, location data, and internal
repository names. Then perform a human review for overclaiming, privacy
leakage, and instructions that would make the private system easier to attack
or misuse.
