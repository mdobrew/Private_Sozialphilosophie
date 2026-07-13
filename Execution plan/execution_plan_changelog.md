# Execution plan — changelog

History of substantive revisions to `execution_plan.md`. Companion to the plan itself; the plan describes the *current state*, this file describes *how it got there*.

Naming conventions used historically in the plan body:
- **Pass-N audit** = the Nth structured audit pass over the plan (e.g. coverage audit, feasibility audit). Each Pass-N reference in the plan body refers to a corresponding entry here.
- **Path D' / Option 3** = the M44-submission target schedule adopted 2026-05-19 after the Pass-4 feasibility audit (replaces the earlier M42-target path). All "post-Path-D'" annotations in the plan body refer to this commitment.
- **second-revision pass / third-revision pass** = revision passes on the syllabus (v5 → v5b → v6) whose item additions cascaded into the plan.

---

## 2026-07-12 — Khurana 1.6 *Teil* correction + Kant→Khurana Module 7 pre-block

Corrected a part-boundary error for Thomas Khurana, *Das Leben der Freiheit* (Suhrkamp, 2017), and restructured its placement. Verified the ToC against the Suhrkamp and CUP (English ed., *The Life of Freedom in Kant and Hegel*, 2026) previews: the book is two roughly equal parts — **Teil I = Kant** (*Die Form der Freiheit*; *Die Wirklichkeit der Freiheit*; ~200 pp) and **Teil II = Hegel** (chs. III *Geist und Natur*, IV *Die Freiheit des Lebens*, V *Das Leben der Freiheit* + *Schluss*; ~212 pp). The syllabus/plan reading "Introduction + Part I (chs. on Hegelian life)" was self-contradictory — the Hegelian reconstruction is **Teil II**; Teil I is the Kant setup — and the "~150 pp" figure fit neither whole part.

