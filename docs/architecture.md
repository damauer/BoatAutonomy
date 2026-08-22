# Architecture

BoatAutonomy uses a staged architecture. Each layer earns promotion with
recorded evidence before the next layer is allowed to depend on it.

## Planes

```mermaid
flowchart TB
  subgraph Vessel["Vessel Interface"]
    Sensors["Read-only marine bus tap"]
    FutureIO["Future isolated actuator interface"]
  end

  subgraph Edge["Edge Runtime"]
    Recorder["Capture and timestamp"]
    Decoder["Decode and normalize"]
    Store["Local storage and replay artifacts"]
  end

  subgraph Platform["Lab and Cluster Platform"]
    Replay["Replay services"]
    Dashboards["Dashboards and queries"]
    CI["Checks, review packets, and release gates"]
  end

  subgraph Control["Future Safety-Control Boundary"]
    Operator["Human enable and override"]
    Limits["Deterministic limits and watchdogs"]
    SafeState["Safe state on fault"]
  end

  Sensors --> Recorder --> Decoder --> Store --> Replay --> Dashboards
  CI --> Replay
  Dashboards --> CI
  FutureIO --> Limits
  Operator --> Limits --> SafeState
```

## Design Rules

- Observe before estimating.
- Replay before shadow mode.
- Shadow mode before assist.
- Assist only with operator enable, physical override, bounded outputs, and
  fault handling.
- Keep raw vessel data, packet captures, and large artifacts outside public Git.
- Treat model output as a request to a bounded controller, not as a command.
- Keep Kubernetes, dashboards, and agents outside the hard real-time safety
  path.

## What The Public Repo Shows

The public repo can show normalized examples, synthetic telemetry, architecture
summaries, evidence formats, review discipline, and safety constraints.

It should not show live topology, internal network names, endpoint addresses,
real vessel tracks, raw captures, private dashboards, credentials, or detailed
procedures for operating the private system.
