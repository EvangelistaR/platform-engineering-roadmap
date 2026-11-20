# Phase 7 — Observability, SRE and FinOps

**Weeks:** 42–46 · **Budget:** 20 hours

## Weekly plan
| Week | Focus | Lab and evidence |
|---|---|---|
| 42 | Prometheus and Grafana | Rails/cluster dashboard |
| 43 | OpenTelemetry | Instrument request traces and metrics |
| 44 | Logs, metrics and traces | Correlate request and investigate failure |
| 45 | Alerting, SLO and incidents | Alert rule, runbook and postmortem |
| 46 | FinOps | Cost review and optimization recommendations |

## Rails instrumentation ideas
- HTTP request duration and error rate.
- Database query latency.
- Sidekiq queue depth and job failures.
- External dependency latency.
- Process memory and runtime metrics.

Avoid high-cardinality labels. Never emit credentials, tokens or sensitive personal data into telemetry.

## Exit criteria
- [ ] Explain logs, metrics and traces and when to use each.
- [ ] Correlate an application request across telemetry.
- [ ] Define an SLI and measurable SLO.
- [ ] Create an actionable alert and runbook.
- [ ] Write a blameless postmortem for a simulated incident.
- [ ] Identify cost drivers and clean up unused resources.

## References
- [Prometheus](https://prometheus.io/docs/introduction/overview/)
- [Grafana](https://grafana.com/docs/)
- [OpenTelemetry](https://opentelemetry.io/docs/)
- [Google SRE resources](https://sre.google/books/)
- [Google Cloud cost management](https://cloud.google.com/cost-management)
