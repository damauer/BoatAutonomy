# Publication Guidelines

This repo is designed to be public-facing, not automatically public. Owner
approval is required before publication.

## Allowed

- Architecture summaries.
- Safety-boundary language.
- Synthetic telemetry.
- Redacted dashboards.
- Public resume or portfolio wording approved by the owner.
- Public-safe future business-direction language approved by the owner, as
  long as it is explicit that no current solicitation is being made.
- Market-facing language approved by the owner, as long as it preserves the
  current research/exploration status and avoids unsupported market-size
  claims.
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
- Fundraising terms, valuation claims, investment-offer language, customer
  commitments, revenue claims, or safety-certification claims.
- Unsupported global market-size claims or statements that imply product
  readiness, regulatory approval, insurance acceptance, or commercial
  deployment.
- Implementation details that materially reduce the safety or privacy of the
  private system.
- Verbatim resume details that add unnecessary inference risk, including street
  address, personal phone number, clearance specifics, protected customer
  details, or sensitive program identifiers.

## Review Before Publish

Before any commit becomes public, run a plain-text scan for addresses,
credentials, hostnames, serials, personal names, location data, and internal
repository names. Then perform a human review for overclaiming, privacy
leakage, and instructions that would make the private system easier to attack
or misuse.
