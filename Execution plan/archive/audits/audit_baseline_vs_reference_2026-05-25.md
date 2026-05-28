# Inventory baseline-active audit — execution_plan_v1.md

**Date:** 2026-05-25
**File audited (read-only):** `/Users/michael/Sozialphilosophie/Execution plan/execution_plan_v1.md`, cross-referenced against `y3_critical_path_v2.md`.
**Purpose:** "C-pass" follow-up to `audit_inventory_vs_schedule_2026-05-24.md` — distinguish documentation gaps (reference-only rows mistakenly counted in Inventory sum) from real gaps (Schedule genuinely under-allocates baseline-active hours).

---

## 1. Per-module table

All hours rounded; "Δ" = Schedule − Baseline-active Inv (negative = Schedule under-allocates).

| Module | Header | Inv all-rows | Inv baseline-active | Schedule | Δ | Reference-only items removed |
|---|---:|---:|---:|---:|---:|---|
| Part 0 — Orientation | ~25 (sched) | 38 | 38 | ~45 (ex-retreat) / ~63 (incl. R1) | +7 / +25 | none — Orient reads ARE Part 0's planned activity |
| Module 1 — Hegel | 75 | 74.5 | 74.5 | ~76 | +1.5 | none (Khurana 1.6 baseline-active but Inv-hours over-priced; see Item-level §5) |
| Module 2 — Marx | 55 | 60.5 | 60.5 | ~64 (M2-only, ex-Khurana W18 portion) | +3.5 | none |
| Module 3 — Weber | 23 | 31 | 31 | ~24 | −7 | none |
| Module 3A — Lukács | 36 | 31.5 | 31.5 | ~40 | +8.5 | none |
| Module 4 — 1st Frankfurt | 70 | 66.5 | 66.5 | ~60 | −6.5 | none |
| Module 4A — Pragmatism | 40 | 34.5 | 34.5 | ~34 | −0.5 | none |
| Module 5 — Pos+Herm | 78 | 74.5 | 74.5 | ~65 | −9.5 | none (5.4 Gadamer is [RS]→Orient but **baseline-active per execution plan placement W48–49**) |
| **Phase I sub-total** | **402** | **411** | **411** | **~408** | **~−3** | — |
| Module 6 — Habermas TKH | 75 | 126.5 | 66.5 | ~88 (incl. R4 retreat ~17h) / ~71 ex-retreat | +4.5 ex-retreat | **6.6 F&G (32h)**, **6.7 Strukturwandel (28h)** — explicit "Optional; *Not currently in baseline*" annotations |
| Module 7 — Honneth | 162 | 259 | 235.5 | ~142 | **−93.5** | 7.11 J.Benjamin (9h, [RS] COULD), 7.14 Allen-Mendieta (13.5h, [RS] COULD), 11A.4 (1.5h, [RS] COULD). 7.18F Phase III frontier conditional (18h) already excluded. |
| Module 8 — Jaeggi | 150 | 190.5 | 188.5 | ~120 | **−68.5** | 8.11 Neuhouser article (2h, COULD baseline) |
| Module 9+10+Streeck | 150 | 198.75 | 194.5 | ~135 | **−59.5** | 9.9 Harding (4.25h, COULD) |
| Module 8A — Außereur. | 57 (all-in) | 33 | 33 | ~45 | +12 | none |
| **Phase II sub-total (excl. M8A)** | **537** | **774.75** | **685** | **~485** | **~−200** | — |
| **Phase II incl. M8A** | **594** | **807.75** | **718** | **~530** | **~−188** | — |

*Note on counts.* This audit's Phase II all-rows count (775h ex-M8A) differs from the prior audit's 703h because it includes the cluster table's full Module-9+10+Streeck inventory (~199h) including the v2.1 un-deferred items (Vogelmann, Boltanski, Harding, Aglietta, von Redecker). If those un-deferrals were excluded from the prior audit's tally, the gap collapses (~199 − ~65 of un-deferred SHOULDs ≈ ~134, which plus M6 67 + M7 259 + M8 190 ≈ 650; still some difference but order-of-magnitude reconciled).

## 2. Phase II reconciliation

