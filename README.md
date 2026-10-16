# krx-stock-runner

Public execution configuration only. Application source, stock inputs, generated reports, and research account files remain in a separate private repository.

- Manual dispatch only; no push or pull-request execution.
- Standard GitHub-hosted Linux runner, with a 25-minute job limit.
- `PRIVATE_REPO_TOKEN` and `KRX_AUTH_KEY` are registered as GitHub Actions Secrets; never commit credentials.
- Checkout does not persist credentials. No artifacts or reports are uploaded here.
- Job logs are public and contain execution summaries. Do not add private data to logs.
- `verify-free-runner.yml` checks runner availability without credentials.

This repository alone does not activate the external daily schedule. Keep the existing private report reader and its integrity checks.
