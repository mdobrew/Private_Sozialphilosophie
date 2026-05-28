# Inventory Mispricing Audit — execution_plan_v1.md

**Date:** 2026-05-25
**File audited (read-only):** `/Users/michael/Sozialphilosophie/Execution plan/execution_plan_v1.md`, cross-referenced against `reading_practices_v4.md` §C.2 (Style × Tier matrix), `text_classification.md`, `sozialphilosophie_syllabus_v6.md`.
**Purpose:** Identify Inv-cell mispricings of the same character as the Celikates 0.1 *Einführung* case (Layered pp/h applied to a text that does not itself read at Layered density). Top-N list for user review.

---

## Framework validation (Celikates 0.1)

Celikates & Jaeggi *Einführung* re-pricing (25→15h) confirms the diagnostic class. The misprice arose because `text_classification.md` assigned **Layered** based on the authors' typical register, but an Einführung *about* Layered authors reads at Transparent/Systematic speed (~17 pp/h, not ~10 pp/h). Re-priced Inv: 250pp ÷ ~17 pp/h ≈ 14.7h + 0.25h flat Orient writing ≈ 15h. Schedule W1–W4 already allocates ~16h, so the Inv was internally inconsistent with the Schedule and is now aligned.

## Audit method

Walked every Inventory row in Modules 0–10 + Module 8A, computing the formula `Reading hours = Pages ÷ pp/h(class, lang)` plus tier-appropriate writing α, with cap min(α×R, n_chapters × ceiling). Compared each Inv cell against (a) the formula output given the assigned class, (b) the Schedule allocation where extractable, and (c) the syllabus v6 per-text estimate where given.

**Headline finding.** After the 0.1 Celikates and 1.6 Khurana repairs (2026-05-25), the remaining Inv cells are tightly aligned with the C.2 formula. Most "suspect" items (Outhwaite, McCarthy, Freyenhagen, Heinrich, Hollis, Streeck) are already correctly classified as Transparent / Analytic, not Layered, so no Celikates-style propagation exists. The framework picks up the obvious cases by design. The remaining over-pricings are small (3–8h each), borderline (class boundaries between Layered/Analytic/Transparent), and several require user-side reading-experience judgement to confirm.

## Top candidates ranked by likely Δ saved

| Rank | v6 ID | Text | Module | Inv Hrs | Schedule Hrs | Syllabus Hrs | Suggested Hrs | Δ saved | Diagnosis |
|---|---|---|---|---|---|---|---|---|---|
| 1 | 0.1 | Celikates & Jaeggi *Einführung* | Part 0 | ~15 (was ~25) | W1–4 ~16 | 12–15 | ~15 | — (already saved 10h) | **Class mismatch (RESOLVED)**: Einführung *about* Layered authors does not read at Layered density. Anchor case for the framework. |
| 2 | 8.5 | Jaeggi & Fraser, *Capitalism: A Conversation* | M8 | ~21.5 | n/a — embedded in M24–25 rows | 15–20 | ~17 | ~4–5 | **Class mismatch (low–med confidence)**: dialogue / Q&A format reads faster than Layered EN. Inv exceeds syllabus high end (20h). Re-pricing to ~13 pp/h with looser α gives ~17h. User should confirm against own pace on dialogue volumes. |
| 3 | 9.10 | Collins, *Black Feminist Thought* (selection Intro + chs. 1, 5, 11) | M9 | ~13.5 | n/a — embedded in M27 row | 10–12 | ~9–10 | ~3–4 | **Class mismatch (low confidence)**: Collins's prose is widely described as accessible-pedagogical; partial selection from a clear monograph. Currently classed Layered EN @13 pp/h; functional pace likely closer to Transparent EN @20 pp/h. Inv slightly exceeds syllabus high end (12h). User should verify. |
| 4 | 5.4 | Gadamer, *Wahrheit und Methode* Part II (selections) | M5 | ~16.5 | W48–49 ~10 active reading | 15–20 | ~15 | ~1.5 | **Tier-effect over-pricing**: tier is Orientation per Inv but Inv includes more than the flat-0.25h writing the matrix prescribes for Orient. 120pp Systematic DE @8 pp/h = 15h + 0.25h flat = ~15.25h. Inv carries ~1.25h surplus, plausibly to cover Gadamer's actual prose difficulty (borderline Dense). Confidence low — could equally be defended as honest mid-band pricing. |
| 5 | 10.1 | Hollis, *Philosophy of Social Science* | M10 | ~12.5 | n/a — embedded in M26–27 | (covered by survey) | ~11 | ~1.5 | **Class mismatch (low confidence)**: textbook, deliberately transparent register. Currently Analytic EN @18 pp/h = 11.1h + 0.12α writing = 12.4h. If re-priced Transparent EN @20 pp/h = 10h + 0.12α = 11.2h. Marginal; classification.md's "Hollis = Analytic textbook" call is defensible. |

