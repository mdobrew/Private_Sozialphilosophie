# Session state — 2026-05-24

> **Staleness note (2026-05-28):** This snapshot predates the M44→M48 submission-target rebuild and the file reorganisation. For current programme parameters, trust `execution_plan.md` and `execution_plan_changelog.md`; for current file layout, trust the live folder. Sections below were updated only for file-reference accuracy, not for substantive programme state.

Captures load-bearing decisions and conventions across the working session. Read on resume.

## Programme-level conventions

- **Submission target:** M44 (Jan 2030) baseline; M46 (Mar 2030) W13-trigger fallback. *M44 is a soft motivational anchor — if scope × capacity arithmetic requires extending the timeline, extend rather than overcommit weekly hours.*
- **Calendar anchor:** M1 W1 = week of 2026-06-15.
- **Naming:** Phases I/II/III/IV (Roman); programme months M1–M44+; programme weeks W1–W57+. Phase 0 renamed to Part 0. v5 → v6 syllabus identifier renumbering complete.
- **Reader profile:** computational macroeconomist at ECB Frankfurt; fluent German; ~7–8 h/week + project-allocated ~7–8 leave days/year (out of 30 total) + dedicated leave-week ~30h/year. Capacity ceiling ~346 h/year → ~1,269h over 44 months.

## Document architecture (5 core files; bridge as 6th specification doc)

