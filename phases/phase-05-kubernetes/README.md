# Phase 5 — Kubernetes and GKE

**Weeks:** 25–34 · **Budget:** 40 hours

## Weekly plan
| Week | Focus | Lab and evidence |
|---|---|---|
| 25 | Architecture, kind and kubectl | Local cluster and architecture notes |
| 26 | Pods, Deployments, ReplicaSets | Rails Deployment and rollout |
| 27 | Services, Ingress and Gateway concepts | Expose Rails service |
| 28 | ConfigMaps and Secrets | Safe externalized configuration |
| 29 | Requests, limits and probes | Resource and health configuration |
| 30 | Volumes, PVC and StatefulSet concepts | Persistence experiment and trade-offs |
| 31 | RBAC and NetworkPolicies | Least-privilege access lab |
| 32 | Helm | Reusable Rails chart |
| 33 | GKE and Workload Identity | Short-lived GKE deployment |
| 34 | HPA and troubleshooting | Diagnose Pending, CrashLoopBackOff and OOMKilled |

## Lab progression
1. Use kind for most exercises to control costs.
2. Keep manifests declarative and versioned.
3. Package the application with Helm.
4. Use GKE to validate managed-cluster and cloud-identity concepts.
5. Document exact cluster teardown steps.

## Exit criteria
- [ ] Deploy and update Rails workload.
- [ ] Expose it through a Service and suitable ingress mechanism.
- [ ] Configure settings and secrets without committing sensitive values.
- [ ] Configure requests, limits and probes.
- [ ] Explain RBAC and service-account identity.
- [ ] Troubleshoot common scheduling, image and memory failures.
- [ ] Create and delete a GKE lab cluster safely.

## References
- [Kubernetes Concepts](https://kubernetes.io/docs/concepts/)
- [Kubernetes Tutorials](https://kubernetes.io/docs/tutorials/)
- [kind](https://kind.sigs.k8s.io/)
- [Helm](https://helm.sh/docs/)
- [GKE](https://cloud.google.com/kubernetes-engine/docs)
