# Phase 3 — Google Cloud Engineering

**Weeks:** 10–18 · **Budget:** 36 hours

## Weekly plan
| Week | Focus | Lab and evidence |
|---|---|---|
| 10 | Projects, billing, IAM, service accounts | Project setup, budget alert, least-privilege notes |
| 11 | Artifact Registry and Cloud Storage | Push image and store non-sensitive artifact |
| 12 | VPC, subnets, firewall, DNS | Network diagram and connectivity test |
| 13 | Compute Engine | Small VM, SSH access and teardown record |
| 14 | Cloud Run | Deploy Rails container and validate health |
| 15 | Cloud SQL | Secure Rails connection to managed PostgreSQL |
| 16 | HTTPS and load balancing | Routing and TLS notes |
| 17 | Cloud Logging and Monitoring | Dashboard and actionable alert |
| 18 | Security and architecture review | ADR, IAM review and cost/cleanup review |

## Guardrails
- Set billing budgets/alerts before provisioning resources.
- Use a dedicated lab project where possible.
- Never commit service-account keys or secrets.
- Prefer workload/user identity and federation over long-lived keys.
- Cloud Run is the first deployment target; Kubernetes comes later.
- Delete paid resources after labs. Budget alerts are notifications, not hard spending caps.

## Exit criteria
- [ ] Explain project, IAM, VPC and service-account boundaries.
- [ ] Deploy Rails to Cloud Run.
- [ ] Connect to Cloud SQL without embedding credentials in the repository.
- [ ] Inspect logs and metrics.
- [ ] Produce architecture diagram and cost/cleanup checklist.

## References
- [Google Cloud documentation](https://cloud.google.com/docs)
- [Google Cloud Skills Boost](https://www.cloudskillsboost.google/)
- [Cloud Run](https://cloud.google.com/run/docs)
- [Cloud SQL](https://cloud.google.com/sql/docs)
- [Google Cloud Architecture Framework](https://cloud.google.com/architecture/framework)
