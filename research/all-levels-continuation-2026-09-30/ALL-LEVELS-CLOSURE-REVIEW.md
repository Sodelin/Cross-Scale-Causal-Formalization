# All-levels closure review

Observed public Samuel repository main: e2502c82ab9a77c00543932f775a71e5374221f7.
Read-only review, 2026-09-30. No fresh finite execution or Lean build.

## Verdict

The currently published package presents a source-faithful computer-assisted proof of the original level-three circularity conjecture and of the whole-network extension of Theorem 4.7, strengthened to every finite reticulation level within the stated structural class. It is not merely a level-two Lean fragment. Conversely, the complete raw-source all-level theorem is not Lean checked, and this review does not supply external mathematical acceptance.

The final mathematical statement is original-NANUQ circular decomposability and exact equality of positive distance split support with the union of splits of displayed trees, for finite binary semi-directed LSA-rootable, outer-labeled planar, galled networks on at least four taxa. It permits arbitrarily many blobs and arbitrarily high finite reticulation level. Distinct displayed quartet topologies are deduplicated and averaged uniformly; switching multiplicities are not used as weights.

## Source correspondence

Primary paper opened independently: Holtgrefe et al., DOI 10.1007/s11538-025-01549-4.

- Definitions 2.1–2.4 establish the network class.
- Theorem 4.7 states circularity and exact displayed support for level-two bloblets.
- Section 6, final paragraphs, explicitly proposes extension to all level-two networks, circularity of level-three bloblets, and extension of some results to a parameterized distance family.
- Section 6 explains the whole-network result's inference value: obtaining the blob tree directly from distances rather than separately with TINNiK. It does not promise a new biological identifiability result.

The package's Theorem A answers the first two precisely and removes both the level bound and one-blob restriction. Theorem B gives a concrete affirmative answer to the existential parameter-family question, but not a maximal classification of all unweighted source-network distances.

## Actual proof and formalization boundaries

Authoritative current files: ALL-LEVEL-PROOF.md §§1–8, ALL-LEVEL-STRUCTURAL-AUDIT.md, ALL-LEVEL-COMPOSITION-AUDIT.md, ALL-LEVEL-SUPPORT-FINITE-AUDIT.md and ALL-LEVEL-SUPPORT-STRUCTURAL-AUDIT.md.

The proof has a structural paired-tip representation, six-label coefficient restriction, exact independently implemented finite certificate, all-level multi-blob composition, and exact support transfer. The composition audit specifically preserves uniform distinct-topology semantics and handles positive port masses and two-/three-port cases. The support audit accounts for bridges and zero-contribution two-port chains. These are mathematical arguments plus executable exact certificates, not a kernel-certified all-level graph theorem.

PUBLICATION-HANDOFF.md and OBLIGATIONS.md state that canonical theta endpoints and related algebra are Lean checked, but raw graph coverage, source conventions, circular ports and actual graph composition hypotheses remain formal obligations. Older ALL-LEVEL-QUALITY.md predates the later support strengthening; its prospective-support wording must not override the newer integrated proof and support audits.

FIVE-TAXON-THRESHOLD.md proves the sharp cutoff of five for universal parameterized anchor positivity, using the six-label structural reduction and equality of inequality catalogs. This is neither pointwise five-label compression nor a minimal witness bound for original fixed-score NANUQ. The exact anchor domain is s=o=1, 1/2<=a<=1, 0<=c<=a. Lean certifies the recorded inequality algebra; representation and enumeration completeness remain external computer-assisted ingredients.

## Further questions are extensions, not proof debts for the answered conjectures

- Maximal unweighted parameter circularity region; global parameter-family composition (the original identity fails unchanged for c>0); support and information-retention classification over that region.
- Sparse selectable query families with bounds and an output guarantee.
- Data-to-quartet estimation under a named evolutionary model and finite-sample uncertainty.
- Efficient recovery of an identifiable feature or quotient; all-level canonical form is not supplied by circularity alone.
- Complete Lean formalization of the source theorem.

The sharp raw-distance error promise below 1/2 and supplied-order boundary-quartet oracle corollary are already present. They do not constitute statistical sample complexity or order discovery. Dropping outer-labeled planarity is not a harmless strengthening: an admitted non-outer-labeled level-two example defeats exact support.

## Handoff readiness

The package can be sent as a transparent research proof packet for expert assessment and reuse in its exact scope; it need not become a complete inference system first. State computer-assisted status and full Lean boundary clearly. DELIVERY-RECEIPT.json records submission of checkpoint cba23504ec7c63936ab60e5c3beb65d296c2e9c5, successful hosted checks, queue title readback, and no curator acceptance or researcher email at that observation. Submission is not acceptance.

The coordinating agent independently reopened the primary publisher page before integrating this assessment.

## Preserve the existing live continuation

CONTINUE-RESEARCH.md explicitly preserves the active packet and bars replacing it with an unrelated search. research/continuation/NEXT-TASK.md names NANUQ-PARAMETER-GLOBAL-01: prove the whole candidate region s=o=1, 1/2<=a<=1, 0<=c<=a for the unweighted distance on arbitrary multi-blob source networks, or produce an exact source-admitted counterexample. If the whole region fails, preserve the obstruction and describe the largest region actually proved with unresolved portions explicit.

This is the natural first continuation within the NANUQ project. The existing theorem is independently publishable; this extension is not an unpaid proof obligation for its already answered conjectures. Failure of the old composition identity at c>0 does not establish failure of circularity. A negative individual anchor likewise does not establish a negative coefficient of the summed distance. Proving the whole supplied region would still not prove maximality beyond that region, which needs a separate necessity argument. One bounded decomposition/search pass is specified; no register-wide proof campaign or rerun of the Lean development is authorized by this packet alone.
