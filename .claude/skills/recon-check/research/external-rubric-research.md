# External rubric research — philosophy pedagogy, argumentation theory, feedback design

Subagent deliverable, 2026-07-14 (web search + model knowledge, marked). This report is the provenance for the *(ext)*-marked rows and the feedback-design rules of `../rubric.md`. Verification flags in Part 4 are load-bearing: several items are secondary-source or model knowledge and are design choices, not findings.

---

## Part 1: Candidate rubric dimensions

Organized in four clusters: **(A) Fidelity** — did you read it right; **(B) Structure** — did you render it as an argument; **(C) Interpretive calibration** — charity, steelmanning, dialectical placement; **(D) Artifact craft** — is the written reconstruction usable. This ordering itself matters for feedback (see Part 3).

### Cluster A — Fidelity to the text

**A1. Main-claim accuracy (conclusion identification)**
- *What good looks like:* The reconstruction's main claim is the author's actual conclusion, at the author's level of ambition (e.g., a transcendental claim vs. an empirical generalization vs. a diagnosis of a social pathology), stated with the author's scope and modality. Shields (2024) distinguishes **intent-accuracy** (approximates what the author intended the argument to accomplish) from **context-accuracy** (captures audience, genre, historical/polemical situation) — both are necessary conditions of a charitable reconstruction, and a reconstruction fails if it "in any way deviates from or contradicts" the author's intent for the argument.
- *Typical failure:* Substituting a nearby, more familiar thesis (e.g., reading Adorno's critique of identity thinking as a claim about measurement error); stating a sub-conclusion as the main conclusion; stating the topic instead of the claim.
- *Source:* Shields, "Charity Principles in Philosophical Argumentation," *Argumentation* 2024 (https://link.springer.com/article/10.1007/s10503-024-09648-7; full text verified via https://d-nb.info/1368223303/34); Concepción, "Reading Philosophy with Background Knowledge and Metacognition," *Teaching Philosophy* 2004 (https://fr.dawsoncollege.qc.ca/writing/wp-content/uploads/sites/196/Concepcion-Reading-Philosopy.pdf).

**A2. Completeness (no essential premise dropped)**
- *What good looks like:* Every premise the conclusion actually needs is present — including the normative or methodological premises continental authors often carry silently (e.g., the immanent-critique premise that norms invoked are the society's own). Ryu et al. verify reconstructions on exactly this criterion: **completeness** = "all necessary or core premises required to reconstruct an argument are included."
- *Typical failure:* Reconstruction whose stated premises don't reach the conclusion; the gap papered over with "therefore."
- *Source:* Ryu et al., "Argument Reconstruction as Supervision for Critical Thinking in LLMs," arXiv 2603.17432 (https://arxiv.org/pdf/2603.17432; full text verified).

**A3. Parsimony (no imported or inflated material)**
- *What good looks like:* Rhetorical flourishes, illustrations, and asides are excluded unless they carry inferential weight; nothing appears as a premise that the author doesn't rely on. Ryu et al.: **parsimony** = "premises that are unnecessary for supporting the conclusion are excluded"; their error taxonomy includes "unnecessary premises, including rhetorical statements or paraphrased content." Pragma-dialectics licenses this as the **deletion** transformation — but only for material irrelevant to resolving the dispute.
- *Typical failure:* Treating every emphatic sentence as a premise; padding the reconstruction with the author's examples as if they were steps.
- *Source:* Ryu et al. (above); van Eemeren & Grootendorst, pragma-dialectics (overview: https://en.wikipedia.org/wiki/Pragma-dialectics; https://link.springer.com/article/10.1007/s11245-024-10074-3).

**A4. Scope, quantifier, and modality preservation**
- *What good looks like:* Qualifications, hedges, domain restrictions, and modal strength survive the reconstruction ("tends to," "under capitalist conditions," "necessarily" vs. "typically"). Ryu et al.'s verified error taxonomy explicitly names "incorrectly represented premises, including **overly generalized premises**" as a top failure pattern.
- *Typical failure:* Universalizing a qualified claim (Honneth's *Missachtung* claims read as exceptionless laws); dropping a "for us moderns" restriction in Hegel; converting a genealogical claim into an analytic one.
- *Source:* Ryu et al. (verified); the quantifier/modality checklist framing is **model knowledge** (standard in informal-logic textbooks, e.g., Govier's *A Practical Study of Argument* — not verified against the text this session).

**A5. Textual grounding (verifiability of the reading)**
- *What good looks like:* Each load-bearing attribution is anchored to a passage (section/page), so disagreements about the reconstruction can be adjudicated against the text rather than memory. Department rubrics operationalize this as "Use of Sources"; matches the project's own anti-hallucination norm (point to the passage, let the reader verify).
- *Typical failure:* Free-floating attribution; paraphrase that can't be traced to any passage; quote-stitching without anchoring the *inferential* claims (quotes prove the words occurred, not that they play the assigned role in the argument).
- *Source:* University at Buffalo Philosophy grading rubrics (https://www.buffalo.edu/cas/philosophy/undergrad-study/learningoals/ug_rubrics.html) — note their rubric is generic and does *not* explicitly cover charity or reconstruction, a documented gap; the quote-stitching failure mode is **model knowledge**.

### Cluster B — Structural rendering

**B1. Argument structure made explicit (standardization, not paraphrase)**
- *What good looks like:* The reconstruction exhibits inferential architecture: which premises are linked vs. independent (convergent), what each sub-argument establishes, where the main inference happens. Concepción (verified): philosophy is read "for arguments, reasons, and conclusions, not facts, plot or character development" — a summary of *content* is not a reconstruction of *support*.
- *Typical failure:* **Paraphrase-instead-of-structure** — a condensed retelling in textual order with no premise/conclusion discipline; premise/conclusion conflation.
- *Source:* Concepción 2004 (verified); linked/convergent standardization terminology is **model knowledge** (Govier; Freeman's argument-diagramming tradition).

**B2. Enthymeme handling with warrant (the addition discipline)**
- *What good looks like:* Missing premises are supplied — but each supplied premise is (a) flagged as supplied, and (b) warranted by what the author plausibly believed or treated as obvious, not by what would make the argument valid. Lambert & Ulrich (quoted in Shields, verified): the criteria of "obviousness and belief… are not licenses to add whatever premises an argument requires to be valid… they are meant to permit us to add only those propositions that are really presupposed as premises by the arguer." Pragma-dialectics: the **addition** transformation — legitimate only when recoverable from the discourse and context.
- *Typical failure:* Silent gap-filling; supplying the premise *you* would need rather than the one the author uses; refusing to fill any gap and declaring the argument invalid (the uncharitable dual).
- *Source:* Shields 2024, §5, quoting Lambert & Ulrich 1980 (verified); pragma-dialectics transformations; Topoi, "Argument Interpretation and the Implicit Side of Enthymemes" (https://link.springer.com/article/10.1007/s11245-025-10235-y; abstract-level only).

**B3. Transformation discipline generally (the pragma-dialectical audit)**
- *What good looks like:* The four reconstruction operations — **deletion** (drop what's dialectically irrelevant), **addition** (make implicit elements explicit), **substitution** (replace vague/ambiguous formulations with clear ones), **permutation** (reorder into the ideal argument sequence) — each performed only where the discourse warrants it. Every reconstruction error is an *illegitimate* deletion, addition, substitution, or permutation. Substitution is the highest-risk operation for this learner's corpus: replacing Hegel's or Adorno's terms with "clearer" ones can silently replace the concept (e.g., rendering *Herrschaft* as "market power").
- *Typical failure:* Substitution that translates the author into the reader's home idiom (for an economist: incentive/equilibrium vocabulary); permutation that manufactures a linear deduction from a deliberately dialectical or constellational text.
- *Source:* van Eemeren & Grootendorst, *A Systematic Theory of Argumentation*; Springer handbook chapter (https://link.springer.com/rwe/10.1007/978-90-481-9473-5_10). The economist-idiom hazard application is **model knowledge** (mirrors project CLAUDE.md's "flag when misleading" rule).

**B4. Validity/cogency of the reconstructed argument — without fallacy-fixing**
- *What good looks like:* The reconstructed argument is rendered as cogent as the text supports; but if the original argument contains a gap or fallacy, the reconstruction *preserves and flags* it rather than repairing it. Ryu et al. (verified): arguments with formal fallacies "cannot be faithfully reconstructed" into deductively valid form — faithfulness forbids repair. Govier's "modest" charity principle (verified via Shields): don't attribute implausible claims or faulty inferences *unless there is good empirical reason to do so* — where there IS textual reason, the flaw stays in.
- *Typical failure:* The reconstruction is a better argument than the text (evaluation smuggled into exposition); or a lazily invalid rendering the author would disown.
- *Source:* Ryu et al. (verified); Govier, "Uncharitable Thoughts About Charity" (position verified via Shields' quotation, not against Govier's own text).

### Cluster C — Interpretive calibration

**C1. Charity calibrated against accuracy (the central tension)**
- *What good looks like:* The reconstruction sits at the *right point* on the charity-accuracy frontier and says where it sits. The literature is genuinely split; encode the split, not a slogan:
  - **Maximal charity** (Scriven 1976, verified quotation via Shields): "make the best, rather than the worst, possible interpretation."
  - **Sub-maximal/modest charity** (Govier, verified via Shields): maximal charity is "triply ambiguous"; too much charity "distort[s] the argument into something the interpreter finds convincing but that has little to do with what the arguer actually offered."
  - Shields' synthesis (verified): four criteria — (i) accurate translation such that the author would *recognize* it as her own, (ii) fairness to intentions in context, (iii) plausibility to both parties, (iv) preservation or improvement of logical features — with (iv) the one modest theorists sacrifice first ((iv′): preserve only those logical features consistent with (i) and (ii)).
- *Typical failure:* Under-charity (dumbest permitted reading) and over-charity (Shields, verified: "steelmanning may entail strawmanning," citing Aikin & Casey 2022).
- *Source:* Shields 2024 (verified full text); Lewiński, "The Paradox of Charity," *Informal Logic* 2012 (https://informallogic.ca/index.php/informal_logic/article/view/3620/2980; verified full text); *Topoi* 2025 special-issue intro (https://link.springer.com/article/10.1007/s11245-025-10331-z).

**C2. Recognizability (the Rapoport test)**
- *What good looks like:* Dennett's first Rapoport rule: "re-express your target's position so clearly, vividly, and fairly that your target says, 'Thanks, I wish I'd thought of putting it that way.'" Shields (verified) independently derives *recognizability* as a charity criterion. Rubric item: *would the author's best current interpreter accept this as the argument?*
- *Typical failure:* A reconstruction that is clear, valid, and unrecognizable — vocabulary and motivating problem replaced.
- *Source:* Dennett's Rapoport rules — **quoted from secondary sources (Marginalian, Open Culture), not checked against *Intuition Pumps***; Shields 2024 (verified).

**C3. Dialectical placement — the "directed against" slot**
- *What good looks like:* Identifies the actual opponent and point of contention: what position, in what debate, would be refuted if the argument succeeds. Lewiński (verified): charity is *relational* — "an analyst who is charitable to one discussion party easily becomes uncharitable to the other." A reconstruction that strengthens the author by weakening her named opponent has failed at fidelity. Also his verified trade-off: the most defensible reading of a *premise* can make the *overall argument* trivial, and vice versa; placement must consider the whole premises-conclusion complex.
- *Typical failure:* **Wrong opponent**; mistaking the author's reconstruction of an opponent for the author's own view — Concepción (verified): "Try to avoid mistaking charitable elucidation for the author's main argument"; apparent self-contradictions usually mean the reader "fail[ed] to notice a change in 'voice.'" (Frankfurt-specific examples are **model knowledge**.)
- *Source:* Lewiński 2012 (verified); Concepción 2004 (verified).

**C4. Presupposition identification (distinct from premise-supplying)**
- *What good looks like:* Names what the argument *takes for granted rather than argues* — background ontological, normative, or methodological commitments — distinguished from suppressed premises (which do inferential work) and from the interpreter's own commitments. Depth ordering: surface assumptions < framework commitments < what the author *could not give up without the project collapsing*.
- *Typical failure:* Trivia ("assumes language exists"); the reader's objections disguised as the author's assumptions; conflation with enthymematic premises.
- *Source:* Largely **model knowledge**. **No published rubric found that grades presupposition-identification as a separate dimension — a genuine gap; the skill defines its own standard here** (the programme's necessity test fills it).

**C5. Anachronism control (rational vs. historical reconstruction)**
- *What good looks like:* The reconstruction knows which genre it is in. Rorty (verified at overview level): **rational reconstruction** treats "the great dead thinkers… as contemporaries" and is legitimately anachronistic *if* "conducted in full knowledge of its anachronism"; **historical reconstruction** confines itself to what the author could have meant. Doubly relevant here: *Rekonstruktion* is itself a Habermasian method, so deliberate modernization will occur — reward *declared* modernization, penalize *silent* modernization.
- *Typical failure:* Undeclared genre-mixing — decision-theoretic apparatus in Hegel presented as exegesis.
- *Source:* Rorty, "The Historiography of Philosophy: Four Genres" (overview sources only); Habermas connection: **model knowledge**.

### Cluster D — Artifact craft

**D1. Exposition/evaluation separation**
- *What good looks like:* The reconstruction is recognizably *exposition*; evaluation, if present, is quarantined and labeled.
- *Typical failure:* Evaluative adjectives doing silent work inside the exposition ("Adorno's *exaggerated* claim…"); fixing the argument while restating it; the project-specific version — Practice C/H evaluation bleeding into the Practice A artifact.
- *Source:* Raven, Philosophy Rubric, UVic (https://web.uvic.ca/~raven/teaching/Rubric.pdf); Pryor, Guidelines on Writing a Philosophy Paper (https://www.jimpryor.net/teaching/guidelines/writing.html); Buffalo rubrics.

**D2. Own-words rendering (comprehension made visible)**
- *What good looks like:* Load-bearing steps in the learner's own words with the author's *terms of art* retained in the original (German where the concept is language-bound), quotes reserved for passages where exact wording is contested. Concepción (verified): philosophers "stop… to check if they can restate ideas in their own words"; restating is the comprehension test.
- *Typical failure:* Quote-stitching (fluent collage, no evidence of understanding); or full translation into home idiom that loses the concept (see B3).
- *Source:* Concepción 2004 (verified); quote-stitching as named failure: **model knowledge** (précis pedagogy, e.g., WSU précis rubric — not independently verified in detail).

**D3. Declared uncertainty and interpretive alternatives**
- *What good looks like:* Where the text underdetermines the reading, the reconstruction says so and names the fork ("on reading A this premise is transcendental, on reading B genealogical — I take A because §X"). Vorobej (verified via Shields): charity selects the strongest interpretation *consistent with the total body of available evidence* — which presupposes the alternatives were noticed.
- *Typical failure:* False determinacy — one confident reading of a passage the secondary literature reads three ways; no flag where the learner guessed.
- *Source:* Shields 2024 quoting Vorobej 2006 (verified); the "name the fork" operationalization is **synthesis/model knowledge**.

---

## Part 2: Documented failure-mode catalogue

Verified in sources this session:
1. **Overly generalized premises** (scope inflation) — Ryu et al., named error type.
2. **Missing essential premises** — Ryu et al., named error type.
3. **Unnecessary/rhetorical premises included** — Ryu et al., named error type.
4. **Inductive arguments reconstructed as deductive** — Ryu et al. (verified). Frankfurt-relevant variant: dialectical/genealogical arguments forced into deductive standard form.
5. **Fallacy-fixing during reconstruction** — Ryu et al.; Govier's modest-charity position.
6. **Voice confusion** — mistaking the author's charitable elucidation of an opponent for the author's view — Concepción, verified.
7. **Reading for content instead of argument** (summary/paraphrase instead of structure) — Concepción, verified.
8. **Charity distortion** — interpreter rebuilds the argument into what *they* find convincing (Govier via Shields); steelman drifting into strawman (Shields n.27, Aikin & Casey 2022).
9. **Charity asymmetry** — strengthening the author by flattening her opponent — Lewiński, verified.
10. **Unwarranted gap-filling** — supplying premises beyond what the arguer "really presupposed" (Lambert & Ulrich via Shields, verified).

Standard teaching lore, **not verified against a published source this session** (mark as model knowledge): premise/conclusion conflation as frequency-leader among novices; missing qualifications; importing one's own disciplinary vocabulary; sub-conclusion as main conclusion; examples treated as premises. No rigorous empirical taxonomy of reconstruction errors found in the philosophy-teaching literature; best empirical anchor is the LLM-evaluation literature (Ryu et al.), which converged on accuracy/completeness/parsimony independently — a striking triangulation with the pedagogy.

---

## Part 3: Recommendations for feedback structure

**1. Frame every piece of feedback around Hattie & Timperley's three questions.** Feed-up (what does a frontier-quality reconstruction of *this text* look like — instantiate the rubric for the text, don't recite it), feed-back (where this reconstruction stands), feed-forward (what to do differently on the next text). Their four levels — task, process, self-regulation, self — carry the key design rule: **task-level corrections fix this artifact; process- and self-regulation-level comments transfer to the next text. Self-level comments (praise of the person) do nothing or harm.** Source: Hattie & Timperley, "The Power of Feedback," *RER* 2007 (https://conselhopedagogico.tecnico.ulisboa.pt/files/sites/32/hattie-and-timperley-2007.pdf); meta-analytic confirmation: Wisniewski et al. 2019 (https://www.frontiersin.org/journals/psychology/articles/10.3389/fpsyg.2019.03087/full).

**2. Order findings by epistemic severity, not textual order.** Severity ladder (**synthesis**; components sourced): (i) fidelity errors (comprehension failed); (ii) structural errors (comprehension probable, rendering failed); (iii) calibration errors; (iv) artifact errors. Labeling the layer implements "separate comprehension errors from writing errors."

**3. Limit the count; deliver in manageable units.** Shute (verified): feedback should be specific, task-focused, "present elaborated feedback in manageable units… small enough pieces so that it is not overwhelming and discarded." Practical rule: 2–4 developed points plus at most a short residual list (the 2–4 number is convention/**model knowledge**; the manageable-units principle is sourced). Source: Shute, "Focus on Formative Feedback," *RER* 2008 (https://journals.sagepub.com/doi/10.3102/0034654307313795).

**4. Calibrate severity explicitly; do not mitigate by sandwiching.** Kluger & DeNisi (verified): over one-third of feedback interventions *lowered* performance; effects degrade as attention moves from task to self; praise attached to cognitively demanding tasks impaired performance. Hyland & Hyland (verified): cushioning praise reads as insincere and gets discounted; hedged criticism gets missed. The experimentally supported alternative is **wise feedback** — explicit high standards plus explicit assurance the learner can meet them. Sources: Kluger & DeNisi 1996; Hyland & Hyland, "Sugaring the Pill," 2001; Cohen, Steele & Ross 1999, "The Mentor's Dilemma"; Yeager et al. 2014 (https://sparq.stanford.edu/solutions/wise-critiques-help-students-succeed).

**5. End with transfer rules, not just local fixes.** Every substantive point closes with a process-level "rule for next time." Sadler: the learner must come to hold the *concept of the standard* and apply it to their own production — feedback that only fixes the artifact keeps evaluative expertise with the assessor ("artificial performance ceiling"). Nicol & Macfarlane-Dick: facilitate self-assessment; occasionally ask the learner to run a named rubric dimension on their own draft before revealing the assessment. Sources: Sadler 1989 (https://michiganassessmentconsortium.org/wp-content/uploads/Formative-Assessment-and-Design-of-Instructional-Systems.pdf); Nicol & Macfarlane-Dick 2006 (https://www.psy.gla.ac.uk/~steve/rap/docs/nicol.dmd.pdf).

**6. Use the Rapoport sequence for the feedback's own rhetoric.** Before criticizing the reconstruction, demonstrate it was understood — one or two sentences re-expressing what the learner's reading gets right and what it was trying to do. Doubles as a check that the *feedback-giver* isn't strawmanning the learner. Source: Dennett via secondary sources.

---

## Part 4: Verification flags

- **Could not verify:** a 5-point "definitely faithful → definitely not faithful" rubric scale attributed to Ryu et al. by a search summary — not in the extractable text of arXiv 2603.17432. Do not cite it. The accuracy/completeness/parsimony triad and the three-type error taxonomy **are** verified in that paper's text.
- **Secondary-source only:** Dennett's Rapoport rules wording; Scriven 1976 and Govier 1981/1989 positions (verified as quoted inside Shields 2024, not against the originals); Rorty's four-genres chapter (overview sources only).
- **Abstract-level only:** Lemanek, "Foregoing Charity in the Classroom," *Argumentation* 2025 (argues for teaching the *interpretive competence underlying* charity rather than the principle as slogan); Stevens, "Avoiding Toxic Charity in Argumentation" (title-level only).
- **Genuine gaps in the literature:** (a) no published rubric separately grades presupposition-identification — the skill defines its own standard (the programme's necessity test); (b) empirical documentation of student reconstruction failure modes is thin — the catalogue rests on textbook lore, Concepción's practitioner observations, and the LLM-evaluation taxonomy; (c) the Buffalo department rubric is generic — detailed reconstruction-specific criteria come from argumentation theory, not from any single published teaching rubric. Mara Harrell's CMU rubric and fairness/charity principles are cited via Shields; the rubric file itself was not parsed.
- **Model knowledge, clearly load-bearing:** the Frankfurt-specific failure examples, the Habermas *Rekonstruktion* connection, the economist-idiom substitution hazard, and the severity ladder. All defensible but marked as design choices, not findings.
