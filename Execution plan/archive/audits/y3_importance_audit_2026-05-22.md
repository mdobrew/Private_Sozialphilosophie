# y3 importance-classification audit — 2026-05-22

*Audit subagent report. Field-importance only (timeline-independent). Audits `y3_critical_path.md` against the syllabus + recent ground-up Hrs computation. Reviews framework structure, tier-derivation rule, and ~25 per-text classifications.*

---

## Part 1 — Framework structure review

The four-category schema (MUST / SHOULD / COULD / DISCRETIONARY) is largely defensible and should be **kept as the top-level structure**. The reasons: (a) it tracks the Phase III-defensibility question cleanly; (b) the conditional-promotion machinery (§4) already gives COULD the role a finer-grained system would split out; (c) more categories would not produce more decisions, only more tagging overhead. The problems are at the **boundary of MUST and at the joint between MUST and tier-derivation**, not in the number of bins.

### Concern 1 — Granularity of MUST: sub-split is warranted

The current rule treats "MUST" as one bin and lets the [P*] / [P] / [ES] tag do the tier work. This conflates two distinct field-importance facts about a MUST text:

- (a) **Reconstruction-load**: is the text one whose argument the user must *himself reconstruct in his own voice* (because he will defend a position in its conceptual idiom in front of reviewers)?
- (b) **Coverage**: is the text one the user must *know well enough to engage in a debate* (because reviewers will expect citation/familiarity)?

These come apart. Hegel *Phänomenologie* IV.A is a paradigm of (a) for a recognition-theoretic piece — the Herr/Knecht structure is the conceptual apparatus the user will reuse — but it carries only ~30 pages of [P] tag. McCarthy *Critical Theory of Habermas* is paradigm (b) — a MUST [ES*] not because the user must reconstruct McCarthy's argument but because it lets him reconstruct Habermas's. The existing rule (MUST [P*] → Full, MUST [P] / [ES] → Light) gets McCarthy right by accident (Light is right for a secondary) but gets *Phän*. IV.A wrong (Light is too thin for a load-bearing recognition primary).

**Proposal**: sub-split MUST as follows.

- **MUST-Anchor** (reconstruct fully; tier = Full regardless of [P*] / [P] / [ES] tag): the text whose conceptual apparatus the user will *deploy* in the Phase III piece. Maps to "the user will need this text's structure under his own pen."
- **MUST-Engage** (reconstruct lightly; tier = Light): the text the user must read and be able to characterise but will not himself rework. Reviewer-expected citation; lay-reader fluency.

This sub-split is field-importance-derived, not timeline-derived. It also makes Concern 3 (below) tractable: MUST-Anchor and MUST-Engage are roughly the *intersection* and the *symmetric difference* of the two definitions of "essential."

### Concern 2 — Matrix sparseness

The implicit matrix `syllabus tag × y3 importance → tier` is sparser than it looks but not so sparse that the structure is redundant. Realistic cells:

| tag → | MUST | SHOULD | COULD | DISCR. |
|---|---|---|---|---|
| [P*] | yes (common) | very rare | impossible in practice | impossible |
| [P] | yes (common) | yes (common) | yes (conditional) | rare |
| [ES] / [ES*] | yes (when no [P] substitute) | yes (common) | yes | rare |
| [RS] | rare | yes | yes (common) | yes |
| [O] / [O*] | rare ([O*] for orientation entry only) | yes | yes | yes |
| [NE] | almost never (one exception below) | rare (Phase IV-deferred default) | rare | yes (default) |
| [MX] | only if Phase III commits | yes (conditional) | yes | yes (default) |

Two non-trivial cells:

- **[P*] = SHOULD**: essentially impossible. If a text has [P*] in v6, it's already curatorially load-bearing — it can't simultaneously be skippable. The only way this cell becomes populated is via an explicit syllabus re-tagging, in which case the tag, not y3, should change.
- **[ES] = MUST**: this cell is populated whenever a secondary text *carries argumentative load that no primary equivalent does*. McCarthy (5.5/6.3), Neuhouser (1.1), Heinrich (2.3), Freyenhagen (4.6) are paradigms. The current framework handles this correctly (these are MUSTs) but the *tier* it routes to (Light) under-utilises some of them. Neuhouser and Heinrich are arguably MUST-Anchor by the sub-split above — they are how the user actually reaches Hegel's *Sittlichkeit*-apparatus and Marx's Wertform-apparatus respectively, both of which will appear in the Phase III piece.

