# Development, Test, And Field Pipeline

This diagram shows the project as a technical production line rather than a
one-off demo.

![Development, test, and field pipeline](../assets/diagrams/development-field-pipeline.png)

Editable source:
[development-field-pipeline.svg](../assets/diagrams/development-field-pipeline.svg).

## What It Shows

The left side starts with BCH bench work: design, schemas, synthetic data,
bench captures, replay, review, and promotion. From there the work splits into
two linked lanes.

The physical validation lane moves from bench assumptions to STG integration,
then toward QST as a transportable or fixed field case connected to SeaTalk
NG / NMEA 2000 sensors. The output is survey evidence and promotion gates, not
unreviewed live control.

The TVL DevOps lane proves the operational machinery: Lima vz, macOS
containers, Kubernetes, Flux, GitOps, SignalK, InfluxDB, Grafana, survey
dashboards, remote debugging, and field-style development.

Terraform, Ansible, and cloud-init matter because rebuildability is part of
the platform, not an afterthought. Future sensor applications may include Go
or Rust collectors and narrowly justified WASM validators, but only where they
show measured benefit.

## Why It Matters

The maturity signal is that development, validation, survey, observability,
and release gates are distinct. That same shape can apply beyond boating: any
physical-system project that needs edge telemetry, replay, disciplined
deployment, and evidence before promotion.

## Public Boundary

This page intentionally omits IPs, hostnames, credentials, live topology,
private runbooks, and actuator details.