- Header sum (M6 75 + M7 162 + M8 150 + M9+10+Str 150 = **537h**, +M8A 57 = **594h**).
- All-rows Inv: **775h ex-M8A / 808h with M8A**.
- Baseline-active Inv: **685h ex-M8A / 718h with M8A**.
- Schedule sum: **~485h ex-M8A / ~530h with M8A** (prior audit's ~547h was close).

**The gap is partially documentation but mostly real.** Removing ~90h of reference-only rows (mostly the M6 conditional F&G+Strukturwandel pair, ~60h) shrinks all-rows Inv from 775 → 685. But baseline-active Inv (685h) still exceeds Schedule (~485h) by ~200h ex-M8A. Headers (537h) sit closer to Schedule than to baseline-active Inv, suggesting **Headers were calibrated to scheduled hours, not to baseline-active inventory** — which means the gap was *built into the modules*, not a re-pricing artefact. With M8A: 718 baseline-active vs 530 scheduled = ~188h under-allocation.

The bridge §6 Class A "~20% capacity overage" framing tracks: 718/594 ≈ +21% over header, and Schedule covers only ~530/718 ≈ 74% of baseline-active reading time.

## 3. Programme total reconciliation

Phase I all-rows = baseline-active = ~411h (Phase I has essentially no reference-only rows; everything in the Inventory tables for M1–5 is MUST or SHOULD-active and matched by Schedule). Header sum Phase I (Part 0 ~25 + M1 75 + M2 55 + M3 23 + M3A 36 + M4 70 + M4A 40 + M5 78) = ~402h. Schedule ≈ 408h.

**Phase I:** essentially no overage (Inv ≈ Header ≈ Schedule, all ~410h).
**Phase II:** baseline-active Inv 718h vs Header 594h → **+21% over header** (vs prior +27% on all-rows; modest improvement).
**Phase II schedule under-allocates baseline-active by ~188h (~26%).**

For the **+27% / +22% prior overage figures**: the +27% was Inv/Header for Phase II all-rows. Reclassification lowers it to ~+21% — the documentation correction shaves ~6 percentage points off, but the bulk of the overage is real (the v2.1 un-deferred items + Anchor upgrades genuinely added hours that Headers haven't absorbed).

## 4. Residual real gaps (Schedule < Baseline-active Inv by ≥10h)

| Module | Δ | Disposition required |
|---|---:|---|
| **Module 7 — Honneth** | **−94h** | Largest gap by far. Schedule (~142h) covers only ~60% of baseline-active Inv (~235h). Either (A) cut more SHOULD-Lights from active scope (7.13 Renault 18h, 7.17 Bedorf 14h, 11A.1+11A.2 Foucault ~15h — but bridge §2.4 flags Vogelmann-equivalent interlocutor protection for some) or (B) raise Schedule (consume more retreat hours, push into M22–M23 boundary). |
| **Module 8 — Jaeggi** | **−69h** | Schedule (~120h) covers ~64% of baseline-active (~189h). Largest single contributor: 8.2 KvL at 49h Inv vs Schedule slot of ~25h "M23 Jaeggi KvL chs. 1–3 + 8" + "M24 chs. 9–10". The 10 Full Recons deliverable is not budget-matched. Either cut chapter coverage (Full → Light for chs. outside 1–3/8–10) or expand schedule. |
| **Module 9+10+Streeck** | **−60h** | Schedule (~135h) covers ~69% of baseline-active (~194h). v2.1 un-deferrals (Vogelmann 21, Boltanski 16, Aglietta 10, von Redecker 14 ≈ 61h) account for nearly all of the gap. The §A.1 Layer 1 cut list explicitly identifies these as restorable. |
| Module 5 — Pos+Herm | −10h | Modest; mostly EuI's 33h Inv vs schedule absorption (~17h across W50–52). Within typical Full-tier overhead slack — not a structural issue. |

Phase I residual gaps are all <10h and within tolerance.

**Trade-off summary.** The Phase II ~188h Schedule shortfall is concentrated in M7/M8/M9+10. Three structural fixes possible: (i) absorb §A.1 Layer 1 cuts (recovers ~60h in M9+10+Str + ~32h in M7 = ~92h, halving the gap); (ii) demote chapter-level coverage for Jaeggi 8.2 (10 Full Recons → 5 Full + 5 Light recovers ~15h); (iii) raise the Header → Schedule integration disciplines (Module 7 header is 162h but Schedule only 142h — closing this alone fixes 20h).

## 5. Item-level reclassifications (baseline → reference-only)

Per-row justifications follow the tier annotation in the Inventory column:

| ID | Text | Hrs | Tier annotation justifying reference-only |
|---|---|---:|---|
| 6.6 | Habermas, *Faktizität und Geltung* | 32 | "[ES] → Light...**Optional**: schedule in M18–M19...***Not currently in baseline because of capacity overage; flag for re-decision at R4***" |
| 6.7 | Habermas, *Strukturwandel der Öffentlichkeit* | 28 | "[ES] → Light...**Optional**: schedule alongside 6.6...***Not currently in baseline***" |
| 7.11 | J. Benjamin (intersubjectivity) | 9 | "[RS] → Light (per y3 **COULD**; conditional SHOULD/Engage if love-sphere/socialisation track)" |
| 7.14 | Allen & Mendieta, responses-to-Jaeggi | 13.5 | "[RS] → Light (per y3 **COULD**; conditional SHOULD if Jaeggi-Allen debate central)" |
| 7.18F | Honneth, *Anerkennung* — Phase III frontier upgrade | 18 | "Full reading + Full reconstruction at Phase III frontier (M37–39)" — explicit Phase III placement, not Phase II baseline |
| 11A.4 | Allen, "Power, Subjectivity, and Agency" | 1.5 | "[RS] → Light (per y3 **COULD**; useful for the debate; light note)" |
| 8.11 | Neuhouser article (on Honneth normative reconstruction) | 2 | "[P] → Light (per y3 **COULD** baseline; v2.0 Full tier-bump demoted)" |
| 9.9 | Harding, *Whose Science?* | 4.25 | "[O] → Orientation (per y3 **COULD**; deferrable per §A.1 Layer 1 if Layer 1 includes COULDs)" |

**Total reclassified to reference-only: ~108h Phase II** (60h in M6 conditional F&G/Strukturwandel + 42h M7 + 2h M8 + 4.25h M9+10).

## 6. Ambiguous calls flagged for user decision

The following items are SHOULD-tier baseline-active per tier annotation, but carry "deferrable per §A.1 Layer 1" or interlocutor-exempt flags that make the Schedule-allocation decision genuinely user-discretionary:

| ID | Text | Hrs | The ambiguity |
|---|---|---:|---|
| **9.6** | **Vogelmann, *Wirksamkeit des Wissens*** | **21** | Tier: SHOULD Light, un-deferred v2.1, ***exempt* from §A.1 Layer 1** per bridge §2.4 interlocutor argument. So baseline-active. But Module 9+10 schedule has no obvious 21h slot for it (M25–M26 inventory line lists it but month-totals don't add up to absorb it). **Real Schedule under-allocation, not documentation.** |
| 7.13 | Renault, *Souffrances sociales* | 18 | SHOULD Light, un-deferred v2.1, "§A.1 Layer 1 first-cut candidate". Baseline-active by tier, but explicitly first to cut. |
| 7.17 | Bedorf, *Verkennende Anerkennung* | 14 | Same: SHOULD Light, Layer 1 first-cut candidate. Baseline-active by tier; exit at first 4-week trigger. |
| 9.7 | Boltanski, *On Critique* | 16 | SHOULD Light, Layer 1 candidate. Baseline-active by tier; first cut. |
| 14.9 | Aglietta, *Régulation* | 10 | SHOULD Orientation, Layer 1 candidate. Baseline by tier; first cut. |
| 14.8 | von Redecker | 14 | SHOULD Light, "**Flag**: deferring conflicts with interlocutor argument — user decision required if §A.1 Layer 2 fires". Symmetric to Vogelmann/Jütten. |
| 8.10 | Jütten | 2 | SHOULD Light, "flags against §A.1 Layer 2 cuts". Trivial hours, baseline-active. |
| 1.6 | Khurana, *Das Leben der Freiheit* | 19 | Tier: SHOULD Orient → baseline-active. But Hrs cell (19h) appears priced from a Full-tier estimate of all of "Intro + Part I"; Inventory footnote says ~8–12h orientation tier; Schedule only absorbs ~3h in W18. **Likely an Inv-hours mispricing — should be ~10h to match annotation.** |
| 5.4 | Gadamer, *W&M* Part II selections | 16.5 | [RS] → Orient (per y3 SHOULD; tag-exception). Baseline-active per W48–49 placement; tier says reading-log only, no filed Recon. The 16.5h is reading-time, which Schedule partly absorbs (~11h). Mild under-allocation, not documentation. |

## 6a. Specific gap reclassifications requested

- **Khurana 1.6 (19h Inv vs ~3h scheduled):** **Mostly documentation.** Item is baseline-active (SHOULD Orient placed at W18) but the 19h Inv-hour cell is over-priced for an Orient-tier read. The execution plan's own footnote says "~8–12h orientation tier" — the Inv cell should be re-priced down to ~10h, which would tighten the gap to ~5–7h (real but small).
- **Gadamer 5.4 (16.5h Inv vs ~11h scheduled):** **Mixed, leaning real.** Tier is [RS]→Orient, but the 16.5h is roughly the genuine reading time for "Part II selections" at dense German pace. Schedule absorbs 11h; ~5.5h shortfall is real but within tolerance.
- **Celikates–Jaeggi 0.1 (25h Inv vs ~16h scheduled):** **Real under-allocation.** This is the orientation text and the only [O]/MUST-Engage Anchor read in Part 0; Inv hours match the syllabus pp/h estimate. Schedule (3+5+5+3 = 16h across W1–W4) under-allocates by ~9h. Part 0 is a deliberately light ramp so this is acceptable, but it is *real* under-allocation, not a documentation artefact.

## Bottom line

The prior audit's ~150h Phase II spread reduces to ~108h after stripping reference-only rows (M6 conditional pair = 60h; M7 [RS]-COULDs = 24h; misc = ~24h). **About 40% of the gap was documentation.** The residual ~188h gap (baseline-active 718h vs schedule 530h, incl. M8A) is real and concentrated in Modules 7, 8, and 9+10. The §A.1 Layer 1 cut list, if invoked, recovers ~92h, leaving a ~96h structural gap requiring either Header-Schedule re-integration or further demotion of Full→Light per-chapter Recon counts (esp. in 8.2 Jaeggi *KvL*).
