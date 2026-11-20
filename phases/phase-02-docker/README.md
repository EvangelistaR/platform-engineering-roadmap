# Phase 2 — Docker Engineering

**Weeks:** 5–9 · **Budget:** 20 hours

## Weekly plan
| Week | Focus | Lab and evidence |
|---|---|---|
| 5 | Engine, images, containers, registries | Run, inspect and debug containers |
| 6 | Dockerfile, layers, multi-stage builds | Multi-stage Rails Dockerfile |
| 7 | Networks and volumes | Rails, PostgreSQL and Redis communicate; data persists |
| 8 | Compose, health checks and configuration | Compose development environment |
| 9 | Security and optimization | Non-root runtime where practical, smaller image, Trivy report |

## Exit criteria
- [ ] Build image from clean checkout.
- [ ] Run Rails, PostgreSQL and Redis locally with Compose.
- [ ] Persist database data using named volume.
- [ ] Configure health checks and environment variables safely.
- [ ] Explain image layers and multi-stage trade-offs.
- [ ] Scan image and document findings/remediation.

## References
- [Docker Get Started](https://docs.docker.com/get-started/)
- [Dockerfile reference](https://docs.docker.com/reference/dockerfile/)
- [Docker Compose](https://docs.docker.com/compose/)
- [Trivy](https://trivy.dev/)