So the matrix is **not so sparse as to be redundant**, but it has two regularities worth surfacing in the document: ([P*] = MUST) is forced and (rare [ES] = MUST-Anchor when secondary > primary as portal).

### Concern 3 — Definition of "essential"

The user's two criteria are genuinely orthogonal:

- (a) **Phase III reviewer-essential** — appears in draft / expected by reviewers
- (b) **Tradition-anchoring** — cannot engage Frankfurt social philosophy without it

The neatest way to handle this is **not** to split MUST into two sub-categories of "essentiality" but to recognise that (a) and (b) supply *different and largely complementary* reasons for the same MUST verdict. The vast majority of texts MUST for (a) are also MUST for (b) — Hegel *RP*, Marx *Kapital* ch. 1, Honneth *KuA*, Jaeggi *KvL*, Fraser-Honneth, Habermas TKH. Where they diverge:

- **(b) but not (a)**: *DdA* (4.2), Adorno *Negative Dialektik* (4.5/4.4 in y3 numbering), Lukács "Verdinglichung" (3A.1). These are tradition-foundational and *will* be invoked in citation, but if the Phase III piece is on Honneth-Jaeggi normative reconstruction they are not load-bearing for the *argument* itself. The right answer here is: keep them MUST, but route to **MUST-Engage** (Light) not **MUST-Anchor** (Full). The tradition demands you've read them with comprehension; the Phase III piece does not demand you reconstruct them.
- **(a) but not (b)**: Zurn "Second-Order Disorders" (8.3), Laitinen-Särkelä typology (8.4), Forst "Noumenal Power" (7.8). These are not tradition-anchoring — the Frankfurt tradition existed perfectly well without them — but they *are* what current reviewers expect anyone writing on social pathology / power to engage. These are clean MUST-Engage cases: cite, characterise, position-take, but no reconstruction-as-apprenticeship is required.

So **the unified criterion for MUST is the disjunction** (a) ∨ (b), and the **MUST-Anchor / MUST-Engage split tracks the intersection vs. the symmetric difference**. Recommended reformulation for §1:

> A text is MUST if either it is reviewer-expected for the Phase III piece (Phase III-reviewer-essential) or it is tradition-anchoring (cannot engage Frankfurt social philosophy without it). MUSTs that satisfy *both* criteria *and* whose apparatus the user will deploy under his own pen are MUST-Anchor (Full). MUSTs that satisfy one criterion only, or that supply reviewer-expected coverage without conceptual reuse, are MUST-Engage (Light).

---

## Part 2 — Tier-derivation rule scrutiny

The current rule maps tag → tier directly and routes through the MUST/SHOULD/COULD/DISCR. label only to determine *whether the text is on the schedule at all*. This is the conflation diagnosed in Part 4 below: tier is being read off the **syllabus tag** when it should be derived from the **y3 classification × tag** product.

**Proposed sharpened rule** (replacing y3 §2 tier defaults):

| y3 class | Tier | Notes |
|---|---|---|
| MUST-Anchor | **Full** | Regardless of tag. Used when the text's apparatus will appear in the Phase III piece under the user's own pen. |
| MUST-Engage | **Light** | Default for MUSTs that are reviewer-expected coverage but not apparatus-reuse. |
| SHOULD [P]/[ES] | **Light** | Unchanged. |
| SHOULD [O]/[RS] | **Orientation** | Unchanged. |
| SHOULD [P*] | **Light** (anomalous; flag) | This cell should almost never occur — if it does, re-examine whether the text is actually MUST. |
| COULD any tag | **Orientation** | Unchanged unless promoted to MUST/SHOULD via §4 trigger. |
| DISCRETIONARY | **skip / Phase IV** | Unchanged. |

Asymmetries this captures that the current rule misses:

1. A MUST [P] can be either Full or Light depending on whether it is anchor or coverage. *Phän*. IV.A is the paradigm of MUST-Anchor [P] → Full.
2. A MUST [ES] (e.g., Neuhouser, Heinrich) can be Full when it is the *portal* through which the user controls a primary apparatus he will reuse. The current rule's blanket "MUST [ES] → Light" undersells exactly those secondaries.
3. SHOULD [P*] / [ES*] should not exist; if it does, that is a flag to re-examine the y3 class, not a routing rule.

