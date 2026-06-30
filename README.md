# runx ci-failure-triage skill

Public package for the `ci-failure-triage` runx skill.

The skill classifies a bounded CI failure snapshot as `real-break`, `dep`,
`infra`, `flake`, or `needs_agent`. It emits a read-only
`runx.ci.triage.v1` packet for a downstream issue-intake, issue-to-pr, or
pr-review-note run. It never opens issues, reruns CI, pages operators, or mints
authority.

## Verification

```bash
npm --prefix skills/ci-failure-triage test

RUNX_RECEIPT_SIGN_KID=runx-demo-key \
RUNX_RECEIPT_SIGN_ED25519_SEED_BASE64=QkJCQkJCQkJCQkJCQkJCQkJCQkJCQkJCQkJCQkJCQkI= \
RUNX_RECEIPT_SIGN_ISSUER_TYPE=hosted \
npx @runxhq/cli@0.6.14 harness ./skills/ci-failure-triage --json
```

The GitHub Actions workflow records unit-test, harness, and optional published
dogfood evidence.