**No further high-confidence over-pricings identified.** All active Inv rows in Modules 0, 1, 2, 3, 3A, 4, 4A, 5, 6, 7, 8, 8A, 9, 10 plus the Streeck/Polanyi row checked. Almost every cell either:

(a) matches the C.2 formula exactly given the assigned class (e.g., 1.1 Neuhouser 19.5h, 1.3 Phänomenologie 8h, 2.1 ÖpM 10h, 3A.1 Lukács 26h, 4.1 Horkheimer 10h, 4.2 DdA 17.5h, 5.2 EuI 33h, 6.1 TKH I 12h, 7.1 KuA 44h, 7.4 Fraser-Honneth 45.5h, 7.7 Forst RauR 27h, 8.1 *Entfremdung* 28h, 8.2 KvL 49h, 8.6 Allen EoP 16h, 8.8 Stahl 23h, 9.2 Fricker 13h, 14.1 Streeck 15.5h);

(b) was already repaired in the 2026-05-25 audit pass (0.1 Celikates, 1.6 Khurana);

(c) carries a known executed-tier annotation (7.5 RdF "Full → 3 Lights", 6b McCarthy "Full retained at execution time") where the Inv hours match the *executed* tier, not the nominal one — these are not over-priced.

## Items potentially UNDER-priced (executed-tier vs declared-tier mismatch)

Two items have Inv hours below what their declared Full tier + chapter-count deliverables would require by the C.2 formula. The pattern: the Inv hours match a Light-tier execution but the Inv row carries a Full tier tag. Resolution is either to re-tag the Inv row (cheap, documentation only) or accept the Inv as honest about the realistic execution (Light).

- **9.3 Celikates *Kritik als soziale Praxis*** (M9): Inv 29h, formula at Full tier with 7 chapter Recons = ~35–39h. The deliverable list specifies "~8 Light Recons" — so the executed treatment is Light despite the Inv "Full" tag, which would give 25 + 3.75 (α×R) = ~29h. **The Inv hours match Light execution; the Full tag is mismatched.**
- **2.3 Heinrich *Kritik der politischen Ökonomie*** (M2): Inv 8.5h, formula at Full tier 140pp Transparent DE = 7.8h reading + ~2.3h writing = ~10h. The deliverable list specifies "5 Light Recons" (Heinrich Kaps. 1–5), so executed treatment is Light: 7.8 + 0.94 = ~8.7h. Inv 8.5h matches Light, again with a Full tag mismatch on the Inv row.

## Summary

**Cumulative Δ saved across the top candidates: ~10h** (already realised in the 0.1 + 1.6 repairs) **+ ~10–15h marginal additional** (items 2, 3, 4, 5 if all four re-priced, mostly low confidence). The bulk of the 25h originally suspected has already been captured by the 0.1 repair.

**Pattern observed.** The Celikates 0.1 mispricing was structurally **unique** — it was the one Einführung in the corpus that `text_classification.md` did not catch with a special rule (Heinrich 2.3 got special rule #1; 0.1 did not). All other Einführungen / companions / surveys in the active inventory (Outhwaite, McCarthy, Freyenhagen, Heinrich, Hollis-as-textbook, Jay, Wiggershaus-bonus, Horster CL1) are correctly assigned to Transparent or Analytic with appropriate pp/h. The remaining candidates (8.5 Jaeggi-Fraser conversation, 9.10 Collins) are *borderline* class-edge cases where the Layered classification is defensible but the reading character may be faster.

**Confidence levels.** Only the 0.1 fix is high-confidence (validated). Items 2 and 3 are low–medium confidence — the call hinges on the user's actual pace on dialogue volumes (8.5) and accessible-feminist-theory prose (9.10). Items 4 and 5 are very low confidence: within rounding error of the formula. **User should verify against own reading experience on dialogue volumes and partial-selection accessible monographs before re-pricing 8.5 / 9.10.**

**Net actionable freed hours from re-pricing (excluding the already-realised 0.1 + 1.6 = 19h):** ~10h at best, ~3h at worst, depending on user's call on items 2 and 3.
