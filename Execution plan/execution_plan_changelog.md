# Execution plan — changelog

History of substantive revisions to `execution_plan.md`. Companion to the plan itself; the plan describes the *current state*, this file describes *how it got there*.

Naming conventions used historically in the plan body:
- **Pass-N audit** = the Nth structured audit pass over the plan (e.g. coverage audit, feasibility audit). Each Pass-N reference in the plan body refers to a corresponding entry here.
- **Path D' / Option 3** = the M44-submission target schedule adopted 2026-05-19 after the Pass-4 feasibility audit (replaces the earlier M42-target path). All "post-Path-D'" annotations in the plan body refer to this commitment.
- **second-revision pass / third-revision pass** = revision passes on the syllabus (v5 → v5b → v6) whose item additions cascaded into the plan.

---

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