- **Syllabus 1.6** → *Einleitung* (Module 1, orientation, ~2–3h) + **Teil II** deferred (~230 pp / ~14–18h); "Part I" corrected to Teil II; forward cross-ref repointed to the Module 7 pre-block and Kant prereqs I.1.5/I.1.7. Module 1 total reduced to 92–153h (Khurana now ~2–3h in-module, down from ~8–12h).
- **Syllabus Appendix I.1** → added **I.1.7** *KU* teleology §§64–66 (the life-analogy Kant, previously absent everywhere; [P], ~4–6h). Baked in the self-standing analysis (the *Grundlegung* reads largely alone; only its *Dritter Abschnitt* — and the whole *KpV* — presuppose the *KrV*). Added **→ Connects** flags to the practical/teleological rows (Grundlegung → RP §§105–141 + Forst 7.7/7.10 + Habermas *Diskursethik*; *KU* → Khurana 1.6 + Hegel's *Leben*/Karen Ng + naturalism 8.12). Renumbered guides to I.1.8–10; hour-budget row 80–120 → 84–126 with the "practical strand separable, not front-loaded" note.
- **Execution plan** → Module 1 1.6 reduced to *Einleitung* only (W18, ~2–3h). Added an opt-in **Kant→Khurana pre-block** at the head of Module 7 (M20–21, before 7.5/7.7): *Grundlegung* (I.1.5) + *KU* teleology (I.1.7) + Khurana *Teil II* (1.6F), ~26–34h. Rationale: read the Kant-dependent reconstruction just-in-time, where it also serves Forst's Kantian constructivism (7.7/7.10) and Honneth's *RdF* (7.5), rather than cold in Module 1 — and *not* inside the calibrated Phase I hours (the plan already defers even §§105–141 out of Phase I).
- **Baseline hours unchanged.** Pre-block is opt-in/conditional (Hegelian-freedom or Kantian-constructivism track), Layer-2 first cut, consistent with the §§34–141 opt-in handling; the *Grundlegung* is Layer-2-**retained** since it also underwrites Forst 7.7.
- **Not done:** the generated `print-syllabus/` export is now stale (still holds the pre-correction Appendix I.1 table and 1.6 entry); regenerate before any print use.

## 2026-07-12 — Stahl 8.8 / W1.1 chapter correction (Teil boundary)

Corrected a chapter miscount for Titus Stahl, *Immanente Kritik* (2013). Verified the ToC against the Campus publisher preview: the book is 476 pp; **Teil I = chs. 1–3 (pp. 19–190)**; **Teil II opens with ch. 4** (Kollektive Intentionalität, p. 191). The syllabus/plan reading "chs. 1–4 (~200 pp)" was internally inconsistent — chs. 1–4 run to p. 255 (~247 pp); the "~200 pp" figure matches chs. 1–3 (~180 pp incl. Einleitung).

- **Syllabus 8.8** → chs. 1–3 (Teil I), ~180 pp, 10–13 h. Descriptor rewritten: Teil I is Stahl-the-cartographer (taxonomy of critique; hermeneutic critics; §3.1 Habermas / §3.2 recognition / §3.4 the sozialontological questions). His own positive theory (recognition model of social normativity, ch. 5 §5.5; practice-theoretic account of immanent critique, chs. 6–8) flagged as Teil II–III, read in the Craft Block.
- **Syllabus W1.1** → retargeted from "chs. 1–4" (which duplicated 8.8) to **Teil II–III core** (ch. 5 §5.5 + chs. 6–7; ch. 4 ontology / ch. 8 *Verdinglichung* as needed). Removes the redundant re-read of Teil I; matches the entry's stated "how to do it" purpose.
- **Execution plan** (Module 8 summary; M26 schedule; 8.8 inventory row; placement note; reconstruction checklist; W1.1 Craft-Block note; Layer-3 trim): core read set to **chs. 1–3**, ~18 h; **ch. 5 added as optional** (+~120 pp / +~10 h) with the note that ch. 5, esp. §5.5, holds Stahl's own view — take it up in Module 8 if the immanent-critique track is live, else it moves to W1.1. Layer-3 trim target changed from "chs. 1–2" to "ch. 2 (hermeneutic survey)". Net Module 8 core load ~−5 h (23 → 18); within tolerance, module total unchanged.

## 2026-06-29 — New `field_map.md`; phase3 §4 endpoint-branch map; branch B + E readings folded in

Outcome of a multi-turn "spines" conversation (which intellectual lineages the programme runs on; which to specialize in).

**New document — `field_map.md`.** The navigational layer: spine definition (spine/track/coverage, lens-vs-field); the six spines + the rival-paradigm distinction; a cross-cutting names index; venues-by-spine; methods (oppose/combine); a live frontier-debate register. Indexes the syllabus by *lineage* rather than module. Not one of the original 8 core docs — added by user request to hold the "where am I in the field / what are my options" layer.

**phase3 §4 endpoint-branch map.** Added a branch table (A–F) at the head of §4's conditional promotions, tying each branch to its spine/method, §4 promotions, syllabus additions, and venue. Keepers flagged: **B (capitalism-as-form), E (Bildung)**.

**Branch B readings → syllabus + text_classification + phase3.** Module 13: 13.6 Sohn-Rethel *Intellectual and Manual Labour* [MX/P], 13.7 Arthur *The New Dialectic and Marx's Capital* [MX/RS], 13.8 Bonefeld *Critical Theory and the Critique of Political Economy* [MX/RS]. Module 14: 14.13 Engster *Das Geld als Maß, Mittel und Methode* [MX/RS], 14.14 Lapavitsas *Profiting Without Producing* [MX/RS], 14.15 Jaeggi & Loick (eds.) *Nach Marx* [MX/ES]. phase3: SHOULD/COULD-conditional (branch B); Sohn-Rethel and the Engster/Lapavitsas pair carry the economist-wedge [Economist's note]s.

**Branch E readings → Appendix H.** H.1.8 Layton *Toward a Social Psychoanalysis* [RS], H.1.9 Ikäheimo *Recognition and the Human Life-Form* [RS], H.3.6 Winker *Care Revolution* [RS]. Appendix H total ~230–320h → ~255–350h. (Keystone Bildung primary Heydorn H.6.2 was already on the syllabus.)

**text_classification housekeeping.** Backfilled 14.11 Mau + 14.12 Castel (present in syllabus/phase3 but absent here) + rows for all nine new items.

**Baseline schedule unchanged.** All branch-B/E additions are conditional (fire only when the branch commits at R5 ~M35), not baseline-active — so execution_plan scheduled hours are untouched, consistent with prior conditional-addition handling. Branches C, D, F stay map-only in `field_map.md` until chosen.

