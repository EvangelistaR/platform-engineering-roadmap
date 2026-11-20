# Phase 4 — Terraform and Infrastructure as Code

**Weeks:** 19–24 · **Budget:** 24 hours

## Weekly plan
| Week | Focus | Lab and evidence |
|---|---|---|
| 19 | HCL, provider, resource, data source | Provision a small GCP resource |
| 20 | Variables, outputs and locals | Parameterized dev configuration |
| 21 | Modules | Reusable networking and application modules |
| 22 | Remote state in GCS | Backend setup and recovery precautions |
| 23 | Lifecycle, import and drift | Controlled drift investigation |
| 24 | Validation, tests and security | CI workflow for fmt, validate, plan and scanning |

## Suggested structure
    terraform/
      modules/
        networking/
        cloud-run/
        cloud-sql/
        artifact-registry/
      environments/
        dev/
        staging/

## Safety
- Never commit tfstate, state backups, credentials or sensitive plan files.
- Restrict access to the GCS state bucket.
- Review terraform plan before every apply.
- Keep environments separate and document destructive changes.
- Start with Terraform alone; defer Terragrunt.

## Exit criteria
- [ ] Provision and destroy a lab environment using Terraform.
- [ ] Explain providers, resources, data sources and dependency graph.
- [ ] Build and consume reusable modules.
- [ ] Secure remote state.
- [ ] Detect and explain configuration drift.
- [ ] Run fmt, validate and security checks in CI.

## References
- [Terraform tutorials](https://developer.hashicorp.com/terraform/tutorials)
- [Google provider](https://registry.terraform.io/providers/hashicorp/google/latest/docs)
- [Terraform language](https://developer.hashicorp.com/terraform/language)
