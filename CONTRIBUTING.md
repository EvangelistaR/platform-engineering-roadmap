# How to Work in This Learning Repository

This repository is a curriculum and an engineering portfolio. Prefer small, reviewable changes.

## Naming
- Labs: labs/<topic>/<lab-name>/
- Phase notes: phases/phase-NN-<slug>/
- Architecture decisions: docs/adr/NNNN-<short-title>.md
- Runbooks: docs/runbooks/<service-or-scenario>.md

## Lab report structure
1. Goal — what capability is being practiced?
2. Prerequisites — tools, accounts and permissions.
3. Architecture — diagram or concise explanation.
4. Steps — reproducible commands/configuration.
5. Validation — how to prove it works.
6. Failure injection — what was deliberately broken and how it was diagnosed.
7. Security — permissions, secrets and exposure.
8. Cost and cleanup — resources created and exact teardown procedure.
9. Learnings — what changed in your mental model?

## Safety
- Never commit credentials, tokens, service-account keys, private keys, .env files, Terraform state or unredacted production data.
- Use dedicated lab projects and least-privilege identities.
- Review every Terraform plan before applying it.
- Avoid public exposure unless the lab explicitly requires it.
- Prefer local tools before paid cloud resources.
- Destroy temporary resources and verify cleanup.
- AI agents begin read-only. Write actions require validation, authorization and audit logging.

## Weekly workflow
1. Open or update the week's GitHub Issue.
2. Complete a focused theory block.
3. Run the lab and capture evidence.
4. Commit the artifact and update the weekly log.
5. Record blockers and the next experiment.
6. Close the issue only when acceptance criteria are met.
