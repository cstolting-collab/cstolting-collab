# Active External Work Log

> Public, evidence-bound status ledger for selected external contributions.
>
> **PLEASE VALIDATE ALL GITHUB WORKFLOW.**

This log covers only these active pull requests:

- [microsoft/fhir-server#5829](https://github.com/microsoft/fhir-server/pull/5829)
- [openai/openai-go#932](https://github.com/openai/openai-go/pull/932)
- [openai/openai-go#933](https://github.com/openai/openai-go/pull/933)

It does **not** monitor personal GitHub activity. An open PR, local test, completed workflow, approval, merge, release, and production behavior are separate evidence states.

## Automatic publication boundary

Sherrie Joseph authorized this bounded release lane on 2026-09-18.

A scheduled workflow may read the three PRs above and update this public ledger with factual status. It may not push to the upstream projects, change upstream code, comment, request approval, rerun CI, merge, close, or represent a held gate as a success.

**Human-led. AI-assisted. Evidence-bound.** CML/Fermata is the human-authored integrity method used to preserve scope, evidence, and claim boundaries; it is not a separate author.

---

## 2026-09-18 — Monitoring baseline

**Overall: HOLD.** All three PRs are open and mergeable. No GitHub workflow is currently reported as failed or cancelled. Every observed GitHub Actions run is completed with `action_required`; that is an upstream verification/authorization hold, not a passing CI result.

| PR | Scope | Test evidence | CI gate | Review | Mergeability | Published state |
| --- | --- | --- | --- | --- | --- | --- |
| [#5829](https://github.com/microsoft/fhir-server/pull/5829) | FHIR Server diagnostic-suppression repair for [issue #5679](https://github.com/microsoft/fhir-server/issues/5679) | **OBSERVED:** PR records a Release rebuild with 0 warnings/0 errors; focused test groups are recorded. | **HOLD:** `Code Scanning - Action` is `action_required`. | No submitted reviews or unresolved review threads observed. | `true` | Open, unmerged. |
| [#932](https://github.com/openai/openai-go/pull/932) | Preserve manual Responses history. | **PARTIAL / OBSERVED:** targeted Go test and vet evidence is recorded; mock endpoint suite was not run after a dependency-fetch problem. | **HOLD:** CI, CodeQL, and Castiron runs are `action_required`. | No submitted reviews or unresolved review threads observed. | `true` | Open, unmerged. |
| [#933](https://github.com/openai/openai-go/pull/933) | Describe non-API HTTP errors accurately. | **PARTIAL / OBSERVED:** focused Go test, vet, compile, Castiron, and diff-check evidence is recorded; a full `go test ./...` pass is not claimed. | **HOLD:** CI, CodeQL, and Castiron runs are `action_required`. | No submitted reviews or unresolved review threads observed. | `true` | Open, unmerged. |

### Current gates

1. **Scope:** bounded to the three linked PRs.
2. **Evidence and tests:** published PR evidence is recorded above; historical local tests were not independently rerun for this journal entry.
3. **Permissions:** upstream GitHub Actions require maintainer/authorized-runner action.
4. **CI gates:** no pass is claimed while the visible runs remain `action_required`.
5. **Published state:** each PR is public, open, unmerged, and mergeable at this baseline.

A future entry will record only material changes, failures, reviewer direction, verified CI results, merges, or closures. Nothing is called complete until scope, evidence, tests, permissions, CI gates, and published state are independently verified.
