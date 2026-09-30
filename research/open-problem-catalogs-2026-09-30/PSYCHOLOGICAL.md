# Psychological open-problem catalog for the cross-scale omnibus

Checked 30 September 2026. This catalog preserves four **externally stated research directions**, then separates each direction from our proposed bounded mathematical or empirical target. An author-stated direction is not necessarily a literal conjecture, and a proposed target is not automatically new. No entry below is admitted as a newly solved open problem or as an immediate Lean proof task.

The omnibus should distribute work through observation, latent-state, action, learning and outcome interfaces. Existing measurement, controlled quotient and stochastic abstraction results are reusable prior work. They do not establish psychological construct validity or treatment effectiveness.

| ID | Source question | Next work | State |
|---|---|---|---|
| PSY-1 | How do realistic causal symptom systems relate to estimated networks and intervention targets? | Source-specific model and identification probe | Investigate model/prior art |
| PSY-2 | Can uncertainty-driven partial approach enable exposure and cross-context learning? | Subsequent-work and missing-mechanism search | Hold |
| PSY-3 | Can learning measurements distinguish durable change from relapse-prone change? | Published-task discrimination probe | Investigate identification/validation |
| PSY-4 | Do longitudinal awareness measures add prognostic value beyond cognition and biomarkers? | Dataset feasibility and prospective estimand | Empirical collaboration required |

PSY-1 and PSY-3 are the two smallest mathematical/inference investigations. Their first outputs should be source-model counterexamples or a discriminating experiment specification. Reproving generic causal nonidentification or automata minimization would not answer the source problem. PSY-2 reuses the existing CBT starter rather than turning its current missing mechanisms into an unsourced proof queue. PSY-4 is a meaningful biology–psychology interface, but the scientific conclusion requires real longitudinal evidence.

## PSY-1: When do measured symptom networks identify a causal intervention target?