**Citation caveats** carried into `field_map.md` for verification before any enters a written bibliography (Sohn-Rethel edition; Honneth *Kritik der Macht* date; Saar English-translation status; Kurz anchor; Finlayson title; Habermas vol. 2 English; German Pädagogik specifics).

## 2026-06-27 — Part-0 orientation review: six literature additions + appendix prefix cleanup

Triggered by a Part-0 reading review (Honneth, "Pathologien des Sozialen" 0.2) surfacing texts absent from the syllabus.

**Catalogue additions (`sozialphilosophie_syllabus.md`).** Six texts: **4.12** Freud *Das Unbehagen in der Kultur* [P]; **4.13** Nietzsche *Zur Genealogie der Moral* I–II [RS]; **7.14** Taylor "The Politics of Recognition" [P] (reuses the slot vacated 2026-05-29 by Allen & Mendieta → 8.13 — the documented 7.14 gap is now closed); and three Freudo-Marxist primaries making Appendix H.1 load-bearing — **H.1.5** Marcuse *Eros and Civilization* [P], **H.1.6** Fromm *Escape from Freedom* [P], **H.1.7** Mitscherlich *Auf dem Weg zur vaterlosen Gesellschaft* [RS]. Module 4 total 99–139h → 111–155h; Appendix H total ~200–280h → ~230–320h.

**Derived docs updated.** `text_classification.md` — 6 new rows (+ backfilled the missing 4.11 Adorno *Drei Studien*), indicative-author list, two borderline notes. `phase3_critical_path.md` — 4.12 SHOULD/Light, 4.13 COULD/Orientation, 7.14 MUST-Engage/Light; Appendix H.1 row expanded; new §4 "Psychoanalytic substrate / authoritarian character" promotion row; §3.0c change-log subsection (version stays v2.1).

**Appendix prefix cleanup (`sozialphilosophie_syllabus.md`).** Fixed a systematic off-by-one rename artifact in Appendices A–H: stale item-prefixes in F/G/H prose normalised to each appendix's letter; mislabeled footer totals corrected (A, D, E, F, G) and one duplicate removed; Appendix D self-references (D.0 recommendation, [Note on D.2.3]) and Appendix G's "[NE] in its entirety" self-reference fixed; inbound cross-refs repaired (Module 4 *Halbbildung* → H.6.1; Appendix C items C.16/C.17 "[H cross-reference]"). Flagged but not changed: two pre-existing numeric mismatches (Appendix E header ~180–250h vs footer ~170–240h; Appendix F/G "beyond Module 16/17" mapping).

**Execution plan (`execution_plan.md`): applied 2026-06-27 per user go-ahead.** Freud 4.12 entered as an **active Light** read in Module 4, W35–36, before 4.2 *DdA* (Module 4 ~70h → ~77h; Phase I total ~486h → ~493h; Phase I Light Recons 38 → 39). Taylor 7.14 entered as an **active Light** read in the Module 7 window alongside 7.3/7.4 (Module 7 ~162h → ~167h; Phase II total ~720h → ~725h; flagged first-cut under falling-behind given the Module-7 capacity overage). Nietzsche 4.13 carried as an **optional early-read flag** (W37–38, ~6–8h from headroom), not in baseline totals — mirrors the *Negative Dialektik* early-read flag. Marcuse/Fromm/Mitscherlich H.1.5–7 remain Phase-IV/appendix, scheduled only on the §4 psychoanalytic-substrate trigger.

## 2026-05-29 — Item relocation: Jütten/Neuhouser → Module 7; Allen & Mendieta → Module 8

Three items were filed under the wrong module (flagged by the user); corrected by content. Renumbering used next-free slots — documented gaps left at 7.14 / 8.10 / 8.11, no cascade renumber:

