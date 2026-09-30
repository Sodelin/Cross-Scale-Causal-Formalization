# Observability, reachable questions, and the response space

30 September 2026 UTC; the motivating message was sent 29 September Pacific. Nolan supplied the extension. The notation and elementary arguments below are the assistant's proposed interpretation. An independent mathematical review agent checked the distinctions; no Lean compiler or empirical model was run.

## The new claim

Nolan proposes that the shape of the candidate space depends on what is observable and retrievable, and that observations of a system's shadow can constrain predictions about the remaining structure. He also asks when reliable response is possible without direct access to the underlying concept, and how that relates to evidence-based practice.

The productive question is not a universal percentage of reality we must observe. It is: **Which observations distinguish the particular property we want, within which admitted models, and with what uncertainty?** This extends the target-generation theory while correcting an ambiguity in its use of C.

## Three spaces, rather than one ambiguous subset

Let T be the declared research-target space and C_A(D) its subset reachable by researcher/procedure A from evidence D, tools and budget. Reachability includes formulating or retrieving a question; it does not certify its truth or usefulness.

Separately let M be the admitted hidden-model class. For permitted probe p, let h_p(m) be the response predicted by model m. For exact data D consisting of pairs (p,y), define

$$V(D)=\{m\in M:\text{for every }(p,y)\in D,\ h_p(m)=y\}.$$

For target quantity q:M->Q define the compatible response space

$$R_q(D)=\{q(m):m\in V(D)\}.$$

These are different objects: reachable questions, compatible models, and compatible answers. Data can expand C_A(D) by revealing an unimagined question while shrinking V(D) by eliminating explanations. It can also leave either set unchanged. There is no general monotonicity theorem for actual human or model reachability; attention, tools, interpretation and memory matter.

The geometry or shape of C requires a specified structure on T, such as a partial order of generality or a graph of transformations. Cardinality alone does not express useful coverage. Calling a set objective does not validate its defining model class or measurement map. A measured response can be recorded reproducibly while its interpretation depends on assumptions; beliefs about T can contain testable claims rather than being purely subjective.

## What an observation update provably does

For a fixed class and calibrated exact observations,

$$V(D\cup\{(p,y)\})=V(D)\cap h_p^{-1}(y)\subseteq V(D).$$

Proof: satisfying all old constraints and the new one is exactly membership in the intersection. Strict shrinkage occurs precisely when an old compatible model predicts something other than y. An empty set flags inconsistency with the assumed class/maps/data; it does not mean a perfectly certain hidden object was recovered.

For nonempty compatible sets, R_q also cannot enlarge under this exact update. It need not shrink. The eliminated models may differ only on properties irrelevant to q. Thus 'observability updates meaningfully change inference' needs a target-specific condition: the new observation removes a formerly possible q-value, or changes a specified probability/decision sufficiently to matter. That is a proposition to establish, not an axiom to assume.

With explicit bounded errors, intersections of admissible measurement regions give a related constraint-set model. In probabilistic inference, updating a posterior is different: a redundant datum may add no information, posterior support can remain unchanged, and chosen credible regions need not nest. Changing the model class or recalibrating the lens can enlarge uncertainty. Do not transfer exact-set monotonicity to every statistical update.

## Reliable prediction without a unique hidden concept

When V(D) is nonempty, exact q-identification holds precisely when R_q(D) is a singleton. Multiple hidden models can therefore remain while agreeing about the requested outcome. Agreement about one q does not imply agreement about another property, a future intervention or a new context.

For approximate answers in a metric output space, an epsilon-accurate answer a requires d(a,q(m))<=epsilon for every compatible m. Response-set diameter at most 2 epsilon is necessary, by the triangle inequality. Diameter at most epsilon is sufficient by choosing any realized response as a. The gap depends on output geometry and available answers. This specifies an accuracy threshold relative to the target, rather than claiming a universal amount of observation.

This is a direct answer to the question about whether psychology works with concepts or shadows. Measurements constrain observable responses and specified latent targets under assumptions. A prediction can be dependable without identifying a unique latent mechanism. Stronger claims about what the concept really is need their own operationalization and identification evidence. This is a logical distinction, not a declaration that a particular psychological construct is unreal or already validated.

## When the whole shadow reconstructs the shape

