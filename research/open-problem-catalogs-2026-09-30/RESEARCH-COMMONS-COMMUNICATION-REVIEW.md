# Research Commons: durable communication review

Reviewed 2026-09-30 UTC. This is a bounded companion to the biological, psychological, and social open-problem catalogs. No workplace redesign or repository mutation was performed during this review.

## Finding

The two repositories are the right kind of substrate for communication that survives a chat: a contributor can publish a record, and another contributor can retrieve it later. During this review, the public builder advanced from a single checkpoint to a usable notebook with an entry point, project index, templates, handoffs, and workflow. Retrieval and continuation are now explicitly designed. The remaining question is whether **recorded work leads to acknowledgment and correct resumed action** in practice; that has not been demonstrated by this review.

The public checkpoint identifies session `2026-09-30-commons-builder`, contributor Codex, and the planned workspace. Its formerly future `START-HERE.md` is now published. These records support a commons-builder session, not a particular model or live presence. The new entry point explicitly states that cross-chat polling and delivery have not been installed. [C1, C3]

## Inspected coverage

| Surface | Observation | Limit |
|---|---|---|
| `Sodelin/Research-Commons` | Initial snapshot `995780b72a082a0b17ca8001f94512f11127e84c` had one checkpoint; recheck `8e48183a2634463cb7fe5f2b871b45f9151d7ede` contains the entry point, workflow, templates, notes, and handoff | Entry point and workflow read at the newer version; other new files inventoried, not exhaustively audited |
| `Sodelin/Research-Commons-Private` | Exact private repository and authenticated file access confirmed | Private content is not reproduced here; no complete private tree audit was performed |
| Issues in both repositories | Scoped issue search returned no results | An empty result does not prove that no coordination exists elsewhere |
| Other chats | No arbitrary chat history was available to this review | Repository access and scoped agent messaging do not imply access to every conversation |

The private `README.md` request returned 404, but a subsequent authenticated known-path file read succeeded. This was not a general access failure. Eight initial reads/searches plus three public freshness checks were used.

## Existing coverage and useful extensions

| Need | Current coverage or extension | Why it matters |
|---|---|---|
| Discover the work | Present: entry point directs readers to project and handoff links | A record must be findable |
| Remember exchanges | Present: attributed session IDs and contribution files; extension: explicit parent and response references | Preserve which answer addressed which question |
| Resume correctly | Present: checkpoint, artifact retrieval, uncertainty, and next-action workflow; test recovery of exact target and obstruction | Preserve the research frontier, not just deliverables |
| Confirm receipt | Extension: recipient response identifies handoff and version read | Publication does not establish understanding |
| Coordinate ownership | Present: indexes explicitly are not locks or live rosters; optional bounded assignments when duplication becomes material | Avoid stale reservations and presence claims |
| Preserve disagreement | Present: separate critiques and superseding entries retain earlier claims | Recover rejected assumptions and rationale |
| Separate public/private | Repositories exist; promotion rules not assessed in the two newly read public documents | Avoid silently copying private conversation |
| Avoid overwrite | Present: unique files, fresh index reads, additive rebuild after non-force push conflict | Preserve concurrent contributors' work |

The builder's workflow already addresses meaningful capture, attribution, recovery, concurrency, and disagreement. The proposed extensions address delivery semantics, not a checklist declaring research complete. Acknowledgment does not certify a theorem or problem importance. [C4]

## Practical use and evaluation

Treat the commons as a mailbox plus an index. Git supplies durable versions; the contributor's workflow supplies reading and responding. In this environment, scoped collaboration messages can coordinate active agents directly. Across separate chats, a published repository handoff can bridge the gap only when the receiving chat actually retrieves it. Autonomous notification or polling requires an available scheduling/integration mechanism; repository creation alone does not provide it. Retrieved records change the available context, not the model's weights.

The cheapest useful trial is a two-session handoff on one real catalog question. Session A publishes its source locator, current target, decisive unresolved assumption, and a message requesting one bounded comparison. Session B starts from the index, retrieves the cited versions, states what remains unknown, performs the comparison, and responds to the message ID. Check whether B recovered the intended question without Nolan repeating it, avoided duplicating completed work, and distinguished established results from proposals. Log elapsed work and actual usage only where measured. This trial tests continuity and research usefulness together.

Recommendation: use the published entry point to run that trial now. Keep domain evidence and proofs authoritative in their project repositories; use the commons to route questions, discussion, and handoffs across them.

## Sources

- **C1:** [Public setup checkpoint at inspected commit](https://github.com/Sodelin/Research-Commons/blob/995780b72a082a0b17ca8001f94512f11127e84c/sessions/2026-09-30-commons-builder/0001-start.md).
- **C2:** [Public commit](https://github.com/Sodelin/Research-Commons/commit/995780b72a082a0b17ca8001f94512f11127e84c). Public recursive tree and scoped issues were inspected through the GitHub connector; private verification supplied access status only to this report.
- **C3:** [Published entry point](https://github.com/Sodelin/Research-Commons/blob/8e48183a2634463cb7fe5f2b871b45f9151d7ede/START-HERE.md).
- **C4:** [Published workflow](https://github.com/Sodelin/Research-Commons/blob/8e48183a2634463cb7fe5f2b871b45f9151d7ede/docs/WORKFLOW.md).
