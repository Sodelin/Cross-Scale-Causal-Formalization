# The 85-declaration baseline and its relation to the omnibus

Assessed 30 September 2026 UTC. Read-only GitHub review by the `baseline_85` agent; no new Lean work or public mutation in this review. Repository main was pinned at [`346c558e7a29646a63dd77b60707697fc6bc9768`](https://github.com/Sodelin/Formalizing-Soft-Sciences/tree/346c558e7a29646a63dd77b60707697fc6bc9768).

## What the 85 means

The integrated inventory contains 85 **theorem declarations**, not 85 independent discoveries. The JSON audit's exact composition is:

| Family | Declarations |
| --- | ---: |
| Solidarity | 16 |
| Identifiability | 9 |
| Measurement | 9 |
| Causality | 6 |
| Learning | 9 |
| CollectiveAction | 10 |
| Aggregation | 8 |
| PublishedCBT | 14 |
| SourceBridge | 4 |
| Total | 85 |

Thus the remembered 67-item core is 16 solidarity + 51 foundations, and the clinical extension adds 18. The historical Mathematics of Psychology solidarity copy is already included. The audit labels 21 supporting declarations, 20 endpoints, 17 consequences, 15 witnesses, 10 integrity checks and 2 explicit reuses. These role labels describe the development; they do not score novelty. Source: [complete machine-readable audit](https://github.com/Sodelin/Formalizing-Soft-Sciences/blob/346c558e7a29646a63dd77b60707697fc6bc9768/research/publication-audit-2026-09-29/theorem-audit.json), audited source snapshot `7835157627548823f03f29dd3987e55601807b55`.

All nine files containing the 85 declarations have identical Git blob hashes in the audited source snapshot and this reviewed main. The count is current for those preserved proof bytes. No claim is made about an unknown distinct older corpus.

## Verification evidence and the new documentation failure

The historical integrated [workflow run 36634412999](https://github.com/Sodelin/Formalizing-Soft-Sciences/actions/runs/36634412999), on audited source `7835157`, is independently confirmed by the GitHub Actions API as completed/success. The [67-declaration receipt](https://github.com/Sodelin/Formalizing-Soft-Sciences/blob/346c558e7a29646a63dd77b60707697fc6bc9768/projects/foundations/verification.md) records Lean 4.19.0, all declaration axiom reports, and source hashes. The workflow additionally checks pinned MATLAB source transcription and the clinical build/audit.

However, the latest [run 36688407438](https://github.com/Sodelin/Formalizing-Soft-Sciences/actions/runs/36688407438) at reviewed main is **failed**. Its job and decoded log show:

- The 67-declaration source build and axiom audit succeeded.
- `scripts/check_foundations.py` failed at line 85 on `psychology/README.md`'s `../clinical` link: this validator requires local targets to be files, and `clinical` is a directory.
- The subsequent clinical verification step was skipped, so this run does not constitute a fresh 85-declaration check.

This failure was introduced by the documentation navigation update, rather than a changed theorem or invalid proof. A tree-based scan of all 11 Markdown files checked by the foundations script found this sole local-target/type failure and no table-width mismatch. Root applied the minimal repair at [`8e665d2a9f6168e6448b2ca49fccbec87d57d3ad`](https://github.com/Sodelin/Formalizing-Soft-Sciences/commit/8e665d2a9f6168e6448b2ca49fccbec87d57d3ad): `[clinical package](../clinical)` became `[clinical observation module](../clinical/ClinicalModels/PublishedCBT.lean)`. The validator, proof manifests and Lean sources were retained.

The normal push-triggered [replacement run 36691100776](https://github.com/Sodelin/Formalizing-Soft-Sciences/actions/runs/36691100776) is confirmed completed/success by fresh API read. Its job confirms success for the 67-declaration source/build audit, research documentation/provenance checks, and the published CBT source-fragment verification. Therefore there is now fresh integrated verification on the repaired documentation head, in addition to the preserved historical proof-byte receipt. No manual rerun was needed.

## What can actually be reused

The valuable baseline is a small verified toolkit plus explicit examples, source mappings and reproducibility. It should stay preserved and be reused where its assumptions match a substantive target. The closest connections are:

| Existing component | Omnibus targets or theory it informs | Essential missing work |
| --- | --- | --- |
| Identifiability: exact observation equivalence, design inclusion, postprocessing information loss | BIO-1/2 observation access; BIO-4/5; PSY-1/3; SOC-01/05; shadow theory | Target-specific prediction maps and lawful model classes; stochastic/noisy identification, sharp uncertainty, design cost and discovery coverage |
| Measurement: additive intercept invariance and bounded-bias ordering | PSY-1/4; SOC-02; construct operationalization | Actual symptom/confidence measurement laws, cohort data or jointly dependent bias mechanisms; construct validity does not follow from algebra |
| Causality: standard binary observational collision and intervention disagreement | BIO-4/5; PSY-1; SOC-01/02/05 | Domain-specific dynamics, intervention semantics, causal transport assumptions or interference; generic collision is not a new source-specific answer |
| Learning: exact consistency, correct/incorrect labels, rival elimination, duplication | Discovery-aware elicitation; PSY-3/4; broadly the omnibus evidence interface | A justified generator that finds relevant questions, noisy-answer rules, adaptive cost bounds and longitudinal learning mechanisms |
| CollectiveAction: task coverage, participation constraints and unrestricted two-person budget | SOC-03/05 | Exchange networks, structural power indices, matching/outside-option bargaining, recognition/congestion dynamics |
| Aggregation: checked Simpson witness and reuse of information loss | BIO-5; SOC-02/05; scale interfaces | Actual cell mixing or social selection/interference semantics, sharp jointly attainable identified regions |
| Published CBT fragment and source bridges | PSY-2; action-dependent observation within shadow theory | Belief inference, policy selection, stochastic learning, uncertainty tolerance, partial approach and context generalization |

The clinical package proves a useful source-specific fact: avoidance's complete declared four-step observation record cannot classify both safe and dangerous states correctly, while the fixed approach record distinguishes those two states. It also checks mass/bounds/equality properties and selected upstream tables. The authors already discussed avoidance's information-loss mechanism. Our contribution here is formal verification and bounded transcription, not empirical treatment efficacy or closure of their future-model agenda. [Exact source map](https://github.com/Sodelin/Formalizing-Soft-Sciences/blob/346c558e7a29646a63dd77b60707697fc6bc9768/PUBLICATION-COVERAGE-2026-09-29.md).

BIO-3's finite-population inheritance target has no substantive implementation in this soft-science corpus; its relevant baseline resides in Samuel Alexander research. Shared identification reasoning is not a substitute for the population transition model.

## A subtle limitation already visible in the baseline

`SocialScience.Identifiability.Identified` currently demands recovery of the **entire parameter**: observational equivalence implies `θ = φ`. Some omnibus tasks require only the desired response or ranking `q(θ) = q(φ)`. Full model recovery can be unnecessarily expensive or impossible even when that response is identified. A future domain interface can reuse the equivalence machinery while expressing response identification. That mathematical extension is not automatically novel; it should be implemented only when required by an admitted source-specific task.

Likewise, `distinguishing_query_eliminates_rival` assumes the distinguishing input and correct label are supplied. It does not prove that an assistant discovers the input, knows the correct label, or chooses the best next target. This is exactly where Nolan's criticism remains outside the baseline.

## Continuation and routable external-chat packets

Preserve this corpus as a pinned reusable baseline. Select extensions by a consequential unresolved source question, and first ask whether the existing proof mechanism already supports broader quantifiers or weaker assumptions. Do not extend every module simply because it can be extended. Do not require rebuilding known foundations when the missing step is a domain mapping, measurement or algorithm.

A compact handoff should carry: (1) question ID and original source/locator; (2) strongest useful target and its explicit scope dimensions; (3) pinned baseline modules/results; (4) what is proved versus proposed; (5) exact missing semantic or mathematical bridge; (6) prior results and restrictions to challenge before implementation; (7) assigned owned files/dependencies and reproducible evidence requirements; (8) canonical discussion/checkpoint path and stopping or escalation conditions. A copied packet makes an external chat routable; it does not imply live agent-to-agent delivery or access to another chat's private context.

Making the lesson reliably available means putting it in the task entry point and requiring fresh hydration of that context. GitHub persistence does not alter model weights or guarantee unprompted recall. The process should explicitly load the all-levels lesson and the strongest target before execution, with actual source/content evidence in the packet rather than relying on declaration counts or remembered slogans.
