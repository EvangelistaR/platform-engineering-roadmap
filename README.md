# Platform Engineering Roadmap

A practical 52-week journey toward Platform Engineering, using Google Cloud as the primary cloud, Terraform for Infrastructure as Code, Docker and Kubernetes for workloads, and Ruby on Rails as the reference application. The final phase introduces a safe, auditable Agentic DevOps MVP.

## Learning profile
- Time: 4 hours/week; approximately 208 hours over 52 weeks.
- Primary cloud: Google Cloud Platform (GCP). AWS is a later follow-up.
- Infrastructure: Terraform.
- Containers/orchestration: Docker, Kubernetes, GKE and Helm.
- Platform workflow: GitHub Actions, GitOps and Argo CD.
- Reference application: Ruby on Rails, PostgreSQL and optionally Sidekiq.
- AI: Ruby-first. Python is deferred unless a concrete ecosystem requirement justifies it.
- Tracking: GitHub Issues, pull requests and weekly progress log.

## Start here
1. Read [ROADMAP.md](ROADMAP.md).
2. Review [the weekly progress log](progress/weekly-log.md).
3. Follow the eight guides in [phases/](phases/).
4. Start with [Phase 1](phases/phase-01-infrastructure/README.md).

## Weekly schedule
| Day | Time | Focus |
|---|---:|---|
| Tuesday | 1h | Focused theory and official documentation |
| Thursday | 1h | Small lab or experiment |
| Saturday | 2h | Implementation, troubleshooting and documentation |
| Monday / Wednesday | — | No scheduled study |

## Roadmap
| Phase | Weeks | Focus | Main outcome |
|---|---:|---|---|
| 1 | 1–4 | Infrastructure fundamentals | Linux/networking labs and scripts |
| 2 | 5–9 | Docker engineering | Containerized Rails reference app |
| 3 | 10–18 | Google Cloud | Rails deployed on GCP |
| 4 | 19–24 | Terraform | Reproducible GCP infrastructure |
| 5 | 25–34 | Kubernetes and GKE | Rails workload running on GKE |
| 6 | 35–41 | Platform Engineering | CI/CD, GitOps and a Golden Path |
| 7 | 42–46 | Observability, SRE and FinOps | Dashboards, SLOs and runbooks |
| 8 | 47–52 | Agentic DevOps | Auditable operational-agent MVP |

## Working agreements
- Prefer official documentation and small experiments over passive course consumption.
- Every week produces evidence: code, configuration, diagram, runbook, test or lab report.
- Do not mark work complete just because a tutorial was watched.
- Keep cloud costs controlled: local-first labs, billing alerts, short-lived resources and teardown steps.
- Never commit credentials, service-account keys, Terraform state, .env files or sensitive logs.
- Use least privilege. AI agents start read-only; consequential actions require human approval.
- Preserve Ruby/Rails as the reference application; do not restart from programming fundamentals.

## Definition of done for a week
- [ ] Learning objective summarized in your own words.
- [ ] Hands-on lab completed.
- [ ] Evidence committed and linked.
- [ ] Troubleshooting notes recorded.
- [ ] Next step and blockers documented.

This is a personal learning workspace. Experimental cloud resources are not production-ready reference architectures without separate security, reliability and cost review.
