# Diagnostic Refinement Template

An iterative workflow for improving plans, syllabi, research designs, and other structured documents. Phase 0 (optional) marks scope. Phase 1 generates the evaluation dimensions. Phase 2 executes targeted revision passes.

---

## Phase 0: Scope Marking (optional; recommended for long or multi-stratum documents)

For execution plans, multi-year roadmaps, or any document with asymmetric resolution (e.g., week-level detail for year 1, month-level for years 2–3, log-only for year 4), mark each section before requesting a diagnostic:

- **Locked** — assumptions or content the diagnostic should not challenge. Saves the reviewer's effort for what's actually open.
- **Active** — under current revision; score and recommend freely.
- **Speculative** — low-confidence sketches. Score for direction, not for detail — a 2/5 here is not the same problem as a 2/5 in an Active section.

Include the markings inline (one-word tags at section headers) or as a preamble. Pass them through to Phase 1 in the prompt.

---

## Phase 1: Diagnostic Audit

Use this prompt **before any revision**. Paste your document below the prompt.

```
I have a draft [DOCUMENT TYPE] on [TOPIC/TITLE]. Before I revise it, I need a
structured diagnostic — not fixes, but an evaluation framework.

1. Identify the 6–8 most important evaluation dimensions for a document of this
   type, considering both the content domain and the artifact's practical purpose.
   Go beyond the obvious (e.g., "content completeness") to include dimensions that
   are commonly neglected for this document type.

2. For each dimension:
   - Define what "good" and "bad" look like on this dimension, with concrete
     indicators (not vague quality labels).
   - Score this draft on a 1–5 scale with a one-sentence justification. If the
     document has multiple resolution strata marked in Phase 0 (e.g., week-level
     vs. month-level vs. log-only), score each stratum separately — averaging
     across asymmetric resolution loses information.
   - Flag the weakness type:
     - **Structural** — requires reorganisation.
     - **Local** — fixable without changing the overall architecture.
     - **Calibration-dependent** — cannot be resolved by revision alone; depends
       on empirical input (e.g., actual pacing data, a checkpoint result). State
       the decision rule that would resolve it; do not revise it now.

3. Recommend a revision sequence: which dimensions should I address first, and why?
   Note any dependencies (e.g., "fixing X will invalidate your work on Y, so do X
   first").

4. The document likely encodes several design trade-offs the author has already
   made — sometimes explicitly, sometimes by omission. List the most consequential,
   state the author's apparent choice, and assess whether the choice is defensible
   given the stated goal. For each, name the evidence that would flip it. Then
   separately note any *unintended* tensions where improving one dimension would
   degrade another.

Here is the draft:

[PASTE DOCUMENT]
```

### What to do with the output

- Review the dimensions. Add any you think are missing, remove any that don't apply.
- Look at the scores. Dimensions scoring 4–5 probably don't need a revision pass.
- Follow the recommended revision sequence — structural before local, upstream before downstream.


---

## Phase 2: Targeted Revision Pass

Use one prompt per dimension. Work through them in the sequence recommended by Phase 1.

```
You are revising this [DOCUMENT TYPE] with a single focus: improving it on the
dimension of [DIMENSION NAME].

Context on this dimension: [paste the "good vs. bad" definition from Phase 1]

Current score: [X/5]. Key weakness identified: [paste the one-sentence
justification from Phase 1].

Constraints:
- Do not reorganise the overall structure unless the weakness is flagged as
  structural. If it is structural, propose the reorganisation explicitly before
  executing it so I can approve.
- Preserve prior revisions: [briefly note what earlier passes changed, if any].
- Where you face a trade-off with another dimension, flag it rather than silently
  resolving it.

Please produce:
1. The revised content. For documents under ~10 pages / ~5k tokens, return the
   full revised text. For larger documents, return **sectional patches**: for
   each section you change, give the exact section anchor (header) and the
   replacement text for that section. Leave untouched sections out. Do not
   silently revise sections outside the dimension's scope.
2. A brief changelog (5–10 lines max) listing what you changed and why.
3. If any cross-section references (a connection register, a milestone list, a
   glossary, a dependency table) depend on the sections you revised, flag them
   for follow-up even if you did not edit them.

Here is the current version:

[PASTE CURRENT DOCUMENT VERSION]
```

### Tips for Phase 2

- After each pass, re-score the target dimension yourself. If it hasn't improved enough, run the same pass again with more specific instructions.
- Every 2–3 passes, do a quick "regression check": skim the document for damage to dimensions you already fixed.
- For documents with cross-cutting infrastructure (connection registers, transition retreats, dependency tables, milestone lists), after each pass verify that the cross-references still resolve to the revised content. A retreat scheduled to consolidate Module 2 must still cover what Module 2 actually covers post-revision.
- Stop when you hit diminishing returns, not when every dimension is 5/5. Documents have trade-offs; a 4/5 across the board usually beats 5/5 on three dimensions and 2/5 on the rest.


---

## Phase 1 Variants for Common Document Types

These are starter dimension sets. Phase 1 will generate its own, but these help you
sanity-check the output and catch anything Claude missed.

### University Syllabus / Reading Course