---

## Part 3 — Per-text re-evaluation (main deliverable)

Texts whose y3 class or tier-derivation should change on **field-importance** grounds. Numbering follows the y3_critical_path.md item IDs (which mostly track syllabus v5; v6 IDs noted where they shift, e.g., the post-v6 renumbering of K → Module 14 / 13).

| Syllabus ID (y3) | Author / short title | Current y3 class | Current tier | Proposed y3 class | Proposed tier | Rationale (field-importance) |
|---|---|---|---|---|---|---|
| 1.1 | Neuhouser *Foundations of Hegel's Social Theory* | MUST [ES*] | Full (by [ES*]) — currently correctly Full | **MUST-Anchor** | Full | Already Full by [ES*] tag — fine; flag is that under the *sharpened rule* this should remain Full *because anchor*, not because of the tag. Neuhouser's centrality is uncontroversial in Hegelian-Frankfurt reception (Honneth's *KuA* §2, Khurana, Jaeggi all engage). |
| 1.2 | Hegel *Rechtsphilosophie* | MUST [P] | Light | **MUST-Anchor** | **Full** | The Phase III piece (any plausible terrain — recognition / *Sittlichkeit* / normative reconstruction / capitalism-as-form) will deploy *Sittlichkeit*-apparatus directly. Light reconstruction is mismatched to the depth at which the user must control §142 ff. |
| 1.3 | Hegel *Phän.* IV.A | MUST [P] | Light | **MUST-Anchor** | **Full** | The execution plan already deviates upward to Full. y3 should systematise this rather than leave it as plan-side annotation. Herr/Knecht is the conceptual entry to *all* recognition theory (7.1, 7.18) and is invoked structurally, not just cited. |
| 2.1 | Marx ÖpM "Entfremdete Arbeit" | MUST [P*] | Full | MUST-Anchor | Full | Already correct. Listed for confirmation. |
| 2.2a/b | Marx *Kapital* I (ch.1 §§1–4 + chs. 2–3 + ch. 10) | MUST [P*]/[P] | Full ch.1 / Light chs. 2–3,10 (split per execution plan) | **MUST-Anchor** ch.1 §4 + **MUST-Engage** chs. 2–3, 10 | Full §4 + Light chs. 2–3, 10 | Endorses the current execution-plan split. y3 should formalise: §4 (Fetisch) is anchor; chs. 2–3 & 10 are engage. |
| 2.3 | Heinrich *KpÖ* | MUST [ES] | Light | **MUST-Anchor** | **Full** | The *neue Marx-Lektüre* framing is precisely the apparatus the user will deploy in a capitalism-as-form Phase III piece. Heinrich is short, transparent, and the access route to value-form thinking; reconstructing him at Full tier is field-importance-justified for an ECB-economist user. |
| 3.1 | Weber "Wissenschaft als Beruf" | MUST [P] | Light | MUST-Engage | Light | Confirmed; no change. (Listed because the v6 Dense classification might mislead one to upgrade.) |
| 3.2 | Weber "Objektivität" essay | MUST [P] | Light | MUST-Engage | Light | Same. Reviewer-expected but apparatus is contested, not reused. |
| 3A.1 | Lukács *Verdinglichung* essay | MUST [P] | Light | **MUST-Engage** but flag for Full upgrade *if* Phase III commits to reification/Verdinglichung | Light → Full conditional | Currently Light is defensible if Phase III is Honneth-Jaeggi pathologies. If it goes Adornian or Honneth *Verdinglichung* (2005)-engaged, this needs Full. Add to §4 trigger table. |
| 4.1 | Horkheimer "Traditionelle und kritische Theorie" | MUST [P*] | Full | MUST-Anchor | Full | Confirmed. Listed because the [P*] is what defines "what makes a theory critical" — for any methodological Phase III piece this is anchor, not engage. |
| 4.2 | *DdA* (Begriff + Odysseus) | MUST [P] | Light | **MUST-Engage** | Light | Confirmed. Distinguish from (b) tradition-anchor: it *is* tradition-anchor, but the user will cite, not reconstruct, the instrumental-rationality apparatus unless Phase III commits to Adornian/critical-theory-of-rationality terrain. Flag for upgrade. |
| 4.5 (y3) / 4.6 (v6) | Freyenhagen *Adorno's Practical Philosophy* | SHOULD | Light | **MUST-Engage** *if* Phase III touches social-pathology Adornian baseline; otherwise SHOULD | Light | Freyenhagen is the major bridge between Adorno and the pathologies debate (Honneth 0.2, Zurn 8.3). Currently SHOULD undersells him for a pathologies-track piece. Flag as conditional MUST. |
| 4A.1 | Dewey *Public and Its Problems* | MUST [P] | Light | MUST-Engage | Light | Confirmed. |
| 4A.3 | Mead *MSS* Part III | MUST [P] | Light | **MUST-Anchor** | **Full** | Honneth's three recognition spheres (Liebe / Recht / Solidarität) descend structurally from Mead's I/me, generalised other, social self. For any recognition-track Phase III piece, this is apparatus the user deploys, not background he cites. Currently underweighted. |
| 5.5 (y3) / 5.1 (v6) | McCarthy *Critical Theory of JH* chs. 1–3 | MUST [ES*] | Full | **MUST-Engage** | **Light** | Counter-intuitive but field-importance-correct: McCarthy is a portal text, not an apparatus the user redeploys. The "best secondary" honour does not translate to Full reconstruction load. Bridge §3 protocol for orientation-monographs would already route here. (This is a downward revision; the user should consider whether the [ES*] tag is itself over-claimed in v6.) |
| 6.1 (y3) / 6.3+6.5 (v6) | Habermas TKH selections | MUST [P] | Light | **MUST-Anchor** for the ch. I rationality apparatus + Light for VI–VIII | Full ch. I, Light VI–VIII | TKH ch. I is apparatus for any communicative-reason engagement; VI–VIII are coverage for the *Lebenswelt*-colonisation thesis. Currently undifferentiated. |
| 7.1 | Honneth *Kampf um Anerkennung* | MUST [P*] | Full | MUST-Anchor | Full | Confirmed. Anchor of an entire module's worth of subsequent argument. |
| 7.5 | Honneth *Recht der Freiheit* selection | MUST [P] | Light | **MUST-Anchor** | **Full** | The method of normative reconstruction is precisely the methodological position the Phase III piece will work in or against. The Markt chapter is the diagnostic specimen for any capitalism-track piece. Light is mismatched. |
| 7.7 | Forst *Recht auf Rechtfertigung* | MUST [P] | Light | **MUST-Engage** | Light | Confirmed for default terrain. Forst is the *alternative* the user will position against, not the apparatus he reuses (unless Phase III pivots to justification-theoretic terrain — §4 conditional). |
| 7.8 | Forst "Noumenal Power" | MUST [P] | Light | MUST-Engage | Light | Confirmed. Reviewer-expected citation; not apparatus reuse. |
| 7.17 | Honneth *Anerkennung* (2018) | MUST split | Light partial + conditional Full | **MUST-Engage** baseline + **MUST-Anchor** conditional | Light + Full conditional | The current v1.2 split is correct in *structure*; the audit only proposes renaming the two halves to align with the sub-split. |
| 7.18 (y3) / 7.19 (v6) | Honneth *Arbeitende Souverän* | SHOULD | Light | **MUST-Engage** (baseline) | Light | This is currently SHOULD with conditional MUST. Field-importance-wise: for an ECB-economist user submitting in 2027–28, *not engaging Honneth's most recent monograph on work / democracy / *Sittlichkeit* is reviewer-noticeable*, irrespective of Phase III topic. Raise to MUST-Engage at baseline. (NB: this *is* a borderline call; reasonable disagreement exists — e.g., one might argue *Arbeitende Souverän* will not have settled reception by 2027. I'd hold it MUST-Engage on the strength of the ECB-economist authorial position.) |
| 8.1 | Jaeggi *Entfremdung* | MUST [P*] | Full | MUST-Anchor | Full | Confirmed. |
| 8.2 | Jaeggi *KvL* | MUST [P*] | Full | MUST-Anchor | Full | Confirmed. The defining systematic statement of the framework. |
| 8.3 | Zurn "Second-Order Disorders" | MUST [P*] | Full | **MUST-Engage** | **Light** | The current [P*] → Full route is over-investment. Zurn is short, conceptually clean, and Phase III-reviewer-essential as a typology *to cite*, not to reconstruct at Full tier. Demoting to Light frees reconstruction budget for actual apparatus texts. (This is the clearest case in the audit of [P*] over-claiming the tier. Either retag in v6 or override in y3.) |
| 8.4 | Laitinen-Särkelä typology | MUST [P*] | Full | **MUST-Engage** | **Light** | Same as 8.3. A 20-page typology article does not justify Full-tier reconstruction overhead. Reviewer-expected coverage at Light is sufficient. |
| 8.6 | Allen *End of Progress* | MUST [P] | Light | **MUST-Anchor** *if* Phase III engages decolonial / progress-critique; **MUST-Engage** otherwise | Light → Full conditional | Allen is *the* internal-Frankfurt bridge to Module 8A. If the Phase III piece touches Allen's challenge, it is apparatus; if not, it is coverage. Add §4 trigger. |
| 8.5 | Jaeggi-Fraser *Capitalism* | MUST [P*] | Full | MUST-Engage | **Light** | A dialogue volume does not warrant Full reconstruction per chapter. Light per text suffices for a debate text the user uses *as a debate*. (Same logic as 8.3, 8.4: [P*] is over-claimed by the tag system for dialogue/short formats.) |
| 8.8 | Stahl *Immanente Kritik* | SHOULD [ES] | Light | SHOULD | Light | Confirmed. |
| 8.12 | Jaeggi *Fortschritt und Regression* | SHOULD | Light | **MUST-Engage** (baseline) | Light | Same logic as 7.19 Honneth *Arbeitende Souverän*: a 2023 monograph by the field's defining figure that supplies the reply to Allen 8.6 — not engaging it reads as engaging 2014-Jaeggi. Promote from SHOULD to MUST-Engage at baseline; Full only if Phase III commits to progress-and-regression terrain. |
| 8A.1 | Said *Orientalism* Intro | MUST | Light | MUST-Engage | Light | Confirmed. (The second-revision promotion to MUST is right; tier is right.) |
| 8A.4 | Quijano "Coloniality of Power" | MUST | Light | MUST-Engage | Light | Confirmed. |
| 8A.6 | Robinson *Black Marxism* | MUST [P] | Light | **MUST-Engage** + flag for **MUST-Anchor** if Phase III commits to racial-capitalism via Fraser K.2 | Light → Full conditional | Robinson is the *concept-supplier* (racial capitalism) that Fraser then uses. If Phase III touches that bridge, anchor; if not, engage. Currently y3 already notes the forward edge. |
| 9.1 | Mannheim *I&U* Part I | MUST [P] | Light | MUST-Engage | Light | Confirmed. |
| 9.2 | Fricker *Epistemic Injustice* | MUST [P*] | Full | **MUST-Anchor** *if* Phase III touches social-epistemology; **MUST-Engage** otherwise | Full → Light conditional | The current [P*] → Full route assumes Phase III engages Fricker. Field-importance-wise, this depends on topic firm-up. The conditionality is *real* — uncommitted, Fricker is reviewer-expected coverage. |
| 9.3 | Celikates *Kritik als soziale Praxis* | MUST [P*] | Full | **MUST-Anchor** | Full | Confirmed. Lay-normativity apparatus is itself a candidate Phase III terrain. |
| 9.4 | Jaeggi "Was ist Ideologiekritik?" | MUST [P] | Light | **MUST-Engage** baseline; **MUST-Anchor** if Phase III engages ideology critique | Light → Full conditional | Currently flat MUST-Light. The conditional matters: an ideology-critique-track Phase III piece reconstructs Jaeggi's move; a recognition-track piece cites it. Add §4 trigger. |
| 9.10 | Hill Collins *BFT* | MUST [ES] | Light | MUST-Engage | Light | Confirmed. |
| 10.1 (y3) / 12.3 (v6) | Taylor "Interpretation and the Sciences of Man" | MUST [P*] | Full | **MUST-Anchor** | Full | Confirmed. Taylor is methodological apparatus for any reconstruction-vs-explanation-track piece. |
| 13.6 (y3) / 12.6 (v6) | Mills *Racial Contract* | MUST [P] | Light | **MUST-Engage** | Light | Confirmed. Reviewer-expected; not apparatus the user redeploys. (Currently right at Light; flagging for clarity.) |
| K.1 (y3) / 14.1 (v6) | Streeck *Gekaufte Zeit* | MUST [P] | Light | **MUST-Anchor** *for the ECB-economist user* | **Full** | This is the strongest case in the syllabus where the *user's* position changes the tier. Streeck's diagnosis of post-2008 capitalism is apparatus the ECB-economist user can deploy under his own pen with unusual leverage. Full reconstruction is field-importance-justified, not vanity. y3 currently underweights. |
| K.2 (y3) / 14.2 (v6) | Fraser *Cannibal Capitalism* | MUST [P] | Light | MUST-Engage | Light | Confirmed at baseline. (Conditional Full if Phase III is Fraser-track.) |
| K.3 (y3) / 14.4 (v6) | Postone *Time, Labor, Social Domination* | MUST [P] | Light | **MUST-Anchor** *if* Phase III commits to capitalism-as-form; otherwise MUST-Engage | Light → Full conditional | Postone's reinterpretation is apparatus, not coverage. For an economist-user piece on capitalism-as-form (a plausible Phase III terrain given the user's profile), this is Full; otherwise Light. Add §4 trigger. |
| K.6 (y3) / 14.7 (v6) | Honneth *Idee des Sozialismus* | MUST [P] | Light | **MUST-Engage** | Light | Confirmed. Short, programmatic; reviewer-expected for any capitalism-or-Honneth-track piece, but not apparatus. |

