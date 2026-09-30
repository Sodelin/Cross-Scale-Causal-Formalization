# Partial Views, Changing Systems, and What Their Shadows Can Identify

**Date:** 2026-09-30 UTC / 2026-09-29 Pacific  
**Origin:** Nolan Downard's cross-scale/shadow hypothesis, interpreted and analyzed with an AI assistant.  
**Status:** Conceptual research note with elementary mathematical arguments. No Lean implementation, empirical validation, novelty claim, or Millennium Problem solution.

## 0. Executive summary

The strongest reading of Nolan's hypothesis is: several partial, context-dependent observations may identify a useful property or abstraction of a hidden system, even when the complete system is not recoverable. The additional challenge is that both the system and its observation process may evolve.

Three distinct questions follow:

1. Which hidden possibilities remain compatible with the observations?
2. Which properties are the same across those possibilities?
3. Does the observed representation retain enough information to predict its own evolution or the effects of specified interventions?

These questions are formalizable. This does not require assuming universal self-similarity. Self-similarity can be introduced later as a specific, testable restriction on a class of mappings.

Evidence confidence: high for the elementary mathematical statements under their definitions; moderate for relevance of the selected causal-representation literature; insufficient for universal transfer across sciences or the proposed autism mechanism. No formal GRADE assessment was conducted.

Next work should target explicit counterexamples and conditions for informative views, before attempting application-specific claims. The immediate contribution is a precise interpretation and failure criteria, not a new theory credited to the assistant.

## 1. Abstract

A “shadow” is modeled as an observation of a latent state through a possibly changing map. Observational equivalence describes what the shadow cannot distinguish. A property can nevertheless be identified if it is constant across compatible states. A changing observation has autonomous predictive dynamics only if projecting the next hidden state does not depend on which indistinguishable hidden state was present. These conditions clarify the difference between accumulating observations, identifying mechanisms, and aligning concepts in conversation. Clinical examples motivate measurement questions but do not establish neural causes.

## 2. Introduction

The metaphor contains a meaningful shift of emphasis: incomplete access does not imply that every useful inference is impossible. A latent object, a property of that object, a useful abstraction, and a conversational label are different inference targets.

The working question is:

> Under what assumptions can a family of partial observations determine a property, predictive abstraction, or causal constraint of an evolving hidden system?

The broad ambition belongs to Nolan. The equations below are the assistant's proposed interpretation; they must not be attributed to Nolan as if he supplied them verbatim.

## 3. Method

Targeted searches examined causal representation learning under partial observability, identifiability of causal abstractions, official autism criteria and descriptions, a primary negative-symptom treatment trial, and the official Yang–Mills problem description. Original mathematical papers and official clinical sources received priority.

This is not a systematic review. No participant or client data were acquired, analyzed, or reproduced. The motivating conversation is not included. No empirical psychological model was fitted and no proof assistant was run. The arguments below can be checked directly from their definitions.

## 4. Findings: three sources of uncertainty

| Source | Mathematical/conceptual interpretation | Key failure |
| --- | --- | --- |
| Partial or distorted view | Several latent states have the same observed output | Observational nonidentifiability |
| Evolving object and lens | Latent transitions and observation maps can both change | State change can be confused with measurement change |
| Different meanings of a label | Speakers attach the same word to different represented features | Semantic alignment can be mistaken for causal validation |

A psychological diagnosis is not automatically a single latent object waiting to be discovered. Treating it as one is an assumption about the model. Diagnostic categories, dimensions, processes, and mechanisms must be distinguished.

### 4.1 A minimal observation model

Let X_t be a hidden state space, F_t a transition from X_t to X_(t+1), and h_t an observation map from X_t into Y_t:

$$
x_{t+1}=F_t(x_t), \qquad y_t=h_t(x_t).
$$

Context, actions, and noise are deliberately omitted from the first mathematical statement. They must be added before this is used as an empirical psychological model.

