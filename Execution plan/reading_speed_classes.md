# Text classification (retired — see below)

> **This document was retired on 2026-07-31.** Its contents were split between the syllabus and
> `reading_practices.md`. The file is kept as a redirect because eight documents link to it.

*[Renamed 2026-07-14 from `text_classification.md`; retired 2026-07-31. Prose references to
"text_classification", "the classification master", or "reading speed classes" throughout the
documents mean the material now located as described below.]*

## Where its contents went

| What | Now lives in | Why |
|---|---|---|
| **Per-text classification** — which prose class each syllabus item is, with language, page count and section count | [sozialphilosophie_syllabus.md](sozialphilosophie_syllabus.md), as the `Lang` / `~pp.` / `Klasse` / `n_ch` columns in every module and appendix table | These are *intrinsic properties of a text*. They do not change when the endpoint, hour budget or importance tiering changes, so they belong next to the text itself. Keeping them in a parallel document keyed by the same item IDs guaranteed drift — and had produced it (see below). |
| **The classification framework** — the five prose classes, their pp/h rates, the indicative-author lists, the special rules, flag conventions, and the `n_chapters` convention | [reading_practices.md](reading_practices.md) § Appendix G | The framework is about *how you read*, and it is a canonical input. It cannot live in `execution_plan.md`, which is a derivative document — rebuilding the plan would destroy the rates. |
| **The hour formula and all derived hour figures** | [execution_plan.md](execution_plan.md) | Hours are derived — `f(pages, prose class, tier, α)` — and derived values should be computed, not stored. |

## Why the merge happened

An eight-lens audit of the syllabus on 2026-07-30 found that maintaining the same per-text facts
in two documents had produced measurable drift:

- **1.2** (*Rechtsphilosophie*, MUST-Anchor) carried ~430 pp. in the syllabus and ~320 pp. here —
  the §§34–141 promotion of 2026-05-29 never propagated. Its section count was likewise still 4
  rather than 5. This is an input to the hour formula for the single largest Part I text.
- **7.21** (Allen, *The Politics of Our Selves*) is MUST-class in `importance_tiers.md` but had no
  row here at all, so it could not be priced by the formula.
- **A.2.2, A.3.2, A.3.3, B.4.3, F.3.2, 6.9, W1.1** carried conflicting page counts between the two
  documents, in several cases with notes here arguing against syllabus figures that had since changed.

Separately, storing *derived* hour totals in the syllabus had let them drift from the syllabus's own
item rows by roughly a third (Part III alone by ~300 h), with four appendices carrying three
mutually inconsistent totals each. Removing the derived values removed the drift surface.

## Outstanding reconciliations

The merge preserved the syllabus figure wherever the two disagreed, and flagged the conflict rather
than silently picking a winner. These still need adjudication against the actual editions:

| Item | Syllabus | Former master | Resolution |
|---|---|---|---|
| A.2.2 Harding | ~180 pp. | ~30 pp. | **Syllabus correct.** The master's note complains the syllabus reads "~30" — it was corrected to ~180 afterwards and the master never caught up. Stale, not a conflict. |
| A.3.2 Shelby | ~25 pp. | ~180 pp. | **Syllabus correct.** Same pattern inverted: the master's note argues *against* a "~180" the syllabus no longer carries. It is a journal article. |
| A.3.3 Jaeggi | ~25 pp. | ~150 pp. | **Syllabus correct.** Master's own note says "~150 appears inflated for an essay". |
| B.4.3 Sugden | ~30 pp. | ~100 pp. | **Syllabus correct.** Master's own note: "likely error; treat as ~30". |
| F.3.2 Hodgson | ~25 pp. | ~150 pp. | **Syllabus correct.** Master's own note: "likely error; treat as ~30". |
| W1.1 Stahl | ~150 pp. | ~200 pp. | **Syllabus correct; ~200 dropped.** Verified against the Campus 2013 ToC (475 pp. total, main text to p. 458). The scheduled scope — §5.5 (29 pp.) + chs. 6–7 (44 pp.), with ch. 4 (65 pp.) and ch. 8 (33 pp.) "as needed" — gives ~73 pp. core, ~112 with ch. 8, ~177 with both. ~150 is a defensible with-as-needed figure; ~200 prices reading *all* of ch. 5, which is not what is scheduled. Method cross-check: the same arithmetic gives 8.8 (Einleitung + chs. 1–3) = 182 pp. against the syllabus's ~180. |
| 6.9 Bohman/Estlund/Floyd | ~120 pp. | ~100 (est) | **Both wrong — corrected to ~230.** Bohman 26 pp. + Estlund chs. 1–3 64 pp. + Floyd chs. 1–2 140 pp. Floyd alone exceeded the whole stated budget. `chapters` also corrected 3 → 6: the old figure counted *texts*, not scheduled sections. |

**A substantive flag raised while checking 6.9,** recorded in the syllabus row: the annotation promises Estlund's "epistemic proceduralism", but that is **ch. 6** — chs. 1–3 are the setup and chs. 4–5 build to it, so as scheduled the item does not reach the thing it is scheduled for. Either add ch. 6 or restate the rationale. A re-scope landing near the original budget: Bohman + Estlund chs. 1–2 + Floyd ch. 2 only (~132 pp.), and Floyd ch. 2 ("Diagnosis: Mentalism") *is* the meta-methodological challenge the note wants.

**All seven are resolved.** In every case the syllabus figure was the correct one and the former
master was stale — which is itself the argument for the merge: the drift ran one way, because the
syllabus was the document actually being edited.

## Classes assigned during the merge

Nine items had no prose class and so could not be priced by the formula. All are now classified:

| Item | Lang | Klasse | chapters | basis |
|---|---|---|---|---|
| 7.20 Pilapil | EN | Layered | 5 (est) | recognition-theoretic monograph in the Honneth/Taylor/Fraser register — anchors to Renault/Bedorf/Allen, not to the Analytic list |
| 7.21 Allen | EN | Layered | 4 | Allen is named in the Layered indicative list; propagated from the cross-listing at H.2.2, which already carried these values |
| 10.6 Hedström & Swedberg | EN | Analytic | 5 (est) | analytical-sociology volume; propagated from the cross-listing at B.1.3 |
| 15.8 Reckwitz | DE | Layered | 5 (est) | Reckwitz named in the Layered list. **chapters is a low-confidence estimate** — "selections" names no chapters; name them if the figure is to be load-bearing |
| C.1–C.5 | — | — | — | copied verbatim from 13.1–13.5, which carry identical titles, scope and page figures. The only differing column is the marker ([P]/[RS] vs **Marxist deepening**) |

The C.1–C.5 case is worth recording: they are **verbatim duplicates** of 13.1–13.5 with no scope
difference at all. That is the un-performed Module 13 / Appendix C extraction showing up as data.

## 1.7F — a real item with a missing row, now added

Listed here previously as an orphan. It is the opposite: the classification row was right and the
*syllabus* was missing the item. `execution_plan.md` schedules it (Kant→Khurana pre-block, M20–21,
opt-in, first cut at Layer 2); the changelog carried it through the 2026-07-14 renumbering as
1.6F → 1.7F; syllabus item I.1.7 names it as its downstream use; and 1.7 itself promised "the
substantive read is the 1.7F pre-block row below" — with no such row. The dangling pointer was the
defect. A row has been added to Module 1 with the classification recovered from this file's own
history: **DE · ~230 pp. · Systematic · 4 chapters** (Teil II = chs. III–V + *Schluss*).

Unscheduled Appendix I items legitimately carry no class: this document only ever covered
scheduled items.
