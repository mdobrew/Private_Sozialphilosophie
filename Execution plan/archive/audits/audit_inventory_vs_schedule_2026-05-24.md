# Audit: Per-Module Inventory-vs-Schedule Hour Mismatches in `execution_plan_v1.md`

**Date:** 2026-05-24
**File audited (read-only):** `/Users/michael/Sozialphilosophie/Execution plan/execution_plan_v1.md`
**Context:** Run immediately after the v2.1 importance-classification rebuild (see `execution_plan_v1_archived_2026-05-24_pre-v2.1-rebuild.md` for prior state). Triggered by user spotting that Module 0 / Celikates-Jaeggi shows ~25h in Inventory but only ~16h in Schedule.

---

## 1. Per-module table

| Module | Header (h) | Inventory sum (texts only, h) | Schedule sum (h) | Δ (Sched−Inv) | Type | Driver |
|---|---:|---:|---:|---:|---|---|
| Part 0 (Orientation) | 35 | 38 (0.1=25 · 0.2=3.5 · 0.3=2 · 0.4=7.5) | 42 (W1–W7) + R1 17 = 59 | Schedule reading 42 vs Inv 38 = +4 reading; but **0.1 Celikates/Jaeggi: Inv 25 vs Sched 16 = −9** | D (item-level Type A) | Celikates/Jaeggi under-scheduled (~9h); Honneth (~6h sched vs 3.5 inv) and Jaeggi (~6h sched vs 2 inv) over-scheduled to compensate |
| Module 1 — Hegel | 75 | 74.5 (1.1=19.5 · 1.2=28 · 1.3=8 · 1.6=19) | 68.75 (W9–W17) | −5.75 vs Inv; **−14h on Khurana 1.6 alone (Inv 19h, Sched ~3h in W18)** | A (large item-level) | Khurana 1.6 says ~19h in Inv but the placement note caps it at "8–12h", and the only schedule allocation is ~3h in W18. Net: ~16h Inv hours never appear in Schedule |
| Module 2 — Marx | 55 | 60.5 (2.1=10 · 2.2a=16 · 2.2b=26 · 2.3=8.5) | ~62 (W18–W25, excl. carry-over re-reads + 3h Khurana) | +1.5 vs Inv; Header understates by ~6h | C-ish | Reasonably consistent; header stale (~55 should be ~62) |
| Module 3 — Weber | 23 | 31 (3.1=7 · 3.2=13 · 3.3=11) | 24 (W26–W28) | **−7 vs Inv** | A | Inv Hrs computed at slow pp/h that the Schedule doesn't budget for. W26–28 is the slimmest module in the plan — 24h reading on ~270pp DE = ~11 pp/h, well above the Style × Tier matrix's Dense DE bottom of 5 |
| Module 3A — Lukács | 36 | 31.5 (3A.1=26 · 3A.2=5.5) | ~40 (W29–W32) | +8.5 vs Inv | B (small) | Schedule absorbs Anwendung #2 (3.5h), DM3 (2h), close (3h), QM2 (2.5h); reading itself ~25h matches Inv text-side |
| R2 | 17 | n/a | 17 | 0 | — | — |
| Module 4 — Frankfurt School | 70 | 66.5 (4.1=10 · 4.2=17.5 · 4.3=2 · 4.4=13 · 4.6=11 · 4.9=4 · 4.10=9) | ~62 (W35–W41) | −4.5 vs Inv | A (mild) | Light gap on Freyenhagen + MM |
| Module 4A — Pragmatism | 40 | 34.5 (4A.1=11.5 · 4A.2=17 · 4A.3=6) | ~34 (W42–W46) | −0.5 vs Inv; Header stale by ~6h | C | Header overstates; Inv≈Sched |
| Module 5 — Positivismusstreit | 78 | 74.5 (5.1=7 · 5.4=16.5 · 5.5=8.5 · 5.2=33 · 5.3=9.5) | **~65** (W47–W54; excludes BONUS Anwendung) | **−9.5 vs Inv, −13 vs Header** | A | Largest Phase I Type A. 5.2 EuI was v2.1-promoted to Full (33h Inv) but Schedule rows W51–W52 only allocate ~10.5+13=23.5h to EuI work; Gadamer Inv 16.5h is heavy for the [RS]→Orient tier with no filed Recon |
| Motivational Checkpoint | 15–20 | ~16–20 (Journal Test 8–10 + Field Report 8–10) | ~21 (W55–W57) | +1 | — | Consistent |
| R3 | 17 | n/a | 17 | 0 | — | — |
| **Phase I subtotal (incl. retreats, MC)** | ~486–495 | ~426 (text inv) | ~488 (sched, incl. retreats + MC + buffer wks W58–62) | Inv low because Khurana absent from Sched & practice overhead unallocated in Inv | — | — |
| R4 | 17 | n/a | 17 | 0 | — | — |
| Module 6 — Habermas TKH | 75 | 66.5 (6a=6.5 · 6b=5 · 6.1=12 · 6.2=11.5 · 6.3=23 · CL1=8.5; 6.6 / 6.7 conditional, not in baseline) | **88** (M16–M19) | **+21.5 vs Inv** | B | Schedule rows are month-bucket aggregates that include H2 begin, DM6, QM3, Skizze prep, Module-close work; Inventory only sums text Hrs |
| Module 7 — Honneth | 162 | **~214** (7.1=44 · 7.2=4 · 7.3=2 · 7.4=45.5 · 7.5=21 · 7.7=27 · 7.8=1.5 · 7.9=22 · 7.11=9 · 7.12=2 · 7.13=18 · 7.14=13.5 · 7.17=14 · 7.18=20 · 11A.1=13 · 11A.2=2 · 11A.4=1.5) | **142** (M19–M22) | **−72 vs Inv; −20 vs Header** | A (severe) + D | Inventory Hrs column sums to ~214h — significantly above the v2.1 header of 162h. Either the per-text Hrs were re-priced post-Anchor upgrades without re-totalling, or several items (7.9, 7.11, 7.14, 11A.4) are notionally "[RS]/COULD" and shouldn't be in the baseline sum. Schedule month-rows under-allocate by ~20h vs the header itself |
| Module 8 — Jaeggi | 155 (placement note) / 150 (subhead) | **~190** (8.1=28 · 8.2=49 · 8.3=2 · 8.4=1.5 · 8.5=21.5 · 8.6=16 · 8.8=23 · 8.9=28 · 8.10=2 · 8.11=2 · CL3=9 · CL4=8.5) | **120** (M22–M25) | **−70 vs Inv; −30 to −35 vs Header** | A (severe) | Same pattern. KvL alone is 49h Inv but month-rows have to share with everything else; M22=15h, M23=30h, M24=40h, M25=35h leaves no room for ~190h of texts. Reading-rate assumptions in Inv (Layered α + slow pp/h on Honneth-monograph-decouple) are inconsistent with Schedule month budgets |
| Modules 9+10+Streeck | 150 (v2.1) | **~199** (9.1=21 · 9.2=13 · 9.3=29 · 9.4=3.5 · 9.5=1.5 · 9.6=21 · 9.7=16 · 9.8=2 · 9.9=4.25 · 9.10=13.5 · 10.1=12.5 · 10.2=9.5 · 10.3=3 · 14.1=15.5 · 14.8=14 · 14.9=10 · CL5=10) | **135** (M25–M27) | **−64 vs Inv; −15 vs Header** | A (severe) | The six un-deferred SHOULDs (Vogelmann + Boltanski + Harding + Aglietta + von Redecker + Renault carry-in) totalling ~75h were added to Inventory in v2.1 but the Schedule month-rows did not absorb the full re-pricing — M25/26/27 = 42/45/48 still resembles the v2.0 month load of ~30/30/35 |
| Module 8A bridge | 57 (all-in, incl. closure) | 33 (texts) | ~45 (M27–M29 reading-only portion of bridge) | +12 vs text Inv; ≈ Header once synthetic note + H1 added | C-ish | Consistent if closure work counted |
| **Phase II subtotal** | 504 v2.0 / 620 v2.1 | ~703 (Inv sums) | ~547 (Sched sums M16–M29) | Inv > Header > Sched | — | — |
| Phase III (M30–M44) | bridge §4: 445; Cap. Env.: 462 | n/a (no per-text Inv tables) | ~352 (Schedule rows in document) | −93 vs bridge §4 | — | Document itself notes the reconciliation (R5 17h + W1 30h folded + W2 30h folded ≈ +60–90h not in row totals) — partially explained, ~10–15h residual delta |

