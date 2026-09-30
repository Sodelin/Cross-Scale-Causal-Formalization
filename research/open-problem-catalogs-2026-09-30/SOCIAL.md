# Social open-problem catalog

Assessment date: **2026-09-30**. Five source-backed candidate problems, with proposed omnibus contributions separated from what the sources already establish. **No entry is authorized here as a verified novel theorem target.** HOLD means the external question is real but the exact proposed subproblem needs a narrower novelty and current-status investigation before substantive implementation.

The existing social source-first gate rejected SP1–SP3 as matches to the elementary Lean corpus; this catalog preserves that conclusion. Budget feasibility, numerical connectedness and additive-bias intervals do not become solutions to bargaining, contagion or joint causal sensitivity because their terminology overlaps.

| ID | Externally posed problem | Proposed contribution | Status | Least costly decision |
|---|---|---|---|---|
| SOC-01 | Distinguish simple from complex contagion in empirical data | Observation-equivalence boundary and a separating observation/intervention specification | HOLD: existing classifiers overlap | Compare exact laws on small graphs against existing contagion definitions |
| SOC-02 | Sensitivity to simultaneous causal biases | Sharp direct/spillover-effect region with selection and outcome misclassification | HOLD: multiple-bias bounds already exist | Map one joint finite model to existing bounds before deriving anything |
| SOC-03 | Structural power rankings versus balanced bargaining payoff rankings | One precisely defined index: graph-class agreement and minimal separating examples | HOLD: exact index and closest theorem must be fixed | Compare index definitions and balanced-outcome solution sets |
| SOC-04 | Status expectation rankings versus Bayesian posterior rankings | Characterize when a signed path aggregation preserves ordinal conclusions | HOLD: source is explicit; scoped theorem and subsequent work unverified | Derive rankings on one shared-path graph under explicit priors |
| SOC-05 | Identify organizational-form recognition separately from resource congestion | Identification boundary and minimum measurement design for a joint event model | HOLD: assumptions and existing latent-event results unverified | Construct two mechanisms with equal density/event observations |

## SOC-01 — What observations distinguish contagion mechanisms?

