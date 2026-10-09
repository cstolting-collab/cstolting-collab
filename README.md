# Sherrie J — Estra Logics<svg xmlns="http://www.w3.org/2000/svg" width="1100" height="560" viewBox="0 0 1100 560" role="img" aria-labelledby="title desc">
<title id="title">CML Fermata collaboration allocation estimate</title>
<desc id="desc">Standing collaboration estimate: 35 percent human leadership and authority, 40 percent AI-assisted technical execution, and 25 percent CML/Fermata continuity and integrity method. These values are estimates, not measured productivity, time savings, ownership, or completion percentages.</desc>
<rect width="1100" height="560" rx="24" fill="#0d1117"/>
<text x="42" y="54" fill="#f0f6fc" font-family="Segoe UI, Arial, sans-serif" font-size="29" font-weight="700">How the work is divided</text>
<text x="42" y="83" fill="#8b949e" font-family="Segoe UI, Arial, sans-serif" font-size="15">Standing collaboration estimate · not measured time savings or ownership</text>

<g transform="translate(205 292)">
  <circle r="126" fill="#161b22"/>
  <path d="M0 0 L0 -112 A112 112 0 0 1 65.83 90.61 Z" fill="#a371f7"/>
  <path d="M0 0 L65.83 90.61 A112 112 0 0 1 -112 0 Z" fill="#3fb950"/>
  <path d="M0 0 L-112 0 A112 112 0 0 1 0 -112 Z" fill="#58a6ff"/>
  <circle r="61" fill="#0d1117"/>
  <text y="-4" fill="#f0f6fc" font-family="Segoe UI, Arial, sans-serif" font-size="17" font-weight="700" text-anchor="middle">CML / Fermata</text>
  <text y="22" fill="#8b949e" font-family="Segoe UI, Arial, sans-serif" font-size="13" text-anchor="middle">human-led</text>
</g>

<g transform="translate(400 132)">
  <rect width="650" height="100" rx="15" fill="#161b22" stroke="#a371f7"/>
  <circle cx="46" cy="50" r="12" fill="#a371f7"/>
  <text x="76" y="43" fill="#f0f6fc" font-family="Segoe UI, Arial, sans-serif" font-size="21" font-weight="700">40% · AI-assisted technical execution</text>
  <text x="76" y="70" fill="#8b949e" font-family="Segoe UI, Arial, sans-serif" font-size="14">Research, implementation help, comparison, drafting, test preparation.</text>
</g>
<g transform="translate(400 250)">
  <rect width="650" height="100" rx="15" fill="#161b22" stroke="#3fb950"/>
  <circle cx="46" cy="50" r="12" fill="#3fb950"/>
  <text x="76" y="43" fill="#f0f6fc" font-family="Segoe UI, Arial, sans-serif" font-size="21" font-weight="700">35% · Human leadership and authority</text>
  <text x="76" y="70" fill="#8b949e" font-family="Segoe UI, Arial, sans-serif" font-size="14">Problem choice, judgment, approvals, publication, scope, final claims.</text>
</g>
<g transform="translate(400 368)">
  <rect width="650" height="100" rx="15" fill="#161b22" stroke="#58a6ff"/>
  <circle cx="46" cy="50" r="12" fill="#58a6ff"/>
  <text x="76" y="43" fill="#f0f6fc" font-family="Segoe UI, Arial, sans-serif" font-size="21" font-weight="700">25% · CML / Fermata integrity method</text>
  <text x="76" y="70" fill="#8b949e" font-family="Segoe UI, Arial, sans-serif" font-size="14">Continuity, evidence boundaries, handoff state, validation, next actor.</text>
</g>
<text x="42" y="525" fill="#8b949e" font-family="Segoe UI, Arial, sans-serif" font-size="13">Estimate only. It does not measure human-time savings, productivity, authorship, ownership, or completion.</text>
</svg>

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