## 2. Total mismatch magnitude

**Sum of |Δ| (Inventory − Schedule) across modules where both can be computed:**

Phase I: |9| (0.1 only) + |16| (1.6) + |1.5| (M2) + |7| (M3) + |8.5| (M3A) + |4.5| (M4) + |0.5| (M4A) + |9.5| (M5) ≈ **~57h** total absolute item/module mismatch in Phase I, with net signed delta ≈ −36h (Sched < Inv).

Phase II: |21.5| (M6) + |72| (M7) + |70| (M8) + |64| (M9/10) + |12| (M8A) ≈ **~240h** absolute, net signed delta ≈ **−192h** (Sched far below Inv).

**Programme totals reconciliation:**

| Source | Phase I | Phase II | Phase III | Programme total |
|---|---:|---:|---:|---:|
| **Capacity Envelope table** (Inv-driven, in doc) | 495 | 620 | 462 | **~1,612** |
| **Sum of Inventory Hrs columns** (text-only, per-module) | ~426 | ~703 | n/a (no Inv) | (n/a complete) |
| **Sum of Schedule Hrs cells** (per row) | ~488 | ~547 | ~352 | **~1,387** |

The "Capacity Envelope" total of ~1,612h is neither the Inventory sum nor the Schedule sum — it appears to be a third quantity ("header + community engagement formalisation + retreat overhead") and is the figure that drove the +27% / +22% capacity-overage claim.