**External source and locator.** Abiad et al., *Hypergraphs and simplicial complexes in focus: a roadmap for future research in higher-order interactions*, Journal of Physics: Complexity 7, 022501 (2026), DOI [10.1088/2632-072X/ae3c4e](https://doi.org/10.1088/2632-072X/ae3c4e), §6.1 final paragraph, printed p.25 (zero-based PDF page 24). The published [Cambridge PDF](https://api.repository.cam.ac.uk/server/api/core/bitstreams/7ade7c44-7d22-4a7c-bfc7-29310947cdd7/content#page=25) was accessible and the problem passage was read. This is an explicit empirical/methodological open challenge, not a named conjecture.

**Closest work, not a blank field.** Cencetti et al., PRL 130, 247401 (2023), and Contreras et al., PLOS Computational Biology 20, e1012206 (2024), are cited immediately by the roadmap. Shamsaddini et al., [arXiv:2505.00958v1](https://arxiv.org/html/2505.00958v1), already study an extended-persistent-homology classifier. Its abstract, models, results and discussion were read: contagion dynamics are simulated on empirical network structures. This prevents a first-discriminator claim. Its limited-observation performance is not a universal reconstruction theorem.

**Our proposed exact target.** Specify a known finite graph family, two competing stochastic transition-law classes, seed regime, observation channel and parameter ranges. Characterize when the classes produce overlapping laws of observed infection times, and which additional observation or controlled exposure separates them. A useful result must state failure cases as well as positive guarantees. It must transfer the separation through a stated observation channel rather than require access to the hidden infection history by assumption.

**Assumptions and significance.** Specify whether reinforcement permits below-threshold infection; otherwise the classes may become artificially easy to distinguish. Account for missing times, unknown contact edges and homophily, or explicitly delimit which of these are outside the theorem. A boundary tells researchers when a classifier's success can support a mechanism claim and when no classifier can resolve the question from the stipulated data.

**Omnibus interface.** Individual adoption states → interaction groups → partial event histories → mechanism-compatible set → intervention decision. Useful joint biological/social module; no claim that disease transmission and social reinforcement share identical laws.

**First discriminator.** Read the closest model definitions, write their exact observation laws on two to four nodes, and seek a nontrivial collision or a separation. Reject if the proposed statement follows directly from an existing identification result or merely recreates a classifier. Existing corpus match: none established.

## SOC-02 — Can jointly biased network effects receive sharp bounds?

**External source and locator.** Cinelli, Feller, Imbens, Kennedy, Magliacane and Zubizarreta, *Challenges in Statistics: A Dozen Challenges in Causality and Causal Inference*, [arXiv:2508.17099v1](https://arxiv.org/html/2508.17099v1#S3.SS6.SSS3), §3.6.3, “Other types of biases” and “Sharpness results.” Full text and those passages were accessible. The authors explicitly pose joint sensitivity to biases including interference; this is a methodological challenge.

**Closest work.** Smith, Mathur and VanderWeele, [*Multiple-bias sensitivity analysis using bounds*](https://arxiv.org/abs/2005.02908), DOI [10.1097/EDE.0000000000001380](https://doi.org/10.1097/EDE.0000000000001380), already combine confounding, selection and misclassification. The primary abstract was read; full-paper retrieval encountered a PMC challenge page. Any new work must compare its actual assumptions and estimand, rather than advertise multiple-bias analysis as new.

**Our proposed exact target.** For a fixed network exposure map and binary treatment/outcome model, characterize the sharp identified region for a specified direct or spillover contrast when outcome misclassification and selection depend jointly on exposure. An admissible result needs explicit sensitivity parameters, observed-data restrictions, a bound and compatible models attaining the bound. An additional analytic or computational gain beyond standard response-type enumeration is required before this qualifies as discovery work.

**Assumptions and significance.** Fix treatment assignment, cluster independence if used, positivity, which data are selected and error-rate constraints. Distinguish bias in recording peer exposure from bias in outcomes. Joint dependence can make applying isolated correction factors misleading. The intended contribution is an exact boundary under a defended model, not a generic warning that bias exists.

**Omnibus interface.** True individual/group outcomes → selection and measurement operators → observed sample → causal effect region. Reuses measurement concepts as vocabulary; current elementary bounded-bias intervals do not solve this target.

**First discriminator.** On one small cluster, align every variable and constraint with the existing multiple-bias framework. Check whether the candidate collapses to its known result. Only pursue a genuinely uncovered interaction of interference and measurement/selection; no novelty inferred from a search returning no hit.

## SOC-03 — When does a graph's power ranking predict bargaining outcomes?

**External source and locator.** Dimitri Volchenkov, *Mathematical Sociology: Models, Structures, and Open Problems*, Mathematics 14(18), 3363 (16 September 2026), DOI [10.3390/math14183363](https://doi.org/10.3390/math14183363), §3.4 concluding question. Publisher metadata was accessible through its indexed primary page, but direct HTML returned HTTP 429. The accessible [author preprint](https://www.preprints.org/manuscript/202608.0726), §3.4, states the question and definitions. Publication-version passage identity beyond the earlier gate was not independently re-audited.

**Closest work.** The source cites Braun and Gautschi (2006) and Kleinberg and Tardos, *Balanced Outcomes in Social Exchange Networks* (STOC 2008). The relevant bibliography and source discussion were read; original full-paper comparison remains required. Computing a balanced outcome is established prior work, not the proposed advance.

**Our proposed exact target.** Select one unambiguous version of the structural index (g), then characterize a graph class on which its strict rankings agree with the payoff ordering across balanced outcomes. Keep separate matching-conditioned agreement, existence of an agreeing outcome, and robust agreement across all maximum-weight matchings. For robust agreement, examine (\inf_{x\in\mathcal B(G)}(x_i-x_j)>0) when (g_i>g_j); require \(\mathcal B(G)\ne\varnothing\). Seek the smallest graph separating two agreement notions and certify minimality within an explicitly bounded class.

**Assumptions and significance.** Fix edge weights, permissible exchanges, outside options and the source's index normalization. Do not silently replace set-valued balanced outcomes by coordinatewise intervals. The scientific distinction is between structural power and realized bargaining power.

**Omnibus interface.** Exchange graph → structural index and bargaining mechanism → set of payoff outcomes → observed orderings. This is a precise transfer test between different “shadows” of the same graph.

**First discriminator.** Recover exact index definitions and the relevant existing class results before enumeration. Compare one known four-node experimental network and one graph with nonunique maximum matching. Current `two_person_budget_iff` has none of these objects and is not a partial solution.

## SOC-04 — Which status graphs preserve rankings under probabilistic interpretation?

**External source and locator.** Volchenkov's accessible author preprint, §3.5, the paragraphs following Proposition 1 and the concluding “Bridges” discussion. The source asks for graph/model conditions making expectation-score and posterior-log-odds rankings agree, including dependent relevance paths. This is an explicit mathematical reconstruction problem. Publisher full-text access and comprehensive subsequent-work search remain incomplete.

**Closest work.** The source gives the independent-path noisy-OR interpretation as Proposition 1, and cites expectation-states models by Berger and colleagues, Fişek et al. (1992), and empirical status-processing comparisons. These are prior art. Proposition 1 must be imported as a baseline; recreating independent noisy-OR is not a new answer. Bibliographic/source-level review only for the older papers.

**Our proposed exact target.** On a declared signed graph family with latent path activations, construct normalized positive/negative observation rules and explicit priors. Characterize when the source's expectation differences have the same signs as posterior-log-odds differences for every actor pair. Prove either an extension allowing a specified overlap pattern or a minimal ranking reversal showing the independent-path bridge's exact boundary.

**Assumptions and significance.** Specify shared causes and edge-transmission dependence, rather than call a path strength a probability. Fix priors and evidence conditions; free priors can destroy universal ordinal equivalence. A successful result would say which psychological/social ranking conclusions survive a probabilistic reformulation, and which empirical contrasts could distinguish the models.

**Omnibus interface.** Psychological expectations and evidence → signed interpersonal graph → probabilistic belief state → social influence ranking. Direct bridge to Nolan's question about what an observed shadow actually preserves.

**First discriminator.** Use one two-path graph sharing an edge and one edge-disjoint graph. Compute both rankings under the same stated evidence/prior model. If disagreement is a trivial free-prior artifact or the agreement follows from standard noisy-OR, redesign or reject. Existing Lean identity variables do not encode these probabilistic mechanisms.

## SOC-05 — Can recognition and competition be separately identified?

**External source and locator.** Volchenkov's accessible author preprint, §3.7 concluding two paragraphs. It explicitly requests a joint event model that distinguishes recognition from resource congestion despite endogenous organizational density. This is a methodological identification problem. The primary source was read; the exact narrow proposal's present open status is unverified.

**Closest work.** The source cites Hannan and Freeman's organizational ecology, Carroll and Hannan's density-dependent models and subsequent organizational-form work. Existing density/event models are baseline prior art. Their bibliography and source exposition were read; independent full-paper theorem comparison remains required.

**Our proposed exact target.** For a declared two-process marked birth/death model, derive necessary and sufficient observation or exclusion restrictions for separately identifying a recognition effect and a congestion effect. Begin with a constructive nonidentification pair matching available density and event histories. Add a specified recognition measure or defended source of variation and derive what is newly identified. A worthwhile extension gives a minimal measurement design or a sharp partially identified region, not another regression of survival on density.

**Assumptions and significance.** Fix the evolution and measurement laws for both latent processes, intensity positivity, risk sets, temporal resolution and which covariates influence both processes. Regulatory change is not an instrument without an exclusion argument. The result could explain why identical organizational counts support different explanations and what extra observations could resolve them.

**Omnibus interface.** Individual/organizational decisions → population event process → recognition/resource latent states → public counts → intervention estimand. The observation contract can share abstractions with biology and psychology while preserving separate substantive semantics.

**First discriminator.** Determine whether the candidate is just a standard latent-state identifiability theorem in new vocabulary. A small observation-equivalent pair may help define the target, but that familiar fact alone is not discovery closure. Continue only with a source-linked unaddressed measurement or process restriction.

## Cross-scale lead that must be treated as prior art

Cinelli et al. §3.9.3 also explicitly treats knowledge elicitation as a search problem. However [da Silva et al., *Expert-Aided Causal Discovery of Ancestral Graphs*, arXiv:2309.12032v4](https://arxiv.org/abs/2309.12032v4) (6 March 2026) already addresses uncertain expert feedback under latent confounding; its primary abstract was checked. Thus Nolan's proposed task-representation intervention should be compared to this work before claiming a new elicitation method. The catalog does not add a sixth target or treat generic multi-agent checking as a solution.

## Search and access record

Ten targeted queries were issued: three source-title searches; four verification/closest-work searches; three narrowing searches. Both search systems were used. Several restrictive system-1 queries returned irrelevant results; those results establish nothing. Direct source retrieval then verified the three prior gate leads and found two additional questions in the author preprint. Closest work was followed from source citations and a retrieved primary preprint. The machine-readable file preserves the exact queries, primary URLs, locators, access boundaries and decision status.

This is a bounded source-and-prior-art assessment through 2026-09-30, not an exhaustive proof that every target remains unsolved. Source freshness makes an explicit challenge credible as a lead; it does not establish the novelty of our narrowed proposal. Catalog inclusion supports investigation, not a submission or a claim of open-problem closure.