| Dimension | What to look for |
|---|---|
| Intellectual narrative | Does the syllabus tell a *story* about the field, or is it a taxonomy? Is there a throughline students can articulate after week 2? |
| Progression logic | Does difficulty, abstraction, or methodological sophistication ramp intentionally? Are there plateaus for consolidation? |
| Motivation architecture | Early wins? Engaging material in the mid-course slump zone (weeks 5–8)? Does the final third feel like a payoff, not an appendix? |
| Canonical–contemporary balance | Can students see why the canon matters *through* the contemporary work, or are they separate blocks? |
| Discussion viability | Do sessions have enough interpretive tension to generate genuine debate? Are readings paired to create productive friction? |
| Workload calibration | Does per-week load account for text density differences? (e.g., 30pp of Rawls ≠ 30pp of a handbook chapter) |
| Assessment alignment | Do assignments actually test what the readings develop, or are they generic essay prompts? |
| Accessibility & logistics | Are texts available? Are prerequisites realistic? Is the schedule robust to a lost session? |

### Research Plan / Proposal

| Dimension | What to look for |
|---|---|
| Question precision | Is the research question specific enough to be falsifiable / answerable, or is it a topic area? |
| Identification / mechanism clarity | Is it clear *what variation* answers the question? For structural work: what is the key model mechanism, and is it disciplined by data? |
| Literature positioning | Does the plan make clear what gap it fills and why existing work doesn't fill it — without strawmanning? |
| Feasibility | Data availability, computational cost, timeline realism. For DSGE/structural: is the model tractable given the question? |
| Contribution calibration | Is the claimed contribution appropriately sized for the target outlet? Neither oversold nor buried. |
| Robustness strategy | What happens if the main result doesn't hold? Is there a Plan B, or does the project collapse? |
| Scope discipline | Is the project one paper or three? Are there "while we're at it" extensions that should be cut? |

### Project Plan / Work Plan

| Dimension | What to look for |
|---|---|
| Goal clarity | Are deliverables concrete and verifiable, or vague aspirations? |
| Dependency mapping | Are task dependencies explicit? Is the critical path identified? |
| Resource realism | Are time/budget/personnel estimates calibrated to actual capacity, or aspirational? |
| Risk identification | Are the top 3 risks named with mitigation strategies, or is the plan sunshine-only? |
| Milestone design | Are milestones genuine decision points (go/no-go, pivot) or just calendar dates? |
| Stakeholder alignment | Does the plan address what different stakeholders care about, or only the planner's perspective? |
| Feedback loops | When and how does the plan incorporate learning? Are there review points before it's too late to change course? |

### Long-Horizon Self-Directed Execution Plan

For multi-year personal roadmaps that combine a learning track with a downstream production goal (research output, publication, portfolio piece). Spans long enough that pacing and motivation are real constraints, not assumptions. Distinct from a syllabus (no learner other than the planner; no pedagogy), a research plan (the research is downstream, not the whole document), and a generic project plan (no team, no external stakeholders).

| Dimension | What to look for |
|---|---|
| Pacing realism | Are hours/week, pp/h, and tier overheads calibrated to *actual* capacity (day job, leave days, mid-week energy) or to the planner's best self? Are both bottom-of-range and midpoint scenarios load-tested? |
| Slippage resilience | Are falling-behind protocols mechanical (rule-bound, not vibes), and do they preserve the spine? Do cuts compose — what survives when the worst-case trigger fires? |
| Resolution calibration | Right detail at the right horizon. Is the near-term over-engineered (false precision)? Is the far-term under-specified at *decision points* that matter (module entries, transition retreats, go/no-go moments)? |
| Learning → production bridge | Do upstream learning modules deliver the specific cognitive inputs the downstream production phase requires? Or is the bridge assumed and the production phase under-staffed? |
| Long-horizon motivation architecture | Where are the dry stretches? Are checkpoints, retreats, and dialogue moments load-bearing (catch failure, force pivots) or decorative? Is there a checkpoint early enough to kill the plan if it should die? |
| Tier / cut discipline | Is the depth-vs-breadth trade-off explicit and recoverable — can you see what was cut and re-enter it later? Or is "Light tier" a euphemism for "I'll skim"? |
| Cross-cutting infrastructure | Do connection registers, retreat purposes, comprehension checks, and milestone lists each do specific work? Or are they ritual scaffolding that survives revision without being re-grounded? |
| External constraint integration | Day-job calendar, leave allowance, family/health robustness. Is the plan brittle to one bad month, or does it absorb shocks? |

### Policy Brief / Memo

| Dimension | What to look for |
|---|---|
| Decision relevance | Does every paragraph help the reader make a specific decision, or is there background filler? |
| Audience calibration | Is the technical depth matched to the reader? (A brief for a minister ≠ a brief for a technical committee.) |
| Argument structure | Is the logic: situation → complication → resolution? Or does it meander? |
| Evidence–assertion ratio | Are claims backed by evidence, or presented as self-evident? |
| Actionability | Are recommendations specific enough to act on, with clear ownership and timeline? |
| Counterargument handling | Are obvious objections anticipated, or will the reader think of them first? |
| Length discipline | Could this be 30% shorter without losing content? |


---

## Adapting This Template

**For new document types**: Run Phase 1 without the variant table. Claude will generate dimensions from scratch. Save good dimension sets here for reuse.

**For domain-specific depth**: Add a line to the Phase 1 prompt: "I work in [DOMAIN]. Weight your dimensions toward concerns specific to this field." For computational macro, this surfaces things like calibration credibility, computational feasibility, and identification-through-functional-form risks that generic prompts miss.

**For team use**: Run Phase 1 independently, then compare dimension sets. Disagreements about which dimensions matter are more productive than disagreements about specific edits.
