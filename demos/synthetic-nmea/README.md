# Synthetic NMEA-Style Telemetry

This directory contains public-safe sample data. The values are synthetic and
do not come from a real vessel, route, marina, or capture session.

The shape is intentionally simple: timestamped normalized paths with values
and units. It is enough to build public screenshots, demo parsers, or example
dashboards without exposing private telemetry.

## Example

```csv
timestamp,source,path,value,unit
2026-01-01T12:00:00Z,synthetic,electrical.batteries.house.voltage,12.74,V
2026-01-01T12:00:01Z,synthetic,environment.depth.belowTransducer,4.8,m
```
