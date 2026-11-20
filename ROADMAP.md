# 52-Week Roadmap

**Target:** Platform Engineer with practical GCP, Terraform, Docker, Kubernetes, GitOps, SRE and an initial Agentic DevOps implementation.

**Capacity:** 4 hours/week, approximately 208 hours total. The timeline is paced intentionally; move a week forward rather than skipping understanding.

## Learning strategy
1. Learn only the Linux/networking depth needed to operate systems.
2. Containerize a familiar Ruby on Rails application.
3. Learn GCP through practical deployments, starting with managed services.
4. Rebuild selected infrastructure with Terraform.
5. Learn Kubernetes locally before GKE.
6. Turn deployment practices into a repeatable developer platform.
7. Add observability, reliability and cost controls.
8. Introduce AI agents after operational tools and workflows exist.

Ruby remains the default language for application and agent integration. Python is not a prerequisite for the core roadmap.

## Weekly cadence
- Tuesday: 1 hour — documentation and focused theory.
- Thursday: 1 hour — small experiment.
- Saturday: 2 hours — implementation, troubleshooting and evidence.
- Monday and Wednesday: no scheduled study.

## Phase 1 — Infrastructure Fundamentals (Weeks 1–4)
**Outcome:** inspect Linux environments and diagnose basic service/network issues.

| Week | Focus | Deliverable |
|---|---|---|
| 1 | Processes, filesystem, permissions, resource usage | Linux investigation report using ps, top, df, du, free and lsof |
| 2 | SSH, DNS, TCP/IP, HTTP/HTTPS | Network troubleshooting report using ssh, dig, curl and ss |
| 3 | Bash, pipes, exit codes, environment variables | Safe environment diagnostic script |
| 4 | Git workflow and incident troubleshooting | Reproducible troubleshooting report |

Exit criteria: explain DNS-to-HTTP request flow; inspect processes, ports and resource pressure; diagnose a simple connectivity failure; write a safe Bash script.

## Phase 2 — Docker Engineering (Weeks 5–9)
**Outcome:** reproducible local environment for the Rails reference application.

| Week | Focus | Deliverable |
|---|---|---|
| 5 | Docker Engine, images, containers, registries | Run, inspect and debug containers |
| 6 | Dockerfile, layers, multi-stage builds, cache | Multi-stage Rails Dockerfile |
| 7 | Networks and volumes | Rails + PostgreSQL + Redis networking and persistence |
| 8 | Compose, health checks, configuration | Complete Compose development environment |
| 9 | Image hardening, non-root runtime, scanning | Optimized image and Trivy report |

Exit criteria: build from clean checkout; run app and dependencies with Compose; persist database data; configure health checks; document image scan findings.

## Phase 3 — Google Cloud Engineering (Weeks 10–18)
**Outcome:** deploy the Rails reference application using GCP managed services.

| Week | Focus | Deliverable |
|---|---|---|
| 10 | Projects, billing, IAM, service accounts | Project setup and least-privilege access notes |
| 11 | Artifact Registry and Cloud Storage | Publish container image and store a non-sensitive artifact |
| 12 | VPC, subnets, firewall, DNS | Network diagram and connectivity lab |
| 13 | Compute Engine | Small secured VM and teardown record |
| 14 | Cloud Run | Deploy Rails container |
| 15 | Cloud SQL | Secure Rails-to-PostgreSQL connection |
| 16 | HTTPS and load balancing | Request-routing and TLS notes |
| 17 | Cloud Logging and Monitoring | Dashboard and actionable alert |
| 18 | IAM/security and architecture review | Architecture decision record and checklist |

Exit criteria: explain project/IAM/network boundaries; deploy Rails; connect to managed PostgreSQL without committed secrets; inspect logs/metrics; tear down paid resources.

## Phase 4 — Terraform and Infrastructure as Code (Weeks 19–24)
**Outcome:** reproducibly provision selected GCP resources.

| Week | Focus | Deliverable |
|---|---|---|
| 19 | HCL, providers, resources, data sources | Terraform-managed GCP resource |
| 20 | Variables, outputs, locals | Parameterized dev configuration |
| 21 | Modules and composition | Reusable networking and application modules |
| 22 | Remote state in GCS and state security | Remote backend and recovery notes |
| 23 | Lifecycle, import and drift | Controlled drift investigation |
| 24 | fmt, validate, tests and security scanning | Terraform CI validation workflow |

Exit criteria: provision/destroy a lab environment; explain state and dependencies; use modules; review plans before apply; run validation and security checks. Never commit state or credentials.

