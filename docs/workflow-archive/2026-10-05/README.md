# Archived workflows

These definitions were moved byte-for-byte out of `.github/workflows`. GitHub will no longer discover them on the default branch after this PR is merged.

| File | Decision |
| --- | --- |
| skills-index.yml | Upstream-only scheduled index build |
| skills-index-freshness.yml | Upstream-only scheduled freshness probe |
| live-providers.yml | Upstream-only scheduled live API canaries |
| deploy-site.yml | Upstream docs deployment infrastructure; release/manual hook requires separate ownership review |
| docker.yml | Upstream-only image publication targeting nousresearch/hermes-agent |
| e2e-desktop.yml | Intentionally disabled flaky desktop suite; deterministic desktop core suite retained |

The installer suite remains manual and release-tag driven. Weekly OSV remains scheduled. CI retains affected-area routing, platform tests, core desktop E2E, and supply-chain checks.

Restore a workflow through a separate branch and PR only after reviewing repository ownership, endpoints, credentials, permissions, triggers, and cost. Restore any required caller explicitly. Archived files are historical evidence, not executable configuration.

See root `review.log` for scope, run evidence, decisions, and unresolved verification.