**Texts I am genuinely uncertain about**, flagged honestly:

- 7.19 Honneth *Arbeitende Souverän* baseline class — reasonable disagreement exists about whether 2023-recency is enough to make this MUST at 2027 submission. Reviewer-norms in Frankfurt-tradition journals are conservative; *Anerkennung* (2018) settled into canon over ~5 years and *Arbeitende Souverän* may still be in dispute by M42. Holding MUST-Engage but flagging.
- 8.12 Jaeggi *Fortschritt und Regression* — same recency caveat. The argument for baseline MUST is that not engaging Jaeggi's reply to Allen is conspicuous; the argument against is that it may not have full reception by 2027. Flagging.
- K.6b Aglietta — I cannot assess the field-importance of Régulation-school texts for current Sozialphilosophie reception with confidence. The y3 v1.2 deferral to Phase IV looks defensible but I'd defer to scholar correspondence (Vogelmann, Khurana, or someone Régulation-adjacent) before locking in.
- I have **no field-importance knowledge** to defend or contest the y3 classifications for the Appendix F/G (Marxist deepening, socialisation/Bildung) at sub-section level — these are appropriately COULD by default and I will not pretend to a per-text view.

---

## Part 4 — Conflation diagnostics

Three places in the current architecture where importance, tier, and tag are tangled.