Variation in y can arise from x, h, or both. If the permitted observation maps are unrestricted, they can conceal arbitrary hidden trajectories: a time-specific constant map can always output the observed y_t. Thus identifiability requires restrictions or calibration; observation alone does not provide them.

A less degenerate ambiguity is y_t=c_t x_t. For any nonzero a_t, replacing x_t with a_t x_t and c_t with c_t/a_t leaves y_t unchanged. An unknown lens can therefore hide the scale and temporal evolution of the object.

### 4.2 What multiple views actually contribute

For a fixed hidden state x and calibrated views h_1,...,h_k, the compatible states are

$$
C(y_1,\ldots,y_k)=\{x:h_i(x)=y_i\text{ for every }i\}.
$$

Adding a compatible observation cannot enlarge this set when the model class and assumptions remain fixed. It need not shrink it: a duplicate or redundant view supplies no distinguishing information. Conflicting exact observations may make the set empty, indicating failure of a model, measurement, or assumption rather than certainty.

Example: observing a+b leaves many pairs possible. Observing a-b as well identifies a=(y_1+y_2)/2 and b=(y_1-y_2)/2. Observing 2(a+b) instead does not identify the pair.

In noisy settings, use a statistical likelihood or an explicit uncertainty set. Do not silently substitute exact equalities for fallible clinical measurements.

### 4.3 Identifying a property without identifying the object

**Elementary proposition.** For a fixed map h:X→Y and target property q:X→Q, there is a function q_bar:h(X)→Q with q=q_bar∘h if and only if

$$
h(x)=h(x') \Longrightarrow q(x)=q(x').
$$

**Argument:** If q factors through h, equal observations give equal q. Conversely, define q_bar(y) using any x with h(x)=y; constancy on each fiber makes the definition independent of the representative.

Here a fiber is the set of states sharing one observation. This is a standard factorization fact, not a novel theorem. It gives a useful formal statement of the central intuition: the complete hidden state may remain ambiguous while a particular property is determined.

The criterion is relative to the assumed state space and known observation map. It does not identify either from data by itself.

### 4.4 When a shadow has its own exact dynamics

**Elementary proposition for changing views.** A well-defined observed transition G_t:h_t(X_t)→h_(t+1)(X_(t+1)) satisfying

$$
G_t\circ h_t=h_{t+1}\circ F_t
$$

exists if and only if

