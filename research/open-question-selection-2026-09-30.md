# Scope correction and open-question selection
Date: 2026-09-30. Motivating hypothesis and research priorities: Nolan Downard.

## What changed
Nolan clarified that the research objective is to answer an unresolved question. Familiar mathematical facts should be imported as prior work, not independently reproduced and presented as the research result. Formalization is warranted when it contributes to the selected unresolved question, repairs a consequential gap, or provides a reusable dependency unavailable in an adequate form.

## Classification of the previous packet
The decision-sufficiency criterion, deterministic regret formula, free-information refinement fact and XOR counterexample are classical elementary supporting results. Their proofs and exact checks are valid within the stated models, but no open problem was answered and no novel theorem was established. The compute spent reproducing them was not justified by a demonstrated dependency on an open target. The earlier packet is preserved under research/prior-work/decision-sufficiency/ for provenance and reuse; it should not be counted as new research output.

Original publication: https://github.com/Sodelin/Formalizing-Soft-Sciences/tree/main/research/new-wave-2026-09-30/decision-sufficiency

## Relevant prior work to use, rather than rebuild
- Ye, Amin & Özdağlar, Learning Decision-Sufficient Representations for Linear Optimization, arXiv:2603.18551v2, 22 May 2026. https://arxiv.org/html/2603.18551v2 . Supplies computational and learning results beyond the elementary finite observation criterion.
- Zhang, Luo & Baltieri, Compositional Behavioral Semantics for State Abstraction in Reinforcement Learning, ICML 2026. https://proceedings.mlr.press/v306/zhang26dy.html . Supplies a framework for behavioral transfer under abstraction.
- Sezener & Dayan (2020), Static and Dynamic Values of Computation in MCTS. https://proceedings.mlr.press/v124/sezener20a.html . Prior work on value of computations beyond immediate steps.
- The existing repository note research/partial-views-and-changing-systems.md supplies neighboring causal-identification literature and the upstream changing-lens problem. This correction does not equate these different models.

## Source-backed open direction
Section 8 of Ye et al. v2 explicitly leaves extension to noisy observations and characterization of sample complexity open. It also lists persistence of hardness under nondegeneracy and extensions beyond linear optimization.

This is an open direction in the cited version, not a certification that no later publication has solved any special case. Targeted searches on 30 September 2026 did not establish such a resolution; they are not exhaustive.

## Candidate target, not a result
For a known bounded linear-program feasible region, unknown costs drawn from a specified distribution, and noisy linear measurements, determine when a representation learned from samples yields a near-optimal decision on a fresh cost instance. Seek matching upper/lower sample or measurement bounds in a precisely stated regime, accounting for a decision-boundary margin and observation noise.

Before spending proof or coding compute:
1. Check the final COLT paper and subsequent work for the exact unresolved regime.
2. Extract the existing noiseless algorithms and assumptions; reuse them.
3. Choose noise, query restrictions, error metric, confidence level and margin assumptions explicitly.
4. Identify which proposed conclusion is absent from the nearest existing theorem.
5. Attempt that gap; move to Lean only when it verifies a consequential new argument or indispensable existing dependency.

A generic perturbation bound, toy simulation or restatement of sufficiency would not answer this target. Unknown/evolving observation maps are an additional problem, not a free extension of known noisy measurements.

## Participation and handoff
Chat researchers can contribute source comparisons, candidate theorem statements, counterexamples and proof arguments in ordinary Markdown. Tool researchers execute literature retrieval, experiments and verification as needed. Record intellectual contribution separately from execution. No contribution requires tool access to be considered.

## Status
No open problem solved in this correction. No additional theorem reproduction, Lean development or model-performance experiment undertaken. This note redirects future work and preserves prior artifacts in the repository Nolan designated.