**(1) Execution plan Appendix A bypasses y3.** The plan's Appendix A "Default tag → tier mapping" maps syllabus tag *directly* to tier (e.g., [P*] → Full, [P] → Light, [ES] → Light, [O] → Orientation). It cites `reading_practices_v4.md` as canonical and does not pass through y3 at all. This means:

- Every [P*] text is implicitly treated as Full-tier reconstruction, regardless of whether y3 classes it as MUST-Anchor or (per the audit) MUST-Engage. Zurn (8.3), Laitinen-Särkelä (8.4), Jaeggi-Fraser (8.5) get Full by tag despite being apparatus the user *cites*, not *reconstructs*.
- Every [P] is implicitly Light, regardless of whether y3 classes it as MUST-Anchor (where the audit argues for Full). *Phänomenologie* IV.A and Marx *Kapital* ch.1 §4 are the explicit-deviation cases the plan currently flags by ad-hoc rationale; the framework should make these *expected*, not exceptional.

**Recommendation**: rewrite the Appendix A header to make the derivation `y3 importance × syllabus tag → tier`, with y3-importance dominant:

| y3 class | Default tier | Tag-driven exceptions |
|---|---|---|
| MUST-Anchor | Full | (none — the y3 class dominates) |
| MUST-Engage | Light | [O]/[RS] → Orientation |
| SHOULD | Light if [P]/[ES], Orientation if [O]/[RS] | — |
| COULD | Orientation | Promoted by §4 to MUST/SHOULD → adopt tier above |
| DISCR. | skip | — |

