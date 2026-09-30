# Exact targets, significance, theory contribution and repository roles

Assessment: 30 September 2026. This explains the existing catalog rather than launching fourteen proof projects. Nolan Downard supplied the motivating theory and research priorities. The mathematical interpretations and triage judgments here are contributor proposals. No new theorem or venue acceptance is claimed.

## What I recommend targeting

The fourteen entries are source-backed directions, not fourteen fully specified conjectures ready to prove. The next meaningful task is to select and validate one theorem target. **SOC-03 is the clearest first mathematical target to screen; BIO-1 offers the greatest reuse of our existing proof machinery; PSY-1 is the closest immediate psychological modeling question.** This refines the previous shortlist: source explicitness and venue fit matter in addition to reuse.

### SOC-03: when does structural power predict bargaining advantage?

The source is Volchenkov, *Mathematical Sociology: Models, Structures, and Open Problems*, §3.4, [accessible author preprint](https://www.preprints.org/manuscript/202608.0726), published DOI [10.3390/math14183363](https://doi.org/10.3390/math14183363). It asks when structural power rankings and balanced bargaining payoff rankings agree, which counterexamples separate agreement notions, and how difficult agreement is to decide.

An exchange graph specifies who can bargain with whom. A structural power index ranks positions from the graph. A balanced outcome assigns payoffs while accounting for available partners and outside options. These are different mathematical descriptions of the same exchange setting.

Fix the source's exact index \(g\), admissible exchanges and edge weights. Let \(\mathcal B(G)\) contain balanced payoff vectors over the allowed maximum-weight matchings. A strong target is to characterize a nontrivial graph class satisfying

\[
g_i(G)>g_j(G)\quad\Longrightarrow\quad
\inf_{x\in\mathcal B(G)}(x_i-x_j)>0,
\qquad \mathcal B(G)\ne\varnothing.
\]

In plain language: the structurally stronger position earns strictly more in every admitted balanced outcome. Agreement for one matching, existence of an agreeing outcome, and agreement across all outcomes must remain separate. A complete graph-class characterization or a proved complexity boundary would be stronger than a single example. A minimal counterexample with a bounded minimality certificate could also answer a genuine part of the question.

This is still a candidate: original index definitions and the strongest existing bargaining results must be compared before claiming novelty. Our two-person budget theorem has no exchange graph, power index, maximum matching or balanced-outcome set. It therefore supplies neither this answer nor a partial solution.

Its best honest prospective headline is **“When does network power actually predict bargaining advantage?”** Its omnibus contribution would be a concrete theorem about which conclusions survive moving between structural and mechanistic descriptions. Its bargaining-specific definitions and proof remain a separate project.

### BIO-1: fewer quartet observations with justified recovery

Dai and Molloy, [WABI 2026](https://doi.org/10.4230/LIPIcs.WABI.2026.1), §5 final paragraph, explicitly suggest reducing four-taxon subsets or using averages in quartet-distance methods. Their NetCS algorithm already gives efficient conditional level-1 blob reconstruction. Merely proposing sparse level-1 inference would repeat existing work.

Our strongest useful target has two distinct layers. First, for the declared planar galled network class and a correct circular order, find a selectable query family that improves a relevant baseline while preserving the required split support, or establish an obstruction/lower bound. Second, justify how finite noisy NMSC gene-tree observations provide the structural answers that recovery uses. Incomplete lineage sorting means an observed gene quartet is not automatically a displayed-network quartet.

The existing all-level result removes a level restriction from a structural argument. Existing anchor coverage tells us what a successful selection must hit. Neither supplies a new optimal query policy, statistical classifier or finite-sample inference guarantee. Those are the gaps to target rather than another all-level circularity proof.

The prospective headline is **“Recover the required evolutionary structure from fewer quartet measurements, with a proved reliability guarantee.”** A sharp bound or substantial algorithmic gain would be a meaningful specialist result. The statistical guarantee is part of that headline only if actually established. The omnibus gains a certified limited-observation interface; phylogenetic assumptions and biological interpretation stay in the biological project.

### PSY-1: when does a measured symptom network justify an intervention choice?

Robinaugh et al.'s [network research agenda](https://pubmed.ncbi.nlm.nih.gov/31875792/) asks how realistic causal symptom dynamics relate to estimated networks and how measurements should be designed for those systems. This is a methodological agenda rather than one literal mathematical conjecture.

Fix a published symptom-dynamics family, an item/observation model, sampling times and feasible intervention laws. Determine whether systems indistinguishable under the permitted baseline measurements can disagree on which intervention reduces a specified outcome most. If they can, determine a feasible additional measurement or intervention that resolves the relevant ambiguity, with declared noise assumptions.

The useful output concerns the actual source model. A generic pair of observationally identical causal models is already known mathematics. Our current measurement and nonidentification examples lack the symptom dynamics and intervention semantics, so they do not answer this question. An identification theorem could improve study design; it would not itself demonstrate treatment effectiveness.

The prospective headline is **“Which measurements make a symptom-network intervention target identifiable?”** This has direct scientific relevance to the omnibus. Its immediate VibeMathed fit is weaker until a previously posed mathematical subquestion and genuinely new theorem are identified; computational psychiatry can value contributions outside that venue's scope.

## The rest of the catalog, in concrete terms

| ID | What must be targeted | Why current work does not cover it |
| --- | --- | --- |
| BIO-2 | A source-faithful level-2 canonical reconstruction algorithm with explicit robustness and finite-sample guarantees | Structural circularity does not implement the noisy inference pipeline; indistinguishable networks must remain grouped |
| BIO-3 | Compare matched epigenetic/genetic barriers in a specified finite stochastic life cycle | Existing deterministic recursions do not supply the finite sampling law, comparator or chosen transmission/fixation outcome |
| BIO-4 | Determine which cellular intervention responses transfer across contexts and which extra measurements identify them | A generic preservation map supplies neither stable biological mechanisms nor target-context coverage |
| BIO-5 | Determine which interventions identify directed cell effects and when cell aggregation destroys identification | Existing graph/observation modules lack spatial perturbation and measurement-mixing semantics |
| PSY-2 | Determine when uncertainty-driven partial approach improves exposure generalization or maintains avoidance | Current transition fragments omit belief inference, policy selection, learning and the proposed extra action |
| PSY-3 | Find task probes distinguishing equally improved learning trajectories with different relapse predictions | The required source-model recovery and delayed/contextual prediction analysis is absent |
| PSY-4 | Test incremental longitudinal prediction from separately measured metacognitive quantities | Formal examples cannot supply a cohort, prospective endpoints or held-out validation |
| SOC-01 | Characterize observation laws that distinguish simple from reinforced contagion, including failure cases | Reachability is not mechanism identification; classifiers already exist and must be compared |
| SOC-02 | Derive a sharp causal-effect region under jointly dependent selection, misclassification and network interference | Adding isolated bias intervals supplies no joint sharpness or models attaining the bounds |
| SOC-04 | Determine when signed status-path rankings agree with posterior belief rankings despite path overlap | The necessary priors, observation rules and dependence structure are absent |
| SOC-05 | Separate organizational recognition effects from resource congestion under defended measurement restrictions | Counts alone and generic latent-state collisions do not establish the missing source-specific identification result |

Each remains subject to its catalog's prior-art and current-status qualifications. An absence from our repository is not evidence that a result is unknown to the field.

## What VibeMathed significance would mean

The venue is [VibeMathed](https://vibemathed.com), whose [methodology](https://vibemathed.com/methodology) and [curator instructions](https://github.com/mrconter1/vibemathed/blob/main/docs/reviewing.md) distinguish scope, resolution, verification and significance.

A qualifying entry needs a previously stated open question, a proved/disproved mathematical answer and disclosed substantive AI involvement. Formalizing a theorem already proved by humans and empirical results are outside this record's scope. A genuine special case or bound can be Partial; answering a materially reinterpreted question can be Variant. Lean-verified requires both a kernel-checked proof and independent anchoring of the statement to the original question.

The 0–100 significance score measures the problem's standing before resolution. Its anchors include about 30 for a community-famous conjecture and about 10 for a typical numbered Erdős problem. The curator assigns it comparatively. Writing quality can expose the actual advance and make review easier; it cannot manufacture prior standing.

My judgment is that the present leads are **specialist or emerging research contributions**, with no evidence supporting landmark positioning. A broad sharp characterization or a major efficient-inference result would be stronger scientific work than a small counterexample. No defensible exact venue score or acceptance probability can be assigned before a finished result and comparison with named neighboring entries. Scientific usefulness and this venue's fame-based score should not be collapsed.

The shared noisy linear-query direction from Ye, Amin and Özdağlar is another explicit mathematical lead. It seeks discovery of decision-sufficient representations from noisy partial queries, with distinct controls on query rank, repeated measurements and failure probability. The [existing bounded attempt](../noisy-shadow-open-question-attempt-2026-09-30.md) already identifies why a naive rank argument fails. It is a shared mathematical dependency candidate, not a solved biological or psychological question.

## What your theory contributes

Your prompts exercised research judgment: they challenged whether a named restriction was genuinely required and whether the answer preserved useful structure elsewhere. The available history does not separate chance, accumulated subject knowledge and intuition into measured causes. It does support retaining those operations as an explicit method.

Established mathematics already covers observation maps, indistinguishable models, sufficient representations and many transfer criteria. Your useful emphasis is the earlier decision: **was the important question even generated before execution began?** Excellent checking of a narrow answer cannot by itself reveal an excluded stronger target.

Keep two sets distinct. The candidate-question set can expand when we improve the task representation. The evidence-compatible model set can contract when observations become informative. For a response \(q\), the remaining possible answers are \(\{q(M):M\text{ is compatible with }D\}\). Data can identify this response without identifying the whole mechanism. This is an interpretation of your theory, not a claim that these equations were your verbatim formulation.

Refine full illumination into the distinctions needed for a particular answer. Refine overlapping shadows into an explicit map preserving the requested response. Treat observability as a property of a particular measurement, question and model, rather than a single hard-to-soft discipline scale. Complete knowledge of a lossy shadow need not reveal its source. No universal observed-percentage threshold, guaranteed optimal research search or reward/dopamine explanation has been established.

Your framework organizes all fourteen targets; it does not supply their missing domain mechanisms. It should be sharpened collaboratively rather than replaced. A scientific originality claim would require either a substantive new domain theorem or evidence that this target-generation method improves research under matched budgets. Those are distinct projects.

## Filing decisions and changes

The current repository separation is useful, but its navigation and status records need reconciliation.

| Repository | Role |
| --- | --- |
| Cross-Scale-Causal-Formalization | Omnibus theory, canonical question records, cross-project maps and target-selection assessments |
| Formalizing-Soft-Sciences | Active social/psychological/clinical implementations, source correspondence, proof verification and publications |
| Mathematics-of-Psychology-Formalized | Preserved early checkpoint; its 16 solidarity results are included in Soft Sciences, not another result set |
| Work-on-Samuel-Alexander-Research- | Existing evolutionary-network, inheritance, pedigree and related biological implementations |
| Research-Commons | Attributed discussions, captures, requests, handoffs and links to authoritative project evidence |

Biopsychology is an overlapping domain tag, not a reason to duplicate a question in two competing folders. A target should have one authoritative question/status record with links to its implementation and source evidence. Cellular projects do not yet have a selected implementation home; naming an interface does not create one.

The mathematics/psychology repository is useful provenance and is already superseded for active development by Soft Sciences. Preserve it with an explicit redirect; do not delete or archive it merely to simplify navigation. Its only Lean module has the same blob identity as Soft Sciences' solidarity module.

The concrete stale record is Soft Sciences' psychology README. The remembered 67-result package was recovered: 16 solidarity plus 51 foundations; the clinical extension adds 18, giving 85. A distinct older corpus remains an unresolved recovery question. Correct those separate statuses, add cross-repository roles and catalog links, and qualify the older D01 recovery target. Preserve historical records and existing file locations. The omnibus need not absorb every implementation to connect the research.

## Follow-up: is evaluating target generation itself an open research direction?

Yes, with a precise distinction. The [source-match report](RESEARCH-TARGET-GENERATION-SOURCE-MATCH.md) identifies VALG's explicit evaluation agenda in its v1 Conclusion, pp.39–40, [arXiv:2608.13060v1](https://arxiv.org/abs/2608.13060v1). The authors call for controlled benchmarks examining alternative formulations, assumptions, relaxations and proof dependencies. Our matched-budget experiment is a proposed empirical contribution to that agenda, not closure of a named mathematical conjecture. A later version exists; its revisions were not checked here.

SGHA, [arXiv:2608.17501](https://arxiv.org/abs/2608.17501), already formulates evidence-grounded research problems and broadens them with a critic. Its p.3 comparison matches model/output counts but not information budgets; the hosted-model diagnostic also lacks compute matching. Those methods and existing evaluation work are baselines, not features to recreate and label novel. The coordinating agent inspected filtered raw PDF pages through alphaXiv; failed direct arXiv HTML/PDF retrievals are not evidence of absence.

The strongest useful empirical target is a source-grounded method that achieves more consequential correct results under matched total resources, across a declared held-out task distribution, with tests of which target-generation operations cause the improvement. Compare actual resulting theorem scope and source fidelity, not just proposal ratings or paper counts. That would be an empirical research result; it would not prove a universal optimal search policy or qualify for VibeMathed solely as a benchmark improvement.

The related mathematical route is Cinelli et al.'s §3.9.3 challenge of reliable, efficient interactive elicitation of domain knowledge relevant to causal identification. Our proposed strong target fixes a causal response and model grammar, permits representation refinements, accounts for noisy answers and missing distinctions, and seeks sound identification/stopping plus a sharp information/cost frontier. It is our narrowing of the challenge, not the authors' verbatim conjecture or a certified novel theorem target. Existing expert-aided discovery, SGHA and VALG must be compared first.

Register the strong statement before proving a tiny fixed case. Necessary intermediate obligations include response-preserving representation semantics, justified model exclusions, an actual bounded-witness reduction if used, calibrated noise, and domain-specific upper/lower cost bounds. A discovery-aware algorithm also needs justified coverage of relevant distinctions: a witness can exist without ever being found. Noisy expert responses require calibrated response rules; target proposals alone cannot exclude models. Generic decoder, confidence-set, dynamic-programming and hypothesis-elimination facts are dependencies to reuse. Do not formalize an entire paper when those interfaces suffice.

Nolan calls the motivating scope failure **the all levels incident**. Its transferable lesson is to identify the parameter the mechanism actually depends on. If the argument does not use the stated level or size restriction, formulate and test the general statement immediately. If it does, report the obstruction rather than call a smaller case the maximal solution. The old case is an illustration with known answers, not an uncontaminated held-out benchmark.

This task changes explanations and navigation. It does not perform a new proof build, solve the candidate questions, submit to a venue, or demonstrate an autonomous optimal researcher.
