# Security Policy

## Reporting a Vulnerability

Please report security vulnerabilities to **security@verifiable-labs.com**.

Do not file public GitHub issues for security-sensitive reports.

We will acknowledge receipt within 72 hours and aim to provide a status
update within 7 days. Coordinated disclosure timelines are agreed
case-by-case.

## Scope

This policy covers the public Verifiable Labs repositories under the
[`verifiablelabs`](https://github.com/verifiablelabs) organisation,
including:

- [`verifiable-labs-envs`](https://github.com/verifiablelabs/verifiable-labs-envs) — SDK + 25 environments + hosted-calibration FastAPI service
- [`verifiable-labs-website`](https://github.com/verifiablelabs/verifiable-labs-website) — marketing site + dashboard
- The hosted endpoints at `api.verifiable-labs.com` and `verifiable-labs.com`

## Out of scope

- Findings against third-party dependencies — please report upstream
- Social-engineering reports against the maintainer
- DoS / rate-limit findings on the unauthenticated public API
  (already rate-limited at 30 req/min/IP — see SDK README)
