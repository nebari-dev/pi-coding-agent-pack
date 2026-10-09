# Security Policy

## Supported Versions

Security fixes are made on `main` and shipped in the next release. Only the most recent release receives fixes; older releases are not patched. If you can, please confirm the issue against the latest release or `main` before reporting.

## Reporting a Vulnerability

Please do not report security vulnerabilities through public GitHub issues, pull requests, or discussions.

Report them privately through GitHub's private vulnerability reporting: [open a new advisory](https://github.com/nebari-dev/pi-coding-agent-pack/security/advisories/new). Only the maintainers can see the report.

Please include as much of the following as you can:

- The version of this pack you are running, and where it is deployed
- Steps to reproduce, or a proof of concept
- The impact as you understand it, including what an attacker would need to exploit it

## What to Expect

The maintainers will acknowledge the report, work with you to confirm and understand the issue, and keep you updated on progress toward a fix. Once a fix is released, we will publish a GitHub Security Advisory and credit you unless you ask us not to.

Please give us a reasonable chance to release a fix before disclosing the issue publicly.

## Scope

In scope:

- The pack's Helm chart and its default values
- Code in this repository, including any services, operators, or UIs it builds
- How the pack integrates with Nebari, such as NebariApp routing, TLS, and Keycloak authentication

Out of scope here:

- Vulnerabilities in upstream Pi coding agent or JupyterHub, unless the issue is caused by how this pack configures or packages it; please report those to the upstream project
- Vulnerabilities in the Nebari platform itself; report those to [Nebari Infrastructure Core](https://github.com/nebari-dev/nebari-infrastructure-core/security/advisories/new) or [nebari-operator](https://github.com/nebari-dev/nebari-operator/security/advisories/new)
- Issues that require an attacker to already hold cluster-admin or cloud-account administrator credentials