The Schedule rows (what the user would actually live week-to-week or month-to-month) sum to ~1,387h — **~225h below the Capacity Envelope 1,612h, or ~14% lower**. The Inventory text-Hrs columns sum to even more than the Capacity Envelope on a Phase II basis but to less in Phase I (because Khurana, Pippin etc. are nominally "in" but only 3h scheduled).

## 3. Capacity-arithmetic correction

The document's stated overage figures (+27% at M44, +22% at M46 against the ~1,612h v2.1 baseline) **rest on the Capacity Envelope numbers, not on the Schedule rows the user is actually building against**.

If capacity arithmetic were instead driven by the **Schedule sums** (~1,387h):
- vs M44 envelope ~1,269h → overage **+118h (+9.3%)** — *not* +27%
- vs M46 envelope ~1,326h → overage **+61h (+4.6%)** — *not* +22%

The 18-point gap (+27% vs +9%) is large enough to change every downstream decision in §A.1 / the resolution-options analysis. The honest answer is that **neither number is right**:

- The Schedule rows materially under-allocate against what the v2.1-upgraded Inventory says is needed (Phase II especially — Mod 7, Mod 8, Mod 9/10 each under by ~60–70h vs Inv). Living the Schedule would mean either reading much faster than the Inventory's pp/h assumptions, or not finishing the un-deferred SHOULDs (which would default back to v2.0).
- The Capacity Envelope total (~1,612h) effectively imputes that the Schedule will absorb the full Inventory — but the Schedule rows do not reflect that absorption.

**The capacity-overage claim of +27% is high-confidence if Inventory rules; the actual lived load if Schedule rules is closer to +9% over M44 — which is within tolerance.** This is exactly the ambiguity the rebuild has hidden.

## 4. Top 5 worst offenders

1. **Module 7 — Honneth (Δ ≈ −72h vs Inv, −20h vs Header).** Inventory Hrs column sums to ~214h (likely double-counting conditional/RS items 7.9, 7.11, 7.14, 11A.4 alongside the baseline-active items) but the Schedule month-rows allocate only 142h to M19–M22. Even against the v2.1 header (162h), the Schedule under-allocates by ~20h. Likely cause: rebuild un-deferred 7.13 Renault (~18h) and 7.17 Bedorf (~14h) and re-tiered 11A.1 (~13h) + 11A.2 (~2h) into Module 7 Inventory, but month-rows (M19=32, M20=30, M21=42, M22=38) only modestly increased over v2.0 baseline.

2. **Module 8 — Jaeggi (Δ ≈ −70h vs Inv, −30h vs Header).** Inventory: 8.1 28 + 8.2 49 + 8.5 21.5 + 8.6 16 + 8.8 23 + 8.9 28 = 165.5h of core Full-tier texts alone. Schedule allocates 120h. Likely cause: KvL (49h Inv) and Entfremdung (28h Inv) priced under Honneth-monograph-decouple (Layered pp/h + Full α) but Schedule month-rows treat them at faster rates.

3. **Modules 9+10+Streeck (Δ ≈ −64h vs Inv, −15h vs Header).** Six v2.1 un-deferrals (Vogelmann 21 + Boltanski 16 + Harding 4.25 + Aglietta 10 + von Redecker 14 + Fricker Full upgrade +2) add ~67h to Inventory but Schedule M25/26/27 budgets show only modest increase (~42/45/48 = 135 total) over what the v2.0 plan presumably had (~30/30/35 = 95). M27 is flagged as overloaded at 48h in the document and even that doesn't close the Inventory gap.