- **8.10 Jütten**, "Is the Market a Sphere of Social Freedom?" → **7.22** (it assesses Honneth's *Recht der Freiheit*, a Module 7 text).
- **8.11 Neuhouser**, "Honneth's Theory of Social Freedom" → **7.23** (a Honneth-method critique).
- **7.14 Allen & Mendieta**, *…The Critical Theory of Rahel Jaeggi* → **8.13** (a volume on Jaeggi, a Module 8 figure).

**Catalogue vs. schedule.** Module/catalogue assignment was corrected in the catalogue documents (`sozialphilosophie_syllabus.md` Modules 7/8 rows + both economist's notes + 7.20 cross-ref + module totals; `text_classification.md`; `phase3_critical_path.md` Module 7/8 sub-tables + v2.1 change-log lines). In `execution_plan.md`, 7.22/7.23 were **rescheduled** to the Module 7 reading window (M24, right after 7.5 *Markt*) so that catalogue and schedule agree (per user follow-up the same day; M8 month-rows, inventory, deliverables, and at-a-glance updated accordingly — M24 ~25h→~29h, M29 ~30h→~26h); 8.13 remains the M7-window opt-in bonus.

**Hour shift.** Module 7 ≈ −5h net (loses Allen/Mendieta 12–18h; gains Jütten+Neuhouser 8–13h); Module 8 ≈ +5h net (mirror). Syllabus headline module totals updated (M7 → 197–265; M8 → 134–186). Baseline scheduled hours unchanged (all three are bonus / Layer-2–3 / conditional, not baseline-active). `print/` per-section splits regenerated to match.

## 2026-05-21 — Practice A redesign + tier-system reconciliation

Outcome of two audits (tier-system consistency + Practice A redesign) and the user's design decisions:

**Tier system — three-document reconciliation:**
- `reading_practices.md` Practice A line 67 was 2-tier ({P, ES} vs {O, RS}). `bridge_document.md` §2.2 was 3-tier (Full / Light / Orientation). Reconciled to 3-tier throughout via a new "When and at what depth" subsection in Practice A. Mapping: [P\*]/[ES\*] → Full (per chapter, 500–800 w, four-part + closing sentence + empirical-presupp sub-heading + 2–3 C1 questions); [P]/[ES] → Light (per text, 200–300 w, two parts: claim + directed-against); [O\*]/[O]/[RS] → Orientation (no filed reconstruction; 1–2 sentence reading-log line); [NE] → out of scope.
- Default tag → tier mapping is canonical in Practice A. Plan deviations are flagged in the Inventory column as `[tag] → Tier (rationale)` (e.g., `[P] → Full (upgraded; load-bearing for Module 7)` for 1.3 Phänomenologie).
- `bridge_document.md` §2.2 updated to include ES\* under Full, to specify per-text (Light) vs per-chapter (Full), and to specify "reading-log line per text" rather than "no written output" for Orientation.

**Policy decision — explicit scheduling.** Every text whose tier specifies a filed note appears as an explicit row in the Schedule's Output column. No more silent folding of Light notes into the W17/W25/W28-etc. comprehension checks. Documented in Practice A "When and at what depth" + reading_practices §L.12 step 8 (workflow check before module-close artifacts).

**Plan-level fixes from the tier-consistency audit:**
- 1.3 Hegel Phänomenologie IV.A: upgraded [P] → Full (was previously [P] with no filed reconstruction — silent-consolidation case). Full reconstruction now filed at W16 (Recon #3). Re-read at Module 7 as textual ancestor of *Kampf um Anerkennung*. Cascaded Recon numbering: ÖpM W21 → #4, Horkheimer W36 → #5, Dewey W44 → #6, McCarthy W48 → #7. Phase I production budget: 6 → 7 Full reconstructions.
- 5.4 Gadamer ([RS]): user decision to keep syllabus tag as [RS]. Under the new default mapping [RS] → Orientation → no filed reconstruction. W49 Light note dropped; Inventory tier annotated `[RS] → Orientation`. The substantive Gadamer-vs-Habermas work remains in W50 (5.5 Habermas Light note) and the module-close comprehension check.
- 0.4 Jay ([O]): W7 Light note dropped per the new default mapping ([O] → Orientation = no filed reconstruction). Reading-log line replaces it; pre-retreat draft absorbs the substantive observation.

**Other Practice A edits applied:**
- Heading rewritten to "Practice A: Written argument reconstruction (Full and Light tiers; Orientation tier reads without a filed note)".
- Per-part demarcation cues added inline to claim / support / directed-against / presuppositions to pre-empt the most common confusions (especially (ii)–(iv) conflation: support is what the author *gives*; presupposition is what they *do not* and *need*).
- Closing forward-looking sentence marked Full-required, Light-optional.
- K-Use-1 cross-reference added in both directions (Practice A → Practice K, Practice K → Practice A).
- Time-allocation rule of thumb: per-tier writing-minute breakdown (Full ~20–30 min/h, Light ~10–15 min/h, Orientation ~0 min/h filed); explicit note that per-author multipliers describe input cost (time per page read) and are independent of the output-tier choice.
- §L.12 step 8 (typical workflow): added "confirm every text read during the module has its filed output before module-close artifacts" check to close the silent-consolidation loophole at the workflow level.
- Execution plan Appendix A reformatted to show per-text format alongside the multiplier, plus the default tag → tier mapping rule as a footer.

**Bridge §2.2 updated** to match.

**Pass B prompt (queued separately):** the deferred module-restructure pass should now incorporate the concrete tier-deviation list from the tier-consistency audit (4A.2 Joas mistag, 1.2 RP mistag, 2.2a Kapital promotion question, plus the systematic "Inventory says Light, Schedule omits Light note" pattern for Phänomenologie [resolved here], Pollock, Lukács 3A.1, Feenberg, Benjamin Theses, Kunstwerk, Kapital 2.2b).

---

## 2026-05-20 — v6 syllabus alignment

- Renamed the syllabus "Phase 0" to "Part 0" to remove terminological collision with programme Phases I–IV. The execution plan was already using "Part 0".
- Applied v5 → v6 identifier renumbering throughout the plan: Module 7 cascade (Forst 7.8a/b → 7.9/7.10, Benjamin → 7.11, Fraser PS → 7.12, Renault → 7.13, Allen-Mendieta → 7.14, Bedorf → 7.17, Honneth *Anerkennung* → 7.18, Honneth *Arbeitende Souverän* → 7.19); Pollock 4.2a → 4.3; K.x Part VI items → Module 14 items 14.x / Appendix D items D.x; Module 12 (Phil. Soc. Sci.) → Module 10; 12A–D (rival paradigms) → 11A–D; Module 13 (Political Philosophy) → Module 12; Mills 13.6 → 12.6; new Module 13 (Marxist Foundations) absorbs former Appendix F.1–F.5; Module 14 (Capitalism as Social Form) absorbs former Part VI essentials; Appendix F → Appendix C, Appendix G → Appendix H; Craft Block C1/C2/C3 → W1/W2/W3 and item C3.1/C3.2/C3.3 → W3.1/W3.2/W3.3.
- Removed the inline Mermaid Temporal DAG (a separate visual is in progress).
- TOC labels updated to match renamed sections.

## 2026-05-19 — Third-revision pass (audit-driven syllabus additions)

Honneth 7.19 *Der arbeitende Souverän* (2023), Forst 7.10 *The Noumenal Republic* (2024), and Jaeggi 8.12 *Fortschritt und Regression* (2023) added to the syllabus as SHOULD-by-default per `phase3_critical_path.md`; conditional-MUST at M30 R5 if Phase III commits to corresponding terrain. The plan absorbs these as Phase III frontier-reading candidates (M37–M39), not Phase II baseline.

## 2026-05-19 — Path D' Option 3 commitment (Pass-4 feasibility audit)

The plan was previously calibrated to an M42 journal-submission target. Pass-4 feasibility audit concluded that the Phase II load (Module 7 Honneth/Forst/Fraser at peak; M27 close-month overload) was structurally extreme and that ~150h of relief was achievable by:
1. Deferring 5 SHOULDs to Phase IV baseline: Vogelmann 9.6, Boltanski *On Critique* 9.7, Harding 9.9, Aglietta (former K.6b → Module 14 item 14.9), Bedorf 7.17. Plus Renault 7.13 (Phase IV default; Phase II-bonus opt-in only).
2. Reducing Module 7 Full reconstructions from 5 to 3 (RdF method + Forst-vs-Honneth → Light methodological summaries).
3. Splitting Honneth 7.18 (was 7.17) *Anerkennung* (2018): partial Light Phase II (~15h) + conditional Full Phase III frontier completion (~25h).
4. Demoting Skizze #5 to [BONUS — opt-in].
5. Forward-shifting Polanyi (CL5) from M27 to M25 to smooth M27 overload.

These were originally documented as "Path D' Option 3" choices and are now plan baseline. Submission target: M44 (Jan 2030).

## 2026-05-18 — Second-revision pass

Plan revised against the second-revised syllabus and the new `phase3_critical_path.md` companion document (MUST / SHOULD / COULD / DISCRETIONARY classification).

Net additions:
- Phase I: Module 1.6 Khurana [O]; Module 4.3 Pollock [ES].
- Phase II: Module 7.9 Forst *Normativity and Power* + Module 7.18 Honneth *Anerkennung* (2018); Module 9.6–9.10 standpoint epistemology cluster + Vogelmann + Boltanski *On Critique*; new Module 8A "Außereuropäische Kritik" (Phase II close / Phase III early); Context Layer #6 Aglietta (alongside Streeck/Polanyi).

Discipline: most additions read at Light or Orientation tier to preserve the bridge §8 fixed parameters. Phase II absorbs ~+80–100h over the previous plan; the cut strategy informed Pass-4 and the subsequent Path D' commitment above.

## 2026-05-19 — Pass-6 audit (G1 cadence taper)

G1 light-discrimination practice tapered from "every module" to: every module M1–M6 (Phase I); alternating modules M7–M14 (Phase II); ad-hoc Phase III. Rationale: the external→internal translation move consolidates by ~Module 7. Documented in `reading_practices.md` §G1 and in the §E.2 module-close checklist.

## 2026-05-19 — Pass-7 coverage audit (E.1 / E.2 protocols)

Added two canonical protocols to the front matter:
- **E.1 Reconstruction-week protocol** — applies to every 📝 Full reconstruction week. Five steps: Practice A reconstruction, closing-sentence record, G2 component (ii) empirical-presuppositions inline, C1 seminar questions, K-Use-1 cross-reference check (W5 only).
- **E.2 Module-close checklist** — applies to every module close. Comprehension check + DM + G1 + C1 tally + C2 cross-thinker question + Practice D debate-map + negative-space note + QM (where applicable).

Phase I gross load addition ~16–20h, offset by ~10–15h bonus-cut buffer; net ~0–5h overage within tolerance.

## 2026-05-19 — Pass-10 audit (back-fill and leave-booking)

- C.IX Régulation-school deepening + Module 8.x Stahl absorption + Phase IV register additions (Operaismo, Analytical Marxism, Eco-Marxism, Régulation).
- Added §D.1.b: Leave-booking lead-time for Writing Blocks W1 (M36 = May 2029, pre-book by Feb 2029) / W2 (M43 = Dec 2029, pre-book by Sep 2029) + family/health-shock softening (graded re-entry rules for 2–4 / 4–8 / 8–16 / >16 week absences).
- Added §D.2 Calibration-Trigger Response Annex: if W13 trigger fires + capacity steady-state, accept cascade to M46 submission target rather than compress Phase III phases. Pre-committed decision.

---

## Open cleanup items (deferred)

The following bulk-cleanup passes are queued for separate execution:

1. **Tag-stripping pass.** Remove inline "Pass-N audit", "Path D' Option 3", "post-Path-D'", "second-revision", "third-revision" annotations from the plan body where their role is reader-facing breadcrumbs rather than active decision-points. This file is the authoritative log for that history; tags in the plan body are redundant once it exists.
2. **Bridge §X.Y / phase3_critical_path §N footnoting pass.** Cross-references currently appear inline ~50× and slow reading. Convert to numbered footnotes or a single Cross-References appendix.
3. **Schedule-table redesign pass.** Migrate all Phase I module schedule tables from `| Wk | Type | Core reading | Hrs | Output | Close items |` to per-item rows `| Wk | Activities | Pages | Hrs |` (one item per row, empty Wk on continuation). Drop Type and Close-items columns. See module-structure prompt in conversation history.
4. **Module-structure pass.** Reorder module sections to: Schedule → Inventory → Deliverables (checklist) → Capability targets → Why this matters → Phase IV connections. Delete redundant "Module arc" subsections. Standardise Inventory tier column to {Full, Light, Orientation, Bonus}.