$$
h_t(x)=h_t(x')
\Longrightarrow
h_{t+1}(F_t(x))=h_{t+1}(F_t(x')).
$$

**Argument:** Necessity follows by applying G_t to equal observations. For sufficiency, define G_t(y)=h_(t+1)(F_t(x)) for any x in the fiber of y. The stated condition makes the definition independent of that choice.

This formalizes “the shadows act in an ordered state” as one specific target: the current observation determines the next observation. It is demanding and may fail.

Counterexample: let x=(a,b), h(a,b)=a, and F(a,b)=(a+b,b). States (0,0) and (0,1) have the same present shadow, but their next shadows are 0 and 1. There is no exact one-step G on a alone.

A history of observations, additional views, or a probabilistic representation might resolve particular failures. None is guaranteed to work without assumptions. A statistical predictor can still be useful even when an exact deterministic transition does not exist; prediction and exact closure are different targets.

### 4.5 The cross-scale and causal extension

An observation quotient is not necessarily a scientifically meaningful higher-level model. To make it causal, specify interventions and require the corresponding outcomes to agree after translation between levels. The earlier research note used a distributional consistency equation; it must be evaluated for a specified intervention family, not inferred from resemblance.

Existing work directly addresses these issues:

- Lee and Bareinboim (2020) study causal-effect identification from distributions measuring different subsets of variables, under graphical assumptions.
- Yao et al. (2023 preprint) study partially observed multi-view representations, with identifiability conclusions including recovery up to smooth bijections under their assumptions.
- Li, Kaba, and Ravanbakhsh (2025) study which causal abstraction can be identified given available latent intervention patterns.

These are close precedents, not evidence that arbitrary conversational viewpoints satisfy those assumptions. [B1–B3]

## 5. Conclusion

The central hypothesis can be made precise as property identification and predictive/causal abstraction under incomplete, changing observations. The hidden object need not be uniquely recoverable for every target property to be recoverable.

Universal self-similarity, clinical mechanisms, and general transfer across disciplines remain additional hypotheses. There is no established implication from the elementary propositions to solving a major open problem.

## 6. Deconstructive analysis: top down

Start with the claimed inference and ask what its target is: a latent state, a trait dimension, a diagnosis, a transition, an intervention effect, or a speaker's intended meaning. Then specify the observations and assumptions that distinguish it.

“People understood each other” supports conversational alignment. It does not by itself establish a neural mechanism. A fitting label can organize a conversation without identifying a unique underlying cause.

## 7. Reconstructive analysis: bottom up

Start with observable behaviors or measurements, their contexts, and their errors. Identify which distinctions each view loses. Combine views only when their correspondence or calibration is justified. Determine whether the target property varies within the remaining equivalence class.

Self-similarity should be defined explicitly: invariant scaling, correspondence of graphs, recurring motifs, shared transition structure, or another stated relation. Those are different mathematical hypotheses; shared vocabulary is not evidence of any one of them.

## 8. Middle-out synthesis and clinical boundaries

Nolan's psychological example suggests a distinction between an individual's experience, the construct used to organize it, and a proposed causal mechanism. That distinction is valuable even when the mechanism proposed during a conversation is incorrect.

Autism is not established as a reward pathway specializing while other pathways atrophy. NIMH describes developmental influences involving genes and environment and does not identify a single primary cause. Reduced engagement or different functioning is not equivalent to structural atrophy. CDC criteria include social-communication differences and restricted/repetitive behavior; support levels describe support requirements in those domains, not the amount of brain atrophy. [B4–B5]

Schizophrenia includes psychotic, negative, and cognitive domains. Negative symptoms are not uniquely the “real” disorder, nor is autism established as its opposite. Negative symptoms can be difficult to treat, but universal untreatability is too strong: a randomized active-comparator trial reported greater improvement in predominant negative symptoms with cariprazine than risperidone in a selected population. This is a bounded finding, not a treatment recommendation or general cure claim. [B6–B7]

The specific clinical mechanism can be rejected without losing the measurement and abstraction question. Agreement on a metaphor supplies no additional biological verification.

## 9. Glossary

- **Identifiability:** Whether the available information and assumptions uniquely determine the specified target, possibly up to a stated equivalence.
- **Fiber:** Hidden states with the same observed value.
- **Observational equivalence:** Models or states indistinguishable by specified observations.
- **Closure:** The projected representation supports the specified dynamics without needing additional hidden distinctions.
- **Calibration:** Restrictions or anchors linking the observation process to the system.
- **Semantic alignment:** Establishing which represented distinctions speakers mean.
- **Self-similarity:** A specified form of structural recurrence; its mathematical meaning must be chosen.

## 10. Bibliography

- **B1.** Lee, S., & Bareinboim, E. (2020). [Causal Effect Identifiability under Partial-Observability](https://proceedings.mlr.press/v119/lee20a.html). ICML, PMLR 119, 5692–5701. Establishes conditional graphical identification results.
- **B2.** Yao, D., et al. (2023 preprint). [Multi-View Causal Representation Learning with Partial Observability](https://arxiv.org/abs/2311.04056). Provides conditional multi-view identifiability results; verify final venue metadata on import.
- **B3.** Li, X., Kaba, S.-O., & Ravanbakhsh, S. (2025). [On the Identifiability of Causal Abstractions](https://arxiv.org/abs/2503.10834). AISTATS 2025; arXiv record provides publication status.
- **B4.** NIMH. [Autism Spectrum Disorder](https://www.nimh.nih.gov/health/publications/autism-spectrum-disorder). Official clinical overview.
- **B5.** CDC. [Clinical Testing and Diagnosis for Autism Spectrum Disorder](https://www.cdc.gov/autism/hcp/diagnosis/index.html). Diagnostic criteria and support levels.
- **B6.** NIMH. [Schizophrenia](https://www.nimh.nih.gov/health/publications/schizophrenia). Official symptom-domain overview.
- **B7.** Németh, G., et al. (2017). [Cariprazine versus risperidone monotherapy for treatment of predominant negative symptoms in patients with schizophrenia](https://doi.org/10.1016/S0140-6736(17)30060-0). The Lancet, 389, 1103–1113. Primary randomized trial.
- **B8.** Clay Mathematics Institute. [Yang–Mills & the Mass Gap](https://www.claymath.org/millennium/yang-mills-the-maths-gap/). Official open-problem description.
- **B9.** Beckers, S., & Halpern, J. Y. (2018 preprint). [Abstracting Causal Models](https://arxiv.org/abs/1812.03789). Background from earlier research; distinct abstraction requirements.

## 11. Metacognitive reflection: process integrity

**Process integrity: Moderate for a conceptual note; inadequate for an exhaustive novelty or clinical mechanism review.** This is a qualitative local assessment, not an AMSTAR-2 score. Strengths: primary and official sources, directly inspectable elementary arguments, explicit attribution and limits. Weaknesses: one extractor, targeted search, no preregistration, no comprehensive failed-theory search, no original data.

RoB-2 would be relevant to a full assessment of B7; it was not completed. B7 is used only to rebut a blanket claim, not to estimate comparative treatment effectiveness. Improvements: source-specific theorem assumption extraction, counterexample collection, and independent mathematical review.

## 12. Metacognitive reflection: inference robustness

The factorization and closure arguments are exact under their definitions. Their empirical applicability is untested. No meta-analysis was performed, so Q, tau-squared, I-squared, funnel/Egger analyses, and pooled effects are inapplicable.

Potential biases: treating all constructs as hidden single objects; confusing coherent interpretation with evidence; inferring causal structure from verbal similarity; interpreting a familiar theorem as validation of the entire hypothesis.

What would change the verdict: informative calibrated views and stable results on unseen contexts could support a specific application; observationally equivalent models with conflicting target properties would refute identifiability for that setup. Failure of closure would require enriching the representation or weakening the claim. No result here establishes cross-disciplinary universality.

## 13. Zotero and Obsidian integration

Collection: Cross-Scale Causal Formalization / Partial Observability. Import B1–B3 and B9 as scholarly items, B7 using its DOI, and B4–B6/B8 as institutional web pages. Tags: identifiability, observation-map, causal-abstraction, dynamic-closure, semantic-alignment, clinical-boundary.

For each paper, extract: target of identification; available views/interventions; assumptions; equivalence allowed; counterexamples; empirical scope. Relate B1–B3 as neighboring identification frameworks. Keep clinical background separate from mathematical proof claims.

Obsidian links: [[Shadow hypothesis]], [[Identifiable properties]], [[Changing observation maps]], [[Causal abstraction]], [[Operationalization]]. This note contains no invented Zotero IDs or citation keys.

## 14. Appendix: open problems and next precise question

“EA Mills/Gann Mills” is tentatively interpreted as Yang–Mills. If that interpretation is correct, the official problem concerns constructing a nontrivial four-dimensional quantum Yang–Mills theory and proving a positive mass gap. The present abstractions do not supply those results. A future application would need a precise construction and a theorem connecting its representations to the required quantum-field properties. [B8]

The “topology and algebra revolution question” was not identified from the spoken description. No particular conjecture is assigned to that phrase.

The next focused mathematical question is:

> When observations and hidden dynamics both vary, which restrictions let us distinguish measurement change from system change sufficiently to identify a specified property or predictive abstraction?

The next empirical question is different:

> Which measurements and contexts are justified for a particular psychological construct?

Keeping those questions distinct protects the value of Nolan's proposal while allowing particular formulations to fail.