The current `reading_practices_v4.md` Practice A tier-routing table (line 77–82) should likewise be revised to route y3-class first, then tag — currently it routes tag-first.

**(2) [P*] tag is over-claiming.** Looking across the syllabus, [P*] in v6 is used for three different things:

- *Tradition-foundational primaries* (Marx *Kapital* §4, Horkheimer 1937, Honneth *KuA*, Jaeggi *KvL*, Jaeggi *Entfremdung*) — anchor function clear
- *Active-frontier monographs/typologies that are reviewer-essential but short* (Zurn 8.3, Laitinen-Särkelä 8.4) — engage function, not anchor
- *Debate volumes* (Fraser-Honneth 7.4, Jaeggi-Fraser 8.5) — engage function

A cleaner v6 retagging could distinguish [P*] for the first category and [P-frontier] or [ES-frontier] for the second/third. Absent that retagging, the y3 sub-split (MUST-Anchor vs. MUST-Engage) must do the work, which it can.

**(3) Conditional promotion in §4 mixes two operations.** The §4 dependency table currently mixes (a) "if topic commits, raise SHOULD/COULD to MUST" and (b) "if topic commits, raise MUST-Engage to MUST-Anchor (Full)." Under the current framework these collapse because MUST has only one tier. Under the proposed split they need to be separated: most topic-commit triggers raise *both* a class-change (some COULDs to MUST-Engage) *and* a tier-upgrade (some MUST-Engages to MUST-Anchor). Listing them in one row hides the second operation. Recommendation: §4 conditional table should have separate columns for class-change and tier-change.