A probe family P0 identifies hidden models up to a declared structural equivalence ~ when

$$[\forall p\in P_0,\ h_p(m)=h_p(m')]\Longrightarrow m\sim m'.$$

The entire permitted shadow is the collection of all permitted responses. If different models share it, observations identify at most their observational equivalence class. To recover more requires a separating measurement/intervention or a restriction on the admitted class. Shared observation is not itself a universal self-similarity claim.

In a finite class of N models, if each distinct pair is separable by a permitted probe, choose one separating probe per pair. The union has at most N(N-1)/2 probes and distinguishes every pair. This is a sufficient finite construction, not an optimal query bound. Without separation, unlimited data of the same permitted kind cannot establish the distinction. Existence of these probes does not guarantee efficient retrieval or selection.

For continuous models, exact identification needs suitable injectivity modulo the chosen equivalence; stable reconstruction from approximate or noisy observations additionally needs an appropriate stability condition. Evolving models require their dynamic and measurement assumptions to be declared. The existing [partial-views note](../partial-views-and-changing-systems.md) explains how a changing lens can be confused with a changing object. A notion of topological shape would additionally require a topology and an appropriate equivalence, rather than inferring it from a metaphor.

## Two discriminating examples

**Independent information versus repetition.** A hidden pair (x,y) has shadow s=x+y. Knowing s=1 leaves a line of possible pairs; repeating that exact reading supplies no new separating information. A second shadow d=x-y determines x=(s+d)/2 and y=(s-d)/2. Each coordinate error is at most epsilon if both measured shadows have absolute error at most epsilon. The gain comes from independent separating structure, not the number or percentage of readings. The first shadow already identifies the sum.

**Complete behavioral knowledge versus hidden structure.** Model A has one state and emits zero after every action. Model B has two states, alternates between them after every action, and always emits zero. Every permitted action/output sequence is identical. Future outputs are fully predictable, but state count is not identified. No additional output history resolves this unless the probe family or model assumptions change.

The second example refutes a universal claim that mapping all shadow interactions reconstructs the original object. It preserves the useful weaker claim that those interactions can define a complete behavioral abstraction for the specified probes.

## A better continuum than hard versus soft

Describe observability relative to a property, model class, probe family, context, error level and calibration stability. Add whether causal interventions are available and how difficult informative probes are to retrieve. Different targets within one field can occupy different positions.

Nolan's proposed curve—less direct observability produces greater reliance on indirect structure—is an empirical hypothesis. These dimensions make it testable without assigning each discipline one fixed hardness score. A mathematical proof gives a logical guarantee under definitions; empirical measurement requires a correspondence to the world. Neither by itself guarantees a complete model of the subject.

This note does not derive a cross-scale uncertainty principle from quantum uncertainty or establish that every observation must be imperfect. Exact observations can be useful idealized mathematical assumptions; physical accuracy and uncertainty are separate application-specific questions.

## Evidence-based practice and the level of claim

APA describes evidence-based psychological practice as combining research evidence with clinical expertise while considering the patient's characteristics, culture and preferences. See its [policy statement](https://www.apa.org/practice/guidelines/evidence-based-statement) and [task-force report](https://pubmed.ncbi.nlm.nih.gov/16719673/). This is a framework for informed clinical decisions, not a requirement that every underlying psychological mechanism be uniquely identified.

Our conceptual implication is that evidence for a decision/outcome and evidence for a unique mechanism are different targets. A supported intervention effect would not automatically establish a complete theory of why it works. Conversely, an elegant latent theory is insufficient evidence of beneficial outcomes. The reliability of any particular practice still requires its actual evidence, applicability and uncertainty to be assessed; no treatment recommendation follows from this note.

## Connection back to generative search

The discovery operation should ask which unresolved models disagree about the important response, then propose a probe or representation that separates that disagreement. It should also ask whether the newly revealed structure suggests a target outside current C_A(D). This generates a new question or investigation instead of merely confirming a completed checklist.

Useful formal work would instantiate a real model class, probe family and q, prove a separation or impossibility result, and compare attainable response uncertainty before and after a chosen observation. Elementary propositions above need no large foundation project. No novel theorem, universal reconstruction guarantee, empirical validation or Lean build is claimed.
