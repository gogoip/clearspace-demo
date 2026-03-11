# clearspace-demo

## ClearScape Vantage Workload Telemetry Demo

Primary deliverable: `notebooks/clearscape_vantage_workload_telemetry_demo.ipynb`.

The notebook demonstrates a notebook-first workflow for:
- validating Vantage telemetry access (DBQL query, DBQL step, ResUsage),
- generating controlled workload signatures in a demo schema,
- deriving workload buckets (`etl`, `bi`, `ad_hoc`) from DBQL telemetry,
- analyzing workload pressure, outliers, and skew with raw telemetry IDs (`QueryID`, `StepID`, sample time, node).

It intentionally avoids a synthetic `workload_map` or generic event table in v1, and keeps the telemetry-to-insight path transparent in SQL + pandas cells.
