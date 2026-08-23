# Synthetic NMEA-Style Telemetry

This directory contains public-safe sample data. The values are synthetic and
do not come from a real vessel, route, marina, or capture session.

The shape is intentionally simple: timestamped normalized paths with values
and units. It is enough to build public screenshots, demo parsers, or example
dashboards without exposing private telemetry.

![Public-safe SignalK survey intake visual](../../assets/evidence/signalk-survey-intake.png)

The visual above shows how this sample shape can appear as a SignalK-style
data browser and survey intake artifact. The displayed values are synthetic or
redacted; the Maretron-style device inventory is redrawn from private survey
evidence with unique identifiers withheld.

## Source Shape

```csv
timestamp,source,path,value,unit
2026-01-01T12:00:00Z,synthetic,electrical.batteries.house.voltage,12.74,V
2026-01-01T12:00:01Z,synthetic,environment.depth.belowTransducer,4.8,m
```
