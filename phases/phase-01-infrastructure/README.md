# Phase 1 — Infrastructure Fundamentals

**Weeks:** 1–4 · **Budget:** 16 hours

## Week 1 — Linux processes, filesystem and permissions
- Learn process tree, signals, users/groups, permissions, filesystem capacity and memory.
- Lab: inspect a running service, identify its process and listening ports, inspect resource usage.
- Commands: ps, top, free, df, du, find, lsof, chmod and chown.
- Evidence: labs/linux/week-01-linux-investigation.md.
- Acceptance: diagnose simulated high CPU or disk pressure and document safe next steps.

## Week 2 — SSH, DNS and network troubleshooting
- Learn practical IP/subnets, TCP handshake, ports, DNS, HTTP status and TLS basics.
- Lab: trace a request from hostname resolution to HTTP response; compare DNS failure, refused connection and timeout.
- Commands: ssh, dig, curl -v, ss, ping and traceroute where available.
- Evidence: labs/networking/week-02-network-diagnostics.md.
- Acceptance: distinguish name-resolution, routing/firewall, connection and application-layer failures.

## Week 3 — Bash automation
- Learn quoting, variables, exit codes, pipes, redirection, loops and safe failure handling.
- Lab: create a diagnostic script reporting disk, memory, key processes, listening ports and configurable HTTP health.
- Evidence: labs/bash/week-03-environment-diagnostics.sh and README.
- Acceptance: handle missing tools and failed checks, exit meaningfully and avoid printing secrets.

## Week 4 — Git and troubleshooting workflow
- Learn focused commits, branches, diffs, logs and incident notes.
- Lab: inject a local failure (wrong port, stopped service or invalid hostname), diagnose it and write an incident report.
- Evidence: labs/troubleshooting/week-04-incident-report.md.
- Acceptance: report symptom, impact, timeline, investigation, root cause, resolution and prevention.

## References
- [Linux man-pages](https://man7.org/linux/man-pages/)
- [curl documentation](https://curl.se/docs/)
- [Git documentation](https://git-scm.com/doc)

## Exit criteria
- [ ] Explain how a process, service and listening socket relate.
- [ ] Inspect filesystem and memory pressure.
- [ ] Diagnose basic DNS and HTTP connectivity failures.
- [ ] Write a safe Bash diagnostic script.
- [ ] Produce a reproducible troubleshooting report.
