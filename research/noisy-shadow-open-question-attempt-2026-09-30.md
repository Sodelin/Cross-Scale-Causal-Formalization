# Noisy-shadow open question: literature audit and one-pass attempt

Date: 2026-09-30. Research motivation and priority: Nolan Downard.
Mode: rapid evidence map and bounded mathematical attempt, not systematic review.
Outcome: genuine author-stated open direction confirmed; no defensible new solution established; no Lean-checked or publication-ready result.

## 0. What is genuinely open?
The final COLT 2026 paper by Ye, Amin and Özdağlar, **Learning Decision-Sufficient Representations for Linear Optimization**, Section 7, pp.12–13, explicitly lists noisy-query extensions and sample complexity, along with robust cost-distribution corruption, as open directions. These are research directions, not named conjectures with a single predeclared proposition.

Final source: https://proceedings.mlr.press/v336/ye26a.html
Final PDF: https://raw.githubusercontent.com/mlresearch/v336/main/assets/ye26a/ye26a.pdf
Downloaded PDF SHA256: 2a465c024498b4dd4028257535a5c869e9f6bf1630f216a9567c82654aa67062
The final version differs materially from arXiv v2: it adds a discussion of robust sample compression under total-variation corruption. Final certificate numbering is Theorem 23, not v2 Theorem 26.

## 1. Nearest solved questions
| Source | Already supplies | Does not establish the target below |
|---|---|---|
| Bennouna et al., arXiv:2602.15365v1, Proposition 10 / Appendix D | Noise robustness for a fixed sufficient measurement dataset | Discovery of that representation from noisy queries |
| Zheng et al., arXiv:1709.10061v3 | Upper/lower sampling bounds for LP optimization with noisy objective-coordinate observations | The queried-direction discovery/stable-compression guarantee sought here |
| Ye et al., arXiv:2603.18551v2 §7.3 and final Appendix E | Regression-based representation discovery from noisy full cost labels under margin assumptions | The same discovery from noisy partial linear queries |
| Hu et al., arXiv:2405.16564v3 | Offline contextual optimization with bandit/semi-bandit feedback | This particular geometric sufficiency certificate |
| Benslimane et al., arXiv:2606.01081v1 | On-policy partial-feedback learning with stationarity analysis | Intrinsic-rank representation discovery certificate |
| Ye & Bennouna, arXiv:2605.25635v1 | Exact LP compression and sample-based learning | A retrieved noisy-query resolution |

A missing claim in these retrieved papers is not proof of worldwide absence.

## 2. Precisely narrowed target
For a known bounded LP feasible region X and known prior cost set C, sample costs independently from P supported on C. Access to a sampled cost is through noisy linear queries
\[
Y_{i,j}=q_{i,j}^{\mathsf T}c_i+\xi_{i,j},
\]
with an explicitly specified noise model. Learn a query-direction set \(\widehat D\) and certify its pointwise-sufficiency failure probability on a fresh cost.

A worthwhile result must separately control:
1. number/rank of genuinely new directions;
2. number of repeated noisy measurements;
3. failure probability and relevant margin/conditioning parameters;
4. computational and oracle access assumptions.

The current noiseless algorithm makes each added direction independent. That statement cannot be silently reused for noisy observations.

## 3. Attempt A: confidence regions in place of exact fibers
Replace the exact compatibility equations by confidence tubes intersected with C. Convexity can retain the facet-relevance argument. However, a facet normal may now be dependent on earlier queries while remaining uncertain. Repeated observations can be necessary without increasing rank.

Simple diagnostic: on X=[0,1], a positive scalar cost makes 0 optimal. If a noisy observation leaves the cost confidence interval crossing 0, the same scalar direction remains uncertain. Querying it again adds a measurement, not an independent direction. This invalidates the inference “every query adds rank, hence at most d-star queries.”

Verdict: failed extension. This does not refute the existence of a better noisy algorithm. It exposes the proof obligation a valid algorithm must repair. A stronger global hyperplane-margin assumption could help simulation arguments but would not automatically solve the original direction.

## 4. Attempt B: robust cost-distribution certificate
The final paper asks about corrupted costs with total-variation distance at most epsilon. A narrow iid subcase admits the following corollary.

Assume P(C)=1, TV(Ptilde,P)≤epsilon<1, exact observations/queries of corrupted sampled costs, computable membership in C, and the original learner's assumptions. Reject sampled costs outside C. Let Q=Ptilde(.|C), and m be the accepted count. For m>0 the original learner yields
\[
R_P(\widehat D)\le
\min\left\{1,\epsilon+\frac4m
\left(6|T|+\log\frac e\delta\right)\right\},
\qquad |T|\le d^\star ,
\]
with confidence at least 1−delta. Use the trivial bound 1 if m=0.