**External source:** Robinaugh, Hoekstra, Toner and Borsboom (2020), *The network approach to psychopathology: a review of the literature 2008–2018 and an agenda for future research*. [DOI 10.1017/S0033291719003404](https://doi.org/10.1017/S0033291719003404); [PubMed 31875792](https://pubmed.ncbi.nlm.nih.gov/31875792/); [PMC text](https://pmc.ncbi.nlm.nih.gov/articles/PMC7334828/). **Locator:** Network Psychometrics → Critical Analysis & Future Directions, first and third development priorities; Empirical Studies → Critical Analysis & Future Directions. **Access:** complete PMC body retrieved; source agenda primary author statement, review not primary empirical study. **Question type:** Author-stated methodological research direction, not literal mathematical conjecture.

**Author-stated unresolved direction, paraphrased:** Clarify how realistic causal symptom systems produce estimated cross-sectional and within-person networks, and develop measurement strategies designed for those systems.

**Current status:** Source direction remains relevant; exact proposed bounded target not proven currently open. Clinical causal/model fidelity and mathematical novelty must be screened. Closest results screened:

- [Evaluating potential effects of distress symptoms’ interventions on suicidality: Analyses of in silico scenarios](https://pubmed.ncbi.nlm.nih.gov/37992776/) (2024; DOI 10.1016/j.jad.2023.11.060; PubMed abstract). Provides in-silico intervention methodology; this must be reused/compared rather than rediscovered.
- [Depression symptom network reorganization under internet-based emotion regulation intervention: Evidence from a large real-world cohort](https://pubmed.ncbi.nlm.nih.gov/42804257/) (2026; DOI 10.1037/amp0001798; PubMed abstract). Large observational study explicitly precludes causal inference; network change is not proof of causal target validity.

**Our operational target:** For a source-specified family M of controlled symptom dynamics with an observation channel h and permitted intervention set A, characterize when two models with indistinguishable permitted baseline observations disagree on q = expected symptom burden after a named intervention. Find a least-cost permitted measurement/intervention that separates the q-relevant equivalence classes, or certify nonidentification in M.

**Assumptions that must be exposed:** Explicit observation channel, symptom scale and sampling interval; Declared latent model class and clinical intervention semantics; Stochastic kernel/model errors and confounding assumptions stated separately; Costs of permitted measurements/interventions fixed before optimization.

**Data/source requirements:** Source equations or recoverable simulation implementation; Instrument/item definitions and feasible intervention menu; Synthetic data suffice for initial identifiability falsification; real longitudinal/intervention data required for empirical assessment.

**Reusable assets and their limits:**

- [Measurement.lean](https://github.com/Sodelin/Formalizing-Soft-Sciences/blob/4cf7366db359317e974416d81a0fe5d6aa258f6e/SocialScience/Measurement.lean): Elementary additive bias intervals only; no construct validity or fitted item model.
- [PredictiveState.lean](https://github.com/Sodelin/Work-on-Samuel-Alexander-Research-/blob/35570664221956edd153cceaa5351a9f7d63605f/research/open-problems/time-self-reference/predictive-memory/PredictiveState.lean): Exact behavioral equivalence across action words; reusable established abstraction substrate, not new psychology mechanism identification.
- [StochasticAbstraction.lean](https://github.com/Sodelin/Work-on-Samuel-Alexander-Research-/blob/35570664221956edd153cceaa5351a9f7d63605f/research/open-problems/time-self-reference/predictive-memory/StochasticAbstraction.lean): Exact joint observation/action law preservation under pushforward conditions; not a fitted clinical model.

**Prior art to reuse:** Causal graphical equivalence, hidden-state identification, experiment design, and decision-sufficient representations are prior art. Do not spend a proof budget rebuilding a generic separating-query theorem; first instantiate and compare a clinical source model and existing intervention methodology.

**Omnibus interface:** Produces observation, latent-state, intervention and outcome contracts linking social stressors and biological state variables to psychological endpoints, with explicit identified vs nonidentified claims.

**What would count as a consequential output:** A source-model counterexample to centrality-as-intervention ranking, or an identifiable decision criterion with measurement cost and exact scope. Either can change study design; an unrelated generic quotient is insufficient.

**Lowest-cost next falsification:** Read the 2024 in-silico method equations/code and attempt two source-consistent dynamics with the same baseline measured network but different intervention ranking. Stop if existing theory already fully supplies the proposed result; reuse it and seek the unresolved source-specific limitation.

**Coverage limitation:** Bounded PubMed searches and selected records, not complete network-causal-identification literature. The 36-result recent search screened first5 latest only; future print-dated records were not used as dated closure evidence.

## PSY-2: When does uncertainty-driven information seeking inhibit versus enable exposure and generalization?

**External source:** Smith, Moutoussis and Bilek (2021), *Simulating the computational mechanisms of cognitive and behavioral psychotherapeutic interventions: insights from active inference*. [DOI 10.1038/s41598-021-89047-0](https://doi.org/10.1038/s41598-021-89047-0); [PubMed 33980875](https://pubmed.ncbi.nlm.nih.gov/33980875/); [PMC text](https://pmc.ncbi.nlm.nih.gov/articles/PMC8115057/). **Locator:** Discussion, paragraph beginning Yet another important topic not addressed is intolerance of uncertainty (previous ledger: XML Sec11 paragraph12). **Access:** complete PMC body retrieved in two offsets. **Question type:** Explicit model extension/simulation research direction.

**Author-stated unresolved direction, paraphrased:** Extend the active-inference model to simulate uncertainty tolerance and partial approach as information seeking, because expected effects on avoidance, exposure and generalization were not simulated.

**Current status:** HOLD. Continuing openness of this exact extension remains inconclusive; no closure or novelty claim. Closest results screened:

- [Using computational models of learning to advance cognitive behavioral therapy](https://pubmed.ncbi.nlm.nih.gov/40289220/) (2025; DOI 10.1038/s44271-025-00251-4; complete PMC body retrieved). Newer learning/representation framework and testable treatment-response hypotheses; does not establish closure of the exact uncertainty/partial-approach extension.
- [Modeling and controlling the body in maladaptive ways: an active inference perspective on non-suicidal self-injury behaviors](https://pubmed.ncbi.nlm.nih.gov/38028726/) (2023; DOI 10.1093/nc/niad025; PubMed abstract). Different uncertainty/body-control target; not a solution of CBT partial approach.

**Our operational target:** Within a source-consistent extended active-inference model, define approach, avoid, and partial-approach actions, stochastic observations, inference/learning and context transfer. Characterize parameter regions in which informative partial approach improves learned approach in an untrained context versus information seeking maintaining avoidance. Target a model-specific sharp phase boundary or robust transfer bound only after prior-art screening.

**Assumptions that must be exposed:** Action semantics and information/reward coefficient explicitly specified; Learning and posterior equations taken from source code or changes individually justified; Training vs untrained context defined; Parameter family/budget fixed; source model fidelity separate from clinical validity.

**Data/source requirements:** Pinned MATLAB source and model extension specification; Defined simulation endpoints and generalization contexts; Clinical fitting and external validation needed for clinical claims; not required for exploratory simulation.

**Reusable assets and their limits:**

- [PublishedCBT.lean](https://github.com/Sodelin/Formalizing-Soft-Sciences/blob/4cf7366db359317e974416d81a0fe5d6aa258f6e/clinical/ClinicalModels/PublishedCBT.lean): Source-linked deterministic transitions/outcome tables; no policy selection, stochastic inference, exposure learning, or clinical effectiveness proof.
- [StochasticAbstraction.lean](https://github.com/Sodelin/Work-on-Samuel-Alexander-Research-/blob/35570664221956edd153cceaa5351a9f7d63605f/research/open-problems/time-self-reference/predictive-memory/StochasticAbstraction.lean): Exact joint observation/action law preservation under pushforward conditions; not a fitted clinical model.

**Prior art to reuse:** Existing active-inference/POMDP decision theory and information-seeking/exposure models are dependencies, not novel results. Current PublishedCBT deterministic fragment does not encode the mechanisms required by this question.

**Omnibus interface:** Learning and policy module relating observable information, bodily arousal/affect, actions and social-context transfer.

**What would count as a consequential output:** A source-consistent simulation distinguishing two uncertainty regimes plus a consequential verified claim absent from closest work. A generic decision threshold alone fails the contribution gate.

**Lowest-cost next falsification:** Search citing/subsequent source-model implementations for uncertainty tolerance and partial approach; inspect the closest one before implementing. Then compare the missing-mechanism list against the current Lean fragment. If the exact extension already exists, reuse it and target its documented limitation.

**Coverage limitation:** Exact PubMed Title/Abstract uncertainty + active-inference query2022–2026 returned1 adjacent record. This excludes neither unindexed work nor papers using different terminology. An earlier untagged title query broadened incorrectly and was discarded.

## PSY-3: Which learning measurements distinguish durable exposure change from rapid change that later relapses?

**External source:** Berwian, Hitchock, Pisupati, Schoen and Niv (2025), *Using computational models of learning to advance cognitive behavioral therapy*. [DOI 10.1038/s44271-025-00251-4](https://doi.org/10.1038/s44271-025-00251-4); [PubMed 40289220](https://pubmed.ncbi.nlm.nih.gov/40289220/); [PMC text](https://pmc.ncbi.nlm.nih.gov/articles/PMC12034757/). **Locator:** Refining treatment; Discussion → Testing the predictions, paragraphs1–4 and Figure3. **Access:** complete PMC body retrieved in two offsets. **Question type:** Author-stated predictive/mechanistic research questions and proposed tests.

**Author-stated unresolved direction, paraphrased:** Can measured latent-cause learning tendencies predict who relapses after exposure, and can model-derived mechanisms guide interventions preventing relapse? Behavioral improvement alone may arise through different learning mechanisms.

**Current status:** Published2025 agenda; existing prototype already fits learning tendencies. Exact mathematical discrimination/measurement target and prospective clinical value are unresolved in this bounded screen, not certified novel. Closest results screened:

- [Source's existing prototype](https://pubmed.ncbi.nlm.nih.gov/40289220/) (2025; DOI 10.1038/s44271-025-00251-4; complete source). Figure3 and cited ref15 already implement a behavioral learning task and fitted model; do not claim to invent latent-cause fitting or relapse modeling.

**Our operational target:** Take the published task and fitted latent-cause model family as fixed. Define the prediction q = recovery-of-fear distribution under a specified delayed/new-context probe. Determine which model parameter/latent-update alternatives are q-equivalent on the existing task, and the smallest feasible added trial or observation schedule separating q-relevant alternatives with a stated noise tolerance.

**Assumptions that must be exposed:** Fixed model equations, priors, task protocol and outcome definition; Parameter identifiability distinct from q-identifiability; Feasible probe set and sampling/measurement noise model declared; A recovered model parameter is not assumed to measure a clinical construct.

**Data/source requirements:** Author task materials and fitted model/code; retrieve ref15 before implementation; Trial-level behavioral data or openly licensed simulation input; Prospective treatment/relapse follow-up for empirical clinical predictive utility.

**Reusable assets and their limits:**

- [PredictiveState.lean](https://github.com/Sodelin/Work-on-Samuel-Alexander-Research-/blob/35570664221956edd153cceaa5351a9f7d63605f/research/open-problems/time-self-reference/predictive-memory/PredictiveState.lean): Exact behavioral equivalence across action words; reusable established abstraction substrate, not new psychology mechanism identification.
- [StochasticAbstraction.lean](https://github.com/Sodelin/Work-on-Samuel-Alexander-Research-/blob/35570664221956edd153cceaa5351a9f7d63605f/research/open-problems/time-self-reference/predictive-memory/StochasticAbstraction.lean): Exact joint observation/action law preservation under pushforward conditions; not a fitted clinical model.
- [PublishedCBT.lean](https://github.com/Sodelin/Formalizing-Soft-Sciences/blob/4cf7366db359317e974416d81a0fe5d6aa258f6e/clinical/ClinicalModels/PublishedCBT.lean): Source-linked deterministic transitions/outcome tables; no policy selection, stochastic inference, exposure learning, or clinical effectiveness proof.

**Prior art to reuse:** Identifiability, active experimental design, latent-cause models, and exact behavioral quotients are established prior work. A worthwhile new target must improve this published task's discriminative capability or establish a source-specific impossibility/robustness result.

**Omnibus interface:** Exports a q-relevant representation and measurement contract. Bridges psychological learning variables, observable behavior, clinical outcome and context changes without pretending one mechanism is uniquely reconstructed.

**What would count as a consequential output:** A practical additional probe justified by an equivalence/discrimination certificate, or proof that allowed probes cannot support the proposed prediction. Clinical prediction requires prospective testing beyond that theorem.

**Lowest-cost next falsification:** Reproduce the published task-model mapping only far enough to test whether alternative learning mechanisms produce the same recorded trajectories but different delayed predictions. Compare against source ref15 and model-recovery analyses before proving anything.

**Coverage limitation:** PubMed2025–2026 Title/Abstract latent-cause + relapse/psychotherapy/exposure search returned0 because the specific term is absent even from the known2025 abstract. That is an index/query coverage gap, not evidence of openness. Citation chain and model comparison remain required.

## PSY-4: Do standardized longitudinal metacognitive measures add predictive value beyond cognition and biomarkers?

**External source:** Cappa, Ribaldi, Chicherio and Frisoni (2024), *Subjective cognitive decline: Memory complaints, cognitive awareness, and metacognition*. [DOI 10.1002/alz.13905](https://doi.org/10.1002/alz.13905); [PubMed 39051174](https://pubmed.ncbi.nlm.nih.gov/39051174/); [PMC text](https://pmc.ncbi.nlm.nih.gov/articles/PMC11497716/). **Locator:** Metacognition and awareness sections; ACD: Implications for diagnosis and clinical management of SCD patients, paragraph on no gold-standard objective assessment. **Access:** complete PMC body retrieved. **Question type:** Author-stated unmet measurement need and longitudinal clinical research direction.

**Author-stated unresolved direction, paraphrased:** Develop objective performance-evaluation measures and test longitudinally whether over/underconfidence or efficiency helps predict progression in subjective cognitive decline, while accounting for informant bias.

**Current status:** Current published agenda corroborated by2026 review; clinical incremental prediction unresolved in inspected sources. Do not claim a mathematics-only proof can answer it. Closest results screened:

- [Trajectories of Self-Awareness Across the Alzheimer’s Disease Spectrum: A Systematic Review of Its Potential Contribution to Early Diagnosis](https://pubmed.ncbi.nlm.nih.gov/42739221/) (2026; DOI 10.3390/diagnostics16172791; complete PMC body retrieved in two offsets). Calls for standardized longitudinal multimodal studies to establish stage-specific trajectories and prognostic utility.
- [Metacognitive performance in Functional Cognitive Disorder (FCD): A meta-analysis](https://pubmed.ncbi.nlm.nih.gov/41428185/) (2026; DOI 10.1007/s13760-025-02969-8; PubMed abstract). Very few studies support impaired global but preserved local monitoring. The2019 request to first demonstrate a local deficit is not retained as an open target.

**Our operational target:** Preregister a longitudinal prediction estimand: incremental out-of-sample prediction of decline for a declared SCD population, horizon and baseline cognition/biomarker model after adding separately measured metacognitive bias, sensitivity and efficiency. Formalize assumptions for whether self/informant disagreement and trial-level confidence identify distinct quantities; compare against a null no-added-prediction model.

**Assumptions that must be exposed:** Declared instrument/task versions, confidence scale and scoring; Separate global appraisal, local performance monitoring, sensitivity, bias and efficiency; Stage/population, biomarker status and follow-up horizon fixed; Measurement invariance, missing follow-up, informant error and transport assumptions explicit.

**Data/source requirements:** Authorized longitudinal cohort with repeated cognition, confidence, informant reports and biomarkers; Consented public/controlled-access data with documented limits; Sufficient held-out follow-up events and external population validation.

**Reusable assets and their limits:**

- [Measurement.lean](https://github.com/Sodelin/Formalizing-Soft-Sciences/blob/4cf7366db359317e974416d81a0fe5d6aa258f6e/SocialScience/Measurement.lean): Elementary additive bias intervals only; no construct validity or fitted item model.
- [PredictiveState.lean](https://github.com/Sodelin/Work-on-Samuel-Alexander-Research-/blob/35570664221956edd153cceaa5351a9f7d63605f/research/open-problems/time-self-reference/predictive-memory/PredictiveState.lean): Exact behavioral equivalence across action words; reusable established abstraction substrate, not new psychology mechanism identification.

**Prior art to reuse:** Signal detection/meta-d′ measures, longitudinal prediction and model comparison are prior art; use existing instruments rather than inventing a generic Lean measure. Mathematical consistency or toy additive identification does not establish construct validity.

**Omnibus interface:** A measurement-and-prediction bridge connecting neurological biomarkers, psychological awareness, informant/social context and functional outcomes.

**What would count as a consequential output:** A source-linked measurement contract and falsifiable prospective validation protocol, followed by evaluated incremental prediction if data available; no diagnostic recommendation from current formalization.

**Lowest-cost next falsification:** Check whether an eligible open/authorized cohort jointly contains trial-level confidence, biomarkers and longitudinal endpoints. If not, mark dataset blocked and do not spend compute proving generic metacognition lemmas.

**Coverage limitation:** Recent PubMed search returned19 records, latest5 screened; fulltext2024 and2026 agenda reviewed. No exhaustive meta-analysis or external validation performed.

## How these questions connect to the theory

Nolan's distinction between discoverable questions and compatible hidden models is directly useful here. An added measurement can shrink the compatible model set without identifying the full mechanism. The relevant decision or prediction may nevertheless become identified. Conversely, a more precise questionnaire score or a reproduced behavior trajectory may leave the intervention-relevant alternatives unchanged.

Accordingly, every module should declare the actual observation channel, permitted interventions, and question-specific outcome. For PSY-1, the shadow is the measured symptom network; the desired answer is intervention ranking. For PSY-3, the shadow is the existing learning-task trajectory; the desired answer is delayed/new-context response. The intervention is useful only if it distinguishes those outcome-relevant alternatives. This is our operational synthesis, not a claim that the source authors endorsed Nolan's theory.

The repository's new decision-sufficiency direction, Ye/Amin/Özdağlar, *Learning Decision-Sufficient Representations for Linear Optimization*, arXiv:2603.18551v2, can be a mathematical bridge after its scope/current publication status is verified by the coordinating agent. It is not itself a clinical open problem and does not authorize a claim that psychotherapy learning is linear optimization.

## Search and evidence record

The machine-readable [PSYCHOLOGICAL.json](PSYCHOLOGICAL.json) contains exact queries, returned counts, continuation states, access manifest, assumptions, source commits and next investigations. Fifteen PubMed discovery/status probes plus one four-record identity pass were performed; this exceeds the initial approximate ten-query budget because two queries broadened unexpectedly and the metacognition status had materially changed. Five primary agenda texts were retrieved as complete PMC bodies, some in consecutive offsets. Selected later empirical papers and the FCD meta-analysis were screened at abstract level only.

The psychology-router skill and relevant clinical/computational lanes were applied. PubMed connector was successfully piloted before generic search. No APA PsycInfo entitlement was assumed. Two generic web discovery queries were noisy and contributed no load-bearing source.

Three important limits remain:

- This is a targeted source-linked catalog, not a systematic review or exhaustive priority claim.
- Zero search hits do not prove an open problem remains open. In particular, the known2025 CBT paper is absent from one exact latent-cause abstract query, demonstrating that query's incompleteness.
- Recent searches returned some future print-dated records. Those records were not used as dated closure evidence. Source identity was resolved for the load-bearing agenda papers; the2025 PMC record notes corrected publication, but correction details were not separately inspected.

No new proof, clinical result, outreach, submission or GitHub mutation was performed by this catalog author. A module can enter implementation only after a named investigator resolves its exact closest-work comparison and source-model mapping.

