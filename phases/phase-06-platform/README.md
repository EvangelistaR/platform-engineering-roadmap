# Phase 6 — CI/CD, GitOps and Platform Engineering

**Weeks:** 35–41 · **Budget:** 28 hours

## Weekly plan
| Week | Focus | Lab and evidence |
|---|---|---|
| 35 | GitHub Actions | Rails test/lint CI workflow |
| 36 | Container CI/CD | Build and publish image to Artifact Registry |
| 37 | Argo CD | GitOps deployment to lab cluster |
| 38 | Helm and promotion | Declarative dev/staging values |
| 39 | Developer experience | Rails service template and onboarding checklist |
| 40 | SRE fundamentals | Initial SLI/SLO and error-budget exercise |
| 41 | Golden Path | Documented self-service workflow |

## Target developer workflow
1. Developer creates a repository from a service template.
2. GitHub Actions runs tests and static checks.
3. Pipeline builds and scans the container image.
4. Image is published to Artifact Registry.
5. GitOps configuration is updated through a reviewable change.
6. Argo CD reconciles desired state.
7. Observability checks deployed service health.

## Exit criteria
- [ ] CI validates Rails changes.
- [ ] Image build/publish workflow is reproducible.
- [ ] GitOps desired state is versioned in Git.
- [ ] Deployment changes are reviewable and traceable.
- [ ] Golden Path documents defaults, security and escape hatches.
- [ ] SLI/SLO has a clear measurement and owner.

## References
- [GitHub Actions](https://docs.github.com/en/actions)
- [Argo CD](https://argo-cd.readthedocs.io/)
- [Platform Engineering](https://platformengineering.org/)
- [Google SRE Book](https://sre.google/sre-book/table-of-contents/)