## 5. Hand argument for the corollary
Ptilde(C)≥1−epsilon>0. On C, conditioning increases Ptilde's density; P is supported there. Therefore the probability overlap of P and Q is at least that of P and Ptilde, so TV(P,Q)≤epsilon.

Conditional on m, the ordered accepted costs are iid Q. Apply the existing fixed-m stable-compression certificate at confidence 1−delta. For every learned error event E, P(E)≤Q(E)+epsilon; total variation controls all events, including the data-dependent E after training. Conditioning on m and then averaging preserves the confidence level without a union bound across accepted counts.

No new rank budget is required because retained costs remain within C. This argument concerns covariate distribution corruption with exact corrupted costs, not noisy oracle responses or adaptive adversarial replacement of a realized sample.

## 6. Novelty verdict
Attempt B is a useful explicit consequence for the final paper's robust discussion. It uses standard conditioning/total-variation arguments and an existing learning theorem. No new algorithm, compression proof or genuinely novel open-problem solution was established.

It is retained as a supporting corollary rather than promoted into the project's research result. Lean formalizing only its final inequality would not make it a new discovery or verify the imported original learning theorem.

## 7. Does Nolan's framework improve the approach?
It usefully keeps observation loss, target choice and missing distinctions visible. In this attempt it helped separate representation discovery from deployment and distinguish query rank from repeated-measurement cost. Those are useful organizing contributions.

No superiority over existing mathematical frameworks or measured research performance was demonstrated. The meaningful test is whether it enables a correct result beyond the nearest prior theorem. This pass did not do so.

## 8. Search record and limits
Search date: 2026-09-30. Two web engines, two alphaXiv discovery calls, source PDFs, filtered full-text queries, author publications and direct arXiv version records were used. Representative exact queries:
- "Learning Decision-Sufficient Representations for Linear Optimization" noisy observations
- "decision sufficient" "noisy" linear optimization representations
- "Data Informativeness in Linear Optimization under Uncertainty" noisy measurements
- "decision-sufficient" "noisy queries"
- "decision-sufficient" "stable compression" "total variation"
- "linear optimization" "representation" "noisy measurements" "sample complexity"

alphaXiv discovery framings: noisy-query learning beyond fixed-dataset perturbation results; robust sample compression under total-variation cost corruption. Results were ranked and capped, not a complete citation census.

Failures: several arXiv HTML and raw-PDF web opens failed; the final official PDF was downloaded separately and inspected with pdftotext. Some heavily quoted queries in the second web engine returned irrelevant material. No MathSciNet, zbMATH or complete forward-citation database search was performed. Subsequent work resolution was not found; universal nonexistence is not asserted.

## 9. Publication status
No VidMath/VibeMath submission and no author email were sent. The project's goal is a useful, novel result with a faithfully stated Lean theorem and successful build evidence. No theorem from this attempt meets that combined threshold.

Lean checks proof correctness for the encoded statement and assumptions. It does not certify novelty, coverage of the original open question, empirical usefulness or correspondence between the source and formal model.

## 10. Reuse
Read existing papers instead of recreating their foundations. Future workers should start at Section 2 and repair Attempt A's rank-versus-measurement issue, or choose another explicitly open question with a more tractable gap.

## 11. Process integrity
Primary source overlap checks and independent mathematical audit prevented two overclaims. Retrieval was non-exhaustive. The imported stable-compression theorem was not re-proved or Lean verified. No result here should be described as a certified open-problem solution.

## 12. Robustness
Attempt B requires iid sampling, known support and exact queried values. Relaxing those conditions changes the problem. The noise extension remains unresolved in this work. No behavioral or token-efficiency experiment was run.

## 13. Bibliography
- Ye, Amin & Özdağlar, COLT 2026: https://proceedings.mlr.press/v336/ye26a.html ; preprint https://arxiv.org/abs/2603.18551
- Bennouna et al.: https://arxiv.org/abs/2602.15365
- Zheng et al.: https://arxiv.org/abs/1709.10061
- Hu et al.: https://arxiv.org/abs/2405.16564
- Benslimane et al.: https://arxiv.org/abs/2606.01081
- Ye & Bennouna: https://arxiv.org/abs/2605.25635

## 14. One-pass verdict
Open direction confirmed in the final source; overlap substantially narrowed; two mathematical routes attempted and audited; no defensible novel solution. Preserve this failed attempt to avoid spending the same compute again.
