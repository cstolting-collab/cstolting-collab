# Sherrie Joseph — Estra Logics

**Continuity engineering for stateful AI and software systems.**

I develop and test **CML (Continuity Markup Language)**, a continuity and state-validation architecture for systems that need to preserve accepted state across multi-step execution, recovery, handoff, and external observation.

My work is human-led, AI-assisted, and evidence-bound. I separate implementation results, observed behavior, hypotheses, and unresolved questions rather than treating them as interchangeable.

## CML in one view

```text
canonical accepted state
        ↓
read-only projection
        ↓
candidate transition
        ↓
invariant / authorization validation
        ↓
explicit commit
```

External observation is handled separately:

```text
external observation
        ↓
noncanonical evidence
        ↓
PASS / FAIL / UNEVALUABLE
```

Evaluation does not mutate canonical state.

## What is implemented

Public CML work includes:

- declarative invariants and state locks
- authorized unlocks
- stale-projection rejection
- fail-closed transition handling
- provenance and checkpoint recovery
- append-only continuity evidence
- explicit separation of canonical state from observation
- reproducible validation and benchmark evidence

CML is **not presented as a theorem prover**, and I do not claim it invented formal verification. The goal is narrower: make continuity and state-transition behavior inspectable, reproducible, and reviewable in systems that carry state across time and actions.

## Start here

### [CML-Trust](https://github.com/cstolting-collab/CML-Trust)
Alpha-stage evidence and continuity validation tooling. It records external observations against compile-valid CML audit plans, preserves revocation history, derives status, and keeps observation separate from canonical state.

### [CML GitHub Work Record](https://github.com/cstolting-collab/CML-GitHub-Work-Record)
Public, evidence-bound record of engineering work, validation standards, experiments, failures, and handoffs.

### [Agent Boundary Check](https://github.com/cstolting-collab/agent-boundary-check)
Synthetic-canary tooling for verifying what AI coding agents can actually read, write, execute, and reach.

### [Pattern Atlas](https://github.com/cstolting-collab/pattern-atlas)
Local-first evidence timeline and relationship mapping.

## Engineering standard

A result is not treated as established because a test passed once.

For performance and reliability work I preserve:

- exact source and environment identity
- control and treatment separation
- correctness parity
- repeated measurements
- median and worst-case reporting
- explicit HOLD states when evidence is incomplete
- reviewable handoffs with unresolved conditions preserved

Failures and superseded experiments are retained because they are useful evidence.

## Collaboration

I am interested in technical review and collaboration around:

- long-horizon and stateful agents
- agent evaluation and oversight
- state-transition validation
- checkpoint and recovery integrity
- provenance and reproducibility
- human authority in AI-assisted workflows

For public repositories, I work only on code I am authorized to inspect and modify.

## Current boundary

Public repositories expose reproducible ideas, evidence, and engineering outcomes. Private research workflows and unpublished implementation details remain private.

---

**Estra Logics**  
Continuity · State · Evidence · Human authority
