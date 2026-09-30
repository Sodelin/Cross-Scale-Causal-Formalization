# Repository roles and filing assessment

Read-only audit, 30 September 2026 UTC. This is a recommendation about ownership and navigation, not a migration or archival action. Fresh public default-branch trees and nine entrypoints were inspected. No private repository content was imported and no build was rerun.

## Verdict

The useful separation already exists, but navigation and status reconciliation are incomplete. **Cross-Scale should own the omnibus's question map and proposed interfaces; Formalizing Soft Sciences should own its implemented social/clinical formalizations; Mathematics of Psychology should preserve its earlier checkpoint.** Research Commons should route contributions and handoffs to those authorities. Keeping every repository as an independently evolving omnibus would create ambiguity.

| Repository and inspected commit | Observed contents | Recommended authoritative role |
|---|---|---|
| Cross-Scale Causal Formalization, `7f2a7eab62143487bb6a2d996234be5ebbab8b8f` | 28 files, including theory, three domain catalogs, source/status records and shared research map; no Lean files | Cross-domain scientific questions, theory interpretation, dependency/transfer map and current project navigation |
| Formalizing Soft Sciences, `7ed8634785b5568c1856ab4e9a29e4f83489a431` | 188 files, root SocialScience/Solidarity code, separate clinical package, project evidence, publications and audits; README reports 85 checked declarations | Implemented psychology/social modules, source correspondence, build receipts and scientific project publications |
| Mathematics of Psychology Formalized, `d75ec0ec75f5e21d112416b1524958f4885b5e10` | Eight files, one Lean source `Solidarity.lean`, receipt and explanatory documents | Preserved original solidarity checkpoint and historical entry point |
| Research Commons, `437462ace5fa237246f2dbc6e6767a9874d74214` | 22 files, captures, notes, sessions, handoffs, workflow and navigation | Durable attributed discussion, coordination and recovery links; not a second result ledger |

Counts exclude directory entries. They describe these snapshots, not completeness of the entire research program.

## Concrete defects

1. **The psychology navigation page is stale.** Soft Sciences `psychology/README.md` still describes the 27 September missing-corpus investigation and an import pending. Its root README and Psychology's result map now reconcile the recovered 67-item package and integrated 85 declarations. A distinct older corpus remains unresolved. These two histories must be separated rather than repeating “the corpus is missing.” The foundations README similarly retains the older recovery wording.
2. **The Psychology repository duplicates implementation rather than supplying additional results.** Its `Solidarity.lean` Git blob is exactly `992e225d3385e02ec74274aa656d34de34a4244f` in both repositories. Psychology already says the broader corpus is canonical in Soft Sciences and that its 16 declarations are included in the 85. This duplication is useful as provenance; two competing active development homes would not be useful.
3. **The omnibus catalog is now stronger than the outward navigation.** Cross-Scale has BIO/PSY/SOC catalogs; Soft Sciences' front page does not point to them. Research Commons' `projects.md` lists Cross-Scale and pins an older theory package, but omits Soft Sciences, the Psychology checkpoint and the new catalogs. Its text correctly tells readers to check current main.
4. **Discipline and implementation are mixed filing axes.** Soft Sciences has `psychology/` as an explanatory page but `clinical/` as an implementation package, and social implementation under root modules and `projects/`. Biology is a catalog here, not a biological implementation folder in Soft Sciences. Domain labels alone will not tell a contributor where to edit or which record determines current status.
5. **Dated copies need authority labels.** Theory/workflow analyses exist in Soft Sciences and as imported snapshots in Cross-Scale. The manifest preserves provenance; subsequent edits should say which current document supersedes a snapshot. Historical copies and publication production sources should remain historical, not receive synchronized edits by default.

## Smallest useful repair

Keep existing files and paths. Add an identical short repository-role table to the three front pages, linking the omnibus catalog, Soft Sciences' implementation/source audit, the historical Psychology receipt and Commons START-HERE. Update the stale psychology recovery text with the recovered-package distinction, retaining the earlier account as dated history.

Give each candidate **one stable question ID and one current status owner** in Cross-Scale; reference its exact implementation repository/path/commit rather than copying proof inventories. Domain tags may overlap: a biopsychology target can be tagged biological and psychological without duplicating its authoritative question record. Distinguish `question`, `implementation`, `source evidence`, `verification`, `historical snapshot` and `discussion` by purpose. For new work, a question page can link those locations before new folders are created.

Keep source-level project registers in Soft Sciences: they describe local model extensions and evidence requirements. Link them to omnibus IDs where correspondence is real. The omnibus should summarize status, not silently convert elementary local questions into externally posed open problems.

Update Commons navigation with these homes and a current catalog link. Preserve attributed notes and supersedes links; a session must retrieve a handoff and acknowledge/continue it. The inspected workflow explicitly installs no automatic cross-chat polling or delivery.

## Should Psychology become defunct?

**Supersede its standalone implementation role, not its historical value.** It contains a meaningful verified checkpoint, but no separate substantive corpus or clinical pipeline appears in the inspected main tree. Its present README already largely serves as a historical entry point. Make that role explicit and direct new implementation to Soft Sciences. There is no need to delete, move, archive or disable it now. Reconsider an active psychology home only if recovered distinct work or new substantive implementation warrants one; a title alone is insufficient.

Primary inspected entrypoints: [Cross-Scale README](https://github.com/Sodelin/Cross-Scale-Causal-Formalization/blob/7f2a7eab62143487bb6a2d996234be5ebbab8b8f/README.md), [Soft Sciences README](https://github.com/Sodelin/Formalizing-Soft-Sciences/blob/7ed8634785b5568c1856ab4e9a29e4f83489a431/README.md), [psychology page](https://github.com/Sodelin/Formalizing-Soft-Sciences/blob/7ed8634785b5568c1856ab4e9a29e4f83489a431/psychology/README.md), [Psychology result map](https://github.com/Sodelin/Mathematics-of-Psychology-Formalized/blob/d75ec0ec75f5e21d112416b1524958f4885b5e10/RESULTS-AND-SOURCE-QUESTIONS.md), [Commons workflow](https://github.com/Sodelin/Research-Commons/blob/437462ace5fa237246f2dbc6e6767a9874d74214/docs/WORKFLOW.md).
