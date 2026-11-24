# vac-dev-team

We build `vac`, a research prototype of a containment controller for AI agents.

Bring an agent, a sandbox or any program. `vac` wraps it and decides every action it tries to take: whether the policy grants it, whether the current mode allows it, and whether any allowance is left. Authority is removed when a lease is not renewed, when a hard rule fires, or when enforcement cannot be confirmed. Automatic signals can only tighten. Only the operator gives authority back.

At the centre is a small decision kernel with machine-checked proofs. Everything around it is tested, and each claim we make names the evidence behind it and what would disprove it.

## Status

Research prototype. Run it only on a disposable Linux or WSL2 machine.

## Repositories

- [verified-agent-containment](https://github.com/vac-dev-team/verified-agent-containment): the kernel, the controller, the proofs and the test lab.

## Reporting a security problem

See the [security policy](https://github.com/vac-dev-team/.github/blob/main/SECURITY.md). Please do not open a public issue for a vulnerability.