| File | Role |
|---|---|
| `sozialphilosophie_syllabus.md` | Intellectual map. Annotated bibliography with tags, hour estimates, [Economist's note] markers, "Marxist deepening" labels (formerly [MX], retired 2026-07-14). |
| `programme_parameters.md` | Programme-level spec. Reader profile, capacity envelope, community engagement track, design requirements, Class A/B/C parameter version-control. **Slimmed 2026-05-24** — obsolete sections deleted; load-bearing canonical content kept. |
| `importance_tiers.md` (v2.1) | Importance overlay. MUST-Anchor / MUST-Engage / SHOULD / COULD / DISCRETIONARY classification. (Prior v1.3 archived at `archive/superseded/y3_critical_path_v1.3.md`.) |
| `reading_speed_classes.md` | Prose-class master mapping (5 classes × language × n_chapters). |
| `execution_plan.md` | Schedule. Phase I weekly, Phase II–III monthly. Inventory tables with Pages, Hrs, Tier annotations. |
| `reading_practices.md` | Method. Practices A–J + Discipline + Using Claude + Note-taking infrastructure + Appendix C §C.2 Style × Tier matrix (canonical) + §C.3 practices defined elsewhere. |
| `diagnostic_refinement_template.md` | Meta-workflow for revising the above (Phase 0 scope marking → diagnostic audit → revision passes). |

Companion files:
- `execution_plan_changelog.md` — revision history
- `archive/superseded/` — prior doc versions (v5 syllabus, v1.3 critical path, pre-rebuild execution-plan + bridge snapshots, renumbering bridge)
- `archive/audits/` — retained audit reports (05-22 to 05-25 batch); the 05-19/05-20 batch and spent agent prompts were deleted in the 2026-05-28 cleanup

## Importance + tier framework (canonical structure)

### Phase III importance classes (per `importance_tiers.md` §2.1, refined in v1.3 + v2)

| Class | Criterion | Default tier |
|---|---|---|
| **MUST-Anchor** | Apparatus the user will reconstruct in his own voice for the Phase III piece | Full |
| **MUST-Engage** | Reviewer-expected coverage; cite/characterise; no apparatus-reuse | Light (Orientation if [O*]/[O]/[RS]) |
| **SHOULD** | Supports Phase III directly but publication could proceed without | Light if [P]/[ES]; Orientation if [O*]/[O]/[RS] |
| **COULD** | Conditional — relevant only if Phase III topic commits to specific terrain | Orientation; upgrade via §4 trigger |
| **DISCRETIONARY** | Intellectually interesting; not Phase III-load-bearing | Skip / Phase IV |

MUST = `(reviewer-essential) ∨ (tradition-anchoring)` disjunction. The Anchor/Engage split tracks *which* criterion drives.

### Style × Tier matrix (canonical in `reading_practices.md` Appendix C §C.2 + mirrored in `execution_plan.md` Appendix A)

**Formula:** `Hrs = (Pages ÷ pp/h) + min(Reading × α, n_chapters × per-Recon ceiling)`

**5 prose-difficulty classes** (decoupled from syllabus tags):

| Class | DE pp/h | EN pp/h | Examples |
|---|---|---|---|
| Dense | 5 (bottom) | 6 (bottom) | Hegel, Adorno DdA/MM, Marx Kapital, Lukács, Mannheim, Weber methodological essays, Horkheimer 1937 |
| Systematic | 8 | 10 | Habermas (TKH, EuI), Gadamer, Forst monographs, Honneth monographs, Khurana, Postone |
| Layered | 10 | 13 | Honneth essays, Jaeggi, Celikates, Rosa, Stahl, Joas, Renault |
| Analytic | 15 | 18 | Forst articles, Fricker, Fraser articles, Zurn, Laitinen-Särkelä, Taylor, Mead, Woodward, Hollis |
| Transparent | 18 | 20 | Neuhouser, McCarthy, Outhwaite, Feenberg, Dewey, Polanyi, Streeck, Heinrich, Pippin |

**Writing α** (per hour of reading): Dense 1.0 Full / 0.4 Light; Systematic 0.5 / 0.2; Layered 0.4 / 0.15; Analytic 0.3 / 0.12; Transparent 0.3 / 0.12. **Per-Recon ceiling**: Full 2h, Light 0.75h.

**Special rules**:
- **Honneth-monograph decouple**: read at Systematic pp/h, write at Layered α.
- **Aphoristic flag**: MM aphorisms + Benjamin Theses stay Dense pp/h; `n_chapters` = thematic clusters of ~5–8.
- α covers body draft + closing sentence + empirical-presuppositions + Konzepte updates + re-read during writing. C1 separately scheduled (~30 min/Full text).

### Tier-derivation rule

Inventory tier = `(Phase III class × syllabus tag) → tier`, Phase III class dominant. Tag-only default mapping in execution_plan Appendix A is a fallback. Deviations annotated `[tag] → ExecutedTier (per Phase III ...)`.

## Reconstruction count convention

**Per-chapter / per-major-section.** Full tier = 500–800w per chapter; Light tier = 150–250w per chapter. Module deliverables list one checkbox per text with explicit Recon count + brief author/title. Reading rows imply the Recon work; no separate 📝 Schedule rows except major Full-tier filings.

**Aphoristic n_chapters convention**: thematic clusters of ~5–8 aphorisms.

Phase I = 25 Full + 46 Light = 71 chapter/section Recons. Phase II ≈ 55 Full + 67 Light = ~122. Phase III = uses Phase I/II Recon corpus, no new chapter-level Recons.

## Community engagement (bridge §2.4, revised 2026-05-24 per two audits)

**Reframed goal**: become an interdisciplinary outsider-insider in the Frankfurt-tradition conversation — *not* an academic insider. Signal a non-standard profile (ECB economist with strong quantitative training + serious Sozialphilosophie self-study + open to collaboration). **M44 is the first visible move, not the destination.** Phase IV is where the signal compounds into participation.

**Activity rebalance (per audit 2)** — current track was "competently designed for the wrong goal":
- **Vorlesung attendance**: downgraded from central activity to "attend selectively when topic aligns" — Gasthörer status is invisible and doesn't compound relationships
- **Public events**: reframed — every event must produce one post-event interaction; "places to start one conversation"
- **Book review submission** (M24–M26, ~20–25h) — kept. *And* cross-disciplinary short essay (Soziopolis / Geschichte der Gegenwart / Mittelweg 36) on the methodological intersection — likely arises naturally from Skizze/Anwendung work
- **ECB-hosted scholar talk** (M22–M25): kept as aspirational reminder — *if feasible*, single highest-leverage move (Herzog/Beckert/Stahl/Hartmann/Jaeggi to speak at ECB DG-R). Realisability uncertain; not treated as an active to-do
- **Discussant role at a workshop** (M20–M30): added — easier to land than speaker slots; "ECB economist on financial-stability-meets-Frankfurt-tradition" is the hook
- **Scholar emails** (Phase III, ~3–4 spread): kept with higher bar — substantive question about *their* work; younger-to-mid-career scholars (Jütten, Vogelmann, Loick, von Redecker) higher-yield than senior (Forst). Philosophy/Sozialphilosophie field is *more permissive* than econ for cold emails from substantive interlocutors
- **Informal presentation** (M37–M39): reframed for feedback quality, not stakes-gradation. FAPTF or private session with 2–3 scholars
- **What's NOT in the plan**: ECB-internal talk *by the user* as rehearsal (considered and dropped). The ECB *hosting* of a scholar is structurally different and aspirational

**Phase IV long-game**:
- **Standing referee work**: realistic at M50–M60+ (after M44 publication). Editor adds user to journal reviewer database; asked for reviews on topics adjacent to published topic-niche. Philosophy is typically single-blind (editor sees reviewer, author doesn't). Sign up to ORCID + journal databases at M44.
- **Co-authored piece** at methodological intersection: realistic flag at M50–M54, after M44 piece in review/published. Likely targets: Jütten, Herzog, Vogelmann. Venues: *European Journal of Social Theory*, *Journal of Economic Methodology*
- **Co-organised workshop**: realistic flag at M60–M72. Theme: "Normative Reconstruction and Macroeconomic Method"
- **Recurring ECB-hosted format** if M22–M25 worked; visiting-fellow arrangements at IfS/ConTrust/MPIfG; one short essay/year sustaining "in the conversation" status

**Interlocutor list** (Phase II–III contact targets, prioritised):
- *Top first-contacts*: Herzog (Groningen), Beckert (MPIfG), Hartmann (Luzern), Jütten (Essex — already in syllabus 7.22, was 8.10!)
- *Strong with caveats*: Stahl (Groningen), Jaeggi (HU Berlin), Forst (Goethe — topic-conditional), Celikates (FU Berlin — runs FAPTF)
- *Younger generation*: Vogelmann (Bremen), von Redecker (Berlin), Loick (Amsterdam)
- *NOT contacted*: Honneth himself (high downside cold-email)

## Hallucination flag

The first community-engagement audit invented `critical-theory.net` as a venue. The site does not exist. All audit reports going forward should be briefed with anti-hallucination warnings + asked to flag uncertainty rather than fabricate. Verified-real venues: *Soziopolis*, *Geschichte der Gegenwart*, *Mittelweg 36*, *WestEnd*, *DZfPh*, *Constellations*, *Philosophy & Social Criticism*, FAPTF, IfS, ConTrust, MPIfG.

## Audits run this session — load-bearing findings

- **Pass E (style × tier allocation)** — earlier in session. Output: Phase I Hrs largely match plan, Phase II Module 7 +57% above plan due to per-chapter Recon convention, +120h Phase II structural.
- **Other-practice budget audit (Agent C earlier)** — ~+107–138h non-Recon adjustments needed: Practice E synthesis notes (~23h), Practice F named re-reads (~22h), Phase III bumps (~35–60h), R3 raise, Skizze raise, W3.3 raise. Currently deferred to schedule-rebuild agent.
- **Phase III importance audit (2026-05-22)** — produced v1.3 framework (MUST-Anchor / MUST-Engage sub-split, Phase III-dominant tier-derivation, §4 dependency table restructured with class-change/tier-change columns). Saved at `agent_audits/y3_importance_audit_2026-05-22.md`.
- **Community engagement audits (2× 2026-05-22 and 2026-05-23)**: first audit was helpful but invented `critical-theory.net`. Second audit (independent, briefed with reframed goal + anti-hallucination warning) substantially superseded the first — reframed plan as "competently designed for the wrong goal." Both saved at `agent_audits/community_engagement_audit_2026-05-22.md` + `_2_2026-05-23.md`.
- **Bridge Class A/B/C audit (Agent B 2026-05-22)** — Capacity ceiling re-computed (~1,269h at 44m baseline vs ~1,524h scheduled load → ~20% overage, not previously asserted 13%). User decision deferred to schedule-rebuild. Class B refreshed with 7 new entries (Style × Tier matrix, Honneth decouple, aphoristic flag, MUST sub-split, tier-derivation rule, doc architecture, naming + calendar). M44 promoted from Class C to Class A.
- **Bridge §3.4 falling-behind redundancy audit** — 98% duplicate of execution_plan §A. Deleted; "schedule slippage → motivational collapse" sentence migrated to bridge §5 (Key Tensions).
- **Cut-list review** — saved as `cut_list_review_2026-05-22.md`. Triggered by Phase II inflation; reviews existing 5-layer cut schema. Pending integration in schedule-rebuild.

## Saved agent prompts (for fresh-agent launch)

Both saved prompts below have been **run and deleted** in the 2026-05-28 cleanup:
- `y3_reclassification_v6.md` — produced `importance_tiers.md` (v2).
- `schedule_rebuild.md` — produced the M48 schedule rebuild now reflected in `execution_plan.md`.

## Open decisions queued

- **Capacity-ceiling overage**: 1,524h scheduled vs 1,269h capacity at 44m → ~20%. Deferred to schedule-rebuild agent — it will surface concretely.
- **Community engagement Phase III activities** — substantive recommendations from audit 2 need application to execution_plan.md (the schedule). Bridge §2.4 framing done; operational details for schedule-rebuild agent.

## Next steps (recommended order)

1. **Launch `agent_prompts/schedule_rebuild.md`** in a fresh agent session. This is the big pass that: (a) recomputes Schedule Hrs from new Inventory + ground-up; (b) reconciles Inventory Tier-column annotations against importance_tiers.md; (c) layers in non-Recon practice adjustments (Practice E, F, R3 raise, Skizze raise, W3.3 raise, etc.); (d) layers in community-engagement audit 2 recommendations into Phase II + Phase III schedule sections; (e) makes the M44 vs M46 timeline call honestly. ~2000-word report expected. Schedule-rebuild prompt already updated to handle all of this.

2. **After schedule-rebuild lands and is reviewed**: any small refinements + final cross-document consistency check.

3. **Documentation hygiene**: any further file deletions (e.g., is `renumbering_bridge.md` still needed?), session_state refresh.

## Conventions for next session

- **Terse responses. Decisions over prose. Tables for option-presentation. Cite file:line.**
- **When the user proposes a structural change, sketch lightly first, surface implications, get confirmation, then execute.** Avoid early commitment.
- **Three-agent parallel pattern works**: read-only audits in parallel for cross-check; user reviews and decides.
- **Anti-hallucination discipline**: warn agents explicitly; ask them to flag uncertainty rather than fabricate venue/author/affiliation details.

## Decisions taken on user's behalf this session

- Slimmed programme_parameters.md drastically — deleted §2.2 + §2.3 + §3.4 + §3.5 + §3.6 (merged into §2.4) + §5 + §7. Renumbered. Refreshed §6 (was §8) with audit B recommendations.
- Applied community-engagement audit 2 framing + user-specific choices to bridge §2.4 (drop ECB-internal-talk-by-user; keep ECB-hosting as aspiration; book review + short essay both; discussant role with how-to-arrange; scholar emails kept with high bar + clearer norms; Phase IV referee-work realistic framing; co-authoring M50–M54 flag; workshop organising M60–M72 flag).
- Updated reading_practices cross-references to point at new Style × Tier matrix locations (replacing obsolete bridge §2.2 + §3.5 refs).
- Saved both community-engagement audits + Phase III audit + Class A/B/C audit + falling-behind audit to `agent_audits/`.