**(4) Tag-overhead for [ES*]/[O*].** v6 uses [ES*] (Neuhouser 1.1, McCarthy 5.1) to mark "the best secondary, on the accelerated path." This conflates two different facts: (a) Neuhouser is the *portal* via which the user controls Hegel's apparatus he will reuse (anchor-secondary), (b) McCarthy is the *guide* via which the user navigates Habermas (orientation-secondary). They should not both be [ES*]. y3 can either ignore the tag and class them MUST-Anchor (Neuhouser) vs. MUST-Engage (McCarthy), or v6 can introduce a finer distinction. The cleaner solution is y3-dominant.

---

## Summary recommendations

1. **Keep MUST / SHOULD / COULD / DISCRETIONARY** as the top-level four-class structure; do not refine it further.
2. **Sub-split MUST into MUST-Anchor (Full) and MUST-Engage (Light)** based on whether the user will reconstruct the text's apparatus under his own pen (Anchor) or know it well enough to cite/characterise (Engage).
3. **Unify the two definitions of "essential" as a disjunction** (Phase III-reviewer-essential ∨ tradition-anchoring) for MUST membership; use the sub-split (Anchor vs. Engage) to capture which definition drives.
4. **Replace y3 §2 tier table** with a y3-class-first derivation rule that allows MUST-Anchor to be Full regardless of tag (capturing *Phän.* IV.A 1.3, Heinrich 2.3, Mead 4A.3, *Recht der Freiheit* 7.5, Streeck K.1) and MUST-Engage to be Light regardless of tag (capturing Zurn 8.3, Laitinen-Särkelä 8.4, Jaeggi-Fraser 8.5).
5. **Rewrite execution plan Appendix A** so tier derives from y3 importance × tag, not tag alone. Currently the plan bypasses y3 and the user is patching with ad-hoc deviation notes.
6. **§4 conditional-promotion table** should distinguish class-changes from tier-upgrades — the two were collapsed because the framework had only one MUST tier.
7. The ~25 text-level revisions in Part 3 are the operational consequence; the bulk are tier-upgrades from Light to Full for genuinely load-bearing apparatus texts (*Phän*. IV.A, *RP*, Heinrich, Mead, *Recht der Freiheit*, Streeck) and tier-downgrades from Full to Light for [P*]-by-tag texts that are reviewer-coverage rather than apparatus (Zurn, Laitinen-Särkelä, Jaeggi-Fraser, possibly McCarthy).