## Phase 5 — Kubernetes and GKE (Weeks 25–34)
**Outcome:** deploy, expose, configure, scale and troubleshoot Rails on Kubernetes.

| Week | Focus | Deliverable |
|---|---|---|
| 25 | Architecture, kind and kubectl | Local cluster and architecture notes |
| 26 | Pods, Deployments, ReplicaSets | Rails Deployment |
| 27 | Services, Ingress and Gateway concepts | Reachable app service |
| 28 | ConfigMaps and Secrets | Safe externalized configuration |
| 29 | Requests, limits and probes | Resource and health configuration |
| 30 | Volumes, PVCs, StatefulSets concepts | Persistence lab and trade-off notes |
| 31 | RBAC and NetworkPolicies | Least-privilege access lab |
| 32 | Helm | Reusable Rails chart |
| 33 | GKE and Workload Identity | Short-lived GKE deployment |
| 34 | HPA, scheduling and troubleshooting | Diagnose Pending, CrashLoopBackOff and OOMKilled |

Exit criteria: deploy from manifests and Helm; troubleshoot common pod failures; configure resource requests/limits and probes; provision and tear down GKE safely.

## Phase 6 — CI/CD, GitOps and Platform Engineering (Weeks 35–41)
**Outcome:** create a repeatable developer workflow and first Golden Path.

| Week | Focus | Deliverable |
|---|---|---|
| 35 | GitHub Actions | Rails test/lint CI workflow |
| 36 | Container build and Artifact Registry | Secure image build/publish pipeline |
| 37 | Argo CD | GitOps deployment to lab cluster |
| 38 | Helm and promotion | Declarative dev/staging configuration |
| 39 | Developer experience | Rails service template and onboarding checklist |
| 40 | SRE: SLIs, SLOs, error budgets | Initial service SLO and measurement plan |
| 41 | Platform product thinking | Documented self-service Golden Path |

Exit criteria: new Rails service follows documented build/publish/deploy steps; desired deployment state is in Git; workflow documents defaults and escape hatches.

## Phase 7 — Observability, SRE and FinOps (Weeks 42–46)
**Outcome:** operate the platform with actionable telemetry and cost awareness.

| Week | Focus | Deliverable |
|---|---|---|
| 42 | Prometheus and Grafana | Application/cluster dashboard |
| 43 | OpenTelemetry | Rails traces and service metrics |
| 44 | Logs, metrics and traces | Correlated troubleshooting exercise |
| 45 | Alerting, SLO and incident response | Alert rules, runbook and postmortem |
| 46 | FinOps and capacity | Cost review and optimization recommendations |

Exit criteria: explain telemetry signals; correlate request traces/logs; define an SLI/SLO; write actionable runbook; identify cost drivers and clean unused resources.

## Phase 8 — Agentic DevOps (Weeks 47–52)
**Outcome:** build a safe MVP agent that investigates operational context through explicitly scoped tools.

| Week | Focus | Deliverable |
|---|---|---|
| 47 | LLMs, structured output and tool calling | Ruby service with validated structured response |
| 48 | Agent loop, MCP and tool contracts | Read-only operational tool interface |
| 49 | Infrastructure Agent | Terraform configuration/plan analysis with evidence |
| 50 | Observability Agent | Alert, log and metric context summary |
| 51 | Workflow orchestration and audit | Multi-step investigation with persisted history |
| 52 | Evaluation, guardrails and human approval | Agentic DevOps MVP and threat model |

Exit criteria: explicit tools only; read-only by default; validated inputs; evidence-linked results; secrets redacted; human approval for consequential actions; execution audit and evaluation cases.

## Cross-cutting practices
- Security: least privilege, secret management, scanning and workload identity.
- Reliability: health checks, resource limits, SLOs, rollback and incident notes.
- Cost: budgets/alerts, local-first labs, short-lived clusters and teardown.
- Documentation: architecture diagrams, ADRs and runbooks.
- Quality: tests, linting, static analysis and reviewable changes.

## Deferred topics
AWS hands-on specialization, Terragrunt, Crossplane, service mesh, Backstage implementation, complex multi-agent frameworks and autonomous production remediation are follow-up topics, not prerequisites for this 52-week plan.

## Completion standard
Demonstrate a Rails delivery path on GCP/GKE, Terraform-managed infrastructure, GitOps deployment, observable service health, a documented Golden Path and an auditable read-only-first Agentic DevOps MVP.
