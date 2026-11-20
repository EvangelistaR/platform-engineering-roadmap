# Phase 8 — Agentic DevOps

**Weeks:** 47–52 · **Budget:** 24 hours

## Goal
Build a small, auditable agentic workflow that investigates operational context through explicitly scoped tools. This is an MVP, not production autonomy.

## Ruby-first implementation
Use Ruby for the first agent service and operational integrations where libraries/APIs support the requirement. Keep Python out of the critical path. Introduce a small Python component only if a selected framework or evaluation tool offers a compelling capability that cannot reasonably be accessed from Ruby.

## Weekly plan
| Week | Focus | Lab and evidence |
|---|---|---|
| 47 | LLMs, structured output and tool calling | Ruby service with validated structured response |
| 48 | Agent loop, MCP and tool contracts | Read-only operational tool interface |
| 49 | Infrastructure Agent | Terraform configuration/plan analysis with evidence |
| 50 | Observability Agent | Alert, log and metric context summary |
| 51 | Workflow orchestration and audit | Multi-step investigation with persisted history |
| 52 | Evaluation, guardrails and approval | MVP demo and threat model |

## Suggested architecture
- Rails API/control plane.
- Replaceable LLM provider adapter.
- Explicit read-only tools for Terraform plans, Kubernetes status and observability data.
- PostgreSQL for investigation history and audit records.
- Background jobs only if asynchronous execution is needed.
- MCP server when interoperability with external agent clients is useful.

## Safety model
1. Start with read-only tools.
2. Validate tool arguments against schemas.
3. Apply least-privilege identities outside the model.
4. Treat retrieved logs/configuration as untrusted data, not instructions.
5. Redact secrets before sending context to a model.
6. Require human approval for consequential changes, especially production.
7. Log actor, tool, redacted arguments, result, timestamps and approval.
8. Evaluate prompt injection, incorrect diagnosis and unsafe tool requests.

## Exit criteria
- [ ] Explain tool calling and the agent execution loop.
- [ ] Invoke an operational read-only tool from Ruby.
- [ ] Produce evidence-linked infrastructure or observability analysis.
- [ ] Persist an auditable investigation record.
- [ ] Demonstrate denial of unauthorized/destructive action.
- [ ] Evaluate representative success and failure cases.
- [ ] Document limitations and next iteration.

## References
- [Model Context Protocol](https://modelcontextprotocol.io/docs/)
- [Google Agent Development Kit](https://google.github.io/adk-docs/) — Python-oriented; evaluate as an option, not the default for this Ruby-first plan.
- [OpenTelemetry](https://opentelemetry.io/docs/)