4. **Module 1 / Item 1.6 Khurana (Δ ≈ −16h on a single item).** Inventory says 19h; the placement note immediately below says "~8–12h orientation tier"; the W18 schedule entry allocates 3h. Three different numbers for the same item in three places within ~5 lines of each other. Almost certainly a v2.1 rebuild artefact — the per-text Hrs was recomputed via the Style × Tier formula (150pp Layered DE bottom ÷ 10 pp/h = 15h reading + Orient flat 0.25h = ~15.25h, not 19; but the placement note's 8-12h corresponds to a different pp/h assumption). Either Inv should drop to ~8h or Schedule should expand W18 (currently 10h total) to ~22h, which it cannot fit.

5. **Module 5 — Positivismusstreit (Δ ≈ −9.5h vs Inv, −13h vs Header).** 5.2 EuI was v2.1-promoted Light→Full Anchor (Inv ~33h, +5h from v2.0). Schedule W51/W52 only allocate ~10.5+13 = 23.5h to EuI-related reading + Full reconstruction. Gadamer 5.4 at 16.5h Inv is also expensive for an Orientation-tier text — the per-text Hrs computation appears not to have been re-priced when the tier was set to Orient.

Honourable mentions: **Part 0 / 0.1 Celikates/Jaeggi (−9h, the user's spotted example)**; **Module 3 — Weber (−7h, header & schedule both ~24h but Inventory says 31h, suggesting Inv was computed at slower pp/h than Schedule assumes)**.

## 5. Recommended reconciliation approach

There are three coherent paths; mixing them is what produced the current state.

**(A) Re-prorate Schedule to match Inventory** — the "honest if scheduled, the user will be at +27% overage" path.
- Requires rewriting every Phase II month-row upward by ~15–25h (M21 from 42→~58, M22 from 38→~55, M25 from 42→~60, M27 from 48→~70). Document already concedes M27 at 48h is overloaded.
- Closes the schedule-side under-allocation; preserves the v2.1 §A.1 cut-list cascade as the user's response surface.
- This is the most truthful but worst-news path.

**(B) Re-price Inventory to match Schedule** — implicitly bake faster reading rates / smaller selections into the Inv column.
- Phase II Inv would drop from ~703h to ~547h (the Schedule sum), implying Inv was computed at roughly 30% slower pp/h than the Schedule month-buckets implicitly use.
- Would require either accepting faster real reading speed than the Style × Tier matrix's "bottom-of-range" or formally re-scoping (e.g., Khurana to 8h not 19h; KvL to selective chapters; Honneth-monograph-decouple loosened).
- Brings the +27% overage figure down to ~+9%, which is within tolerance.

**(C) Mark some Inventory items "active in module but Hrs scheduled separately"** — explicitly carve out which Inv items the Schedule rows are intended to absorb vs which are reference-only.
- For Module 7: 7.9 N&P (22h), 7.11 J. Benjamin (9h), 7.14 Allen-Mendieta (13.5h), 11A.4 (1.5h) are [RS] / COULD — likely intended as "in the Inventory for completeness but not Schedule-baseline". If those ~46h are flagged "not in baseline Schedule", the Mod 7 Inv drops from ~214 to ~168, close to the 162h header.
- This is a documentation fix, not a re-pricing.

**Intentional vs. unintentional mismatches.** Some of the Schedule>Inventory cases (Module 3A +8h, Module 6 +21h) are legitimately intentional — practice/H2/close/Skizze/QM hours need somewhere to live and the Inv column doesn't carry them. Document this with an explicit overhead row per module, or accept the Type B mismatch as designed.

**Recommended sequence:**

1. **Fix (C) first** — explicitly mark which Inventory items are baseline-active vs. reference. This likely resolves Module 7's Inv sum and several phantom items elsewhere. Cheap, no real reorganisation.
2. **Then audit (B) vs (A)** — for each module where the Δ remains ≥10h after (C), decide whether the truth is "the Schedule lies and we're +27% overloaded" or "the Inv was over-priced and we're actually fine". The Capacity Envelope arithmetic depends on this answer.
3. **Re-price single-item discrepancies** (Khurana 1.6 = 19h vs 8–12h vs 3h; Gadamer 5.4 = 16.5h vs Orient tier).
4. **The Part 0 / 0.1 Celikates-Jaeggi gap is real** — Inv 25h, Sched 16h. The Schedule has 16h of Einführung reading across W1–W4 at ~5h/wk on ~270pp of Layered DE — that's ~17 pp/h, well above the matrix's Layered DE bottom of 10. Either Schedule needs ~4 more hours per week (impossible in the ramp) or the Inv pp/h assumption should be lifted to acknowledge the Einführung is genuinely lighter than the matrix default.

**Bottom line.** The 18-percentage-point swing between the Schedule-driven overage (+9%) and the Capacity-Envelope-driven overage (+27%) at M44 is the single most consequential finding. Until the per-module Inventory/Schedule gaps are reconciled, the cut-list cascade in §A.1, the M44-vs-M46 decision, and the "interlocutor-flagged Layer 2 conflict" all rest on unstable arithmetic.
