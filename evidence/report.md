# ci-failure-triage delivery report

Package: `jaasieldelgado131/ci-failure-triage@sha-6fe47c6cfe1a`

Public registry URL: https://runx.ai/x/jaasieldelgado131/ci-failure-triage@sha-6fe47c6cfe1a

Source revision: https://github.com/jaasieldelgado131/runx-ci-failure-triage-skill/tree/6fe47c6cfe1a8ef96faae81b192aa5fecbe0472e

Workflow evidence: https://github.com/jaasieldelgado131/runx-ci-failure-triage-skill/actions/runs/28479995607

## Summary

- The package name is exactly `ci-failure-triage`.
- The published registry ref is `jaasieldelgado131/ci-failure-triage@sha-6fe47c6cfe1a`.
- The run used `runx-cli 0.6.14`.
- The hosted registry read succeeded against `https://api.runx.ai`.
- The Linux workflow completed successfully.
- The inline harness passed with 2 cases and 0 assertion errors.
- The harness case `real_break_clear_logs` sealed successfully.
- The harness case `ambiguous_truncated_logs` stopped with `needs_agent`.
- The dogfood run sealed with receipt `runx:receipt:sha256:24e063546d5aa81c00b4177f6c442dc2dcbb6bc891cb0ece8aa738495b1c8aaa`.
- The receipt verification returned `valid: true` with no findings.

## Dogfood result

The post-publish dogfood run used the published registry package and completed graph `ci-failure-triage` with status `Succeeded`.

Classification output:

- `verdict`: `real-break`
- `confidence`: `0.95`
- `recommended_lane`: `issue-to-pr`
- `rationale`: `clear code/test failure visible in logs`
- `evidence_refs`: `log:1`, `log:2`, `log:3`, `log:4`, `log:5`

Policy checks:

- No tracking item was opened.
- No CI rerun was executed.
- No operator was paged.
- No authority was minted.
- The output is a read-only draft routing packet for downstream governed lanes.

## Evidence files

- `evidence.json` summarizes the package, registry read, harness, dogfood result, and acceptance mapping.
- `verification.json` contains the receipt verification verdict for the dogfood receipt.
