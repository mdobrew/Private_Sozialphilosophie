# Text classification (master reference)

This is the canonical mapping of every text in [sozialphilosophie_syllabus.md](sozialphilosophie_syllabus.md) to a prose-difficulty class plus chapter/section count. Used by downstream agents to compute per-text hour budgets via the formula:

`Total Hrs = (Pages ÷ pp/h) + α × reading_hrs`

where pp/h and α (writing-time multiplier per tier) are class-dependent per [execution_plan.md](execution_plan.md) Appendix C (reading pacing norms) and Appendix A (tier overheads). Bottom-of-range pp/h figures (the fast end) are listed below per the calibration anchor in [session_state.md](session_state.md).

---

## Classification framework

Five prose-difficulty classes, bottom-of-range pp/h:

| Class | DE pp/h | EN pp/h | Indicative authors |
|---|---|---|---|
| **Dense** | 4–5 | 5–6 | Hegel (RP, Phän), Marx (Kapital, ÖpM), Adorno (DdA, MM, ND), Lukács, Mannheim, Horkheimer 1937, Weber methodological essays, Husserl |
| **Systematic** | 6–8 | 8–10 | Habermas (TKH, EuI, *Philosophische Diskurs*), Gadamer, Forst monographs (RauR, *Normativität und Macht*, *Noumenal Republic*), Honneth monographs (KuA, RdF, *Anerkennung* 2018, *Arbeitende Souverän*), Khurana, Postone, Luhmann, Bourdieu monographs, Schütz, Boltanski/Thévenot |
| **Layered** | 8–10 | 10–13 | Honneth essays (*Pathologien*, "Anerkennung als Ideologie"), Jaeggi (*Entfremdung*, KvL, *Fortschritt und Regression*), Celikates, Rosa, Renault, Stahl, Joas, Bedorf, Allen, Boltanski, Heinrich, Reckwitz, Federici, Beckert, Vogelmann, Wright, Brown, Henning, Heller, Márkus, Kosík, Heydorn, Mollenhauer, Freud, Nietzsche (*Genealogie*), Marcuse, Fromm, Mitscherlich |
| **Analytic** | 12–15 | 14–18 | Forst articles (Noumenal Power), Fricker, Fraser articles, Zurn, Laitinen-Särkelä, Taylor, Hollis, Mead, Woodward, Anderson, Mills, List & Pettit, Epstein, Pettit, Cohen, Roemer, Putnam, Hempel, Elster, Coady, Searle, Bratman, Gilbert, Tuomela, Hindriks, Bicchieri, Hodgson, Guala, Hartsock, Harding, Khalidi, Hacking, Sugden, Reiss, Hausman, Goldman, Lackey, Felitti, Frega, Stojanov, Drerup/Schweiger, English |
| **Transparent** | 15–18 | 15–20 | Neuhouser, McCarthy, Outhwaite, Feenberg, Jay, Dewey, Polanyi, Streeck, Pippin, Wood, Heinrich (intro text), Wiggershaus, Ringer, Freyenhagen, Hickel, Sennett, Bauman, Bell, Beck, Schimank/Volkmann, Joas/Knöbl, Hurrelmann/Bauer, Siegler textbook, Bowlby, Cassidy/Shaver, Vygotsky, Gerhardt, Shonkoff/Phillips, Freeman, Sayer, Bhaskar, SEP entries, Routledge handbooks, Graeber, Scott, Mbembe (relatively), Mignolo (relatively) |

**Special rules:**
1. **Heinrich** *Kritik der politischen Ökonomie* (2.3) → **Transparent** (deliberate intro text; ~14 pp/h)
2. **Weber** 3.1 "Wissenschaft als Beruf" + 3.2 "Objektivität" → **Dense** (slow methodological prose); 3.3 *W&G* I.1 §§1–17 → **Systematic**
3. **Honneth** split: monographs → Systematic; essays → Layered
4. **Aphoristic structure** is a *flag* (column Flag = `Aphoristic`), not a class — applied to Benjamin "Theses on History" + Adorno *Minima Moralia* (both kept Dense). Benjamin "Kunstwerk" = Dense essay, no flag.

**Flag conventions:**
- `Aphoristic` — non-systematic, fragmentary structure
- `(est)` after pages — page count estimated, not in syllabus
- `(?)` — page count unknown

**n_chapters:** scope as scheduled per syllabus. "chs. 1–5" → 5; "Intro + chs. 1–3" → 4; single essay → 1; "Part I, chs. 1–2" → 2; orientation/reference-only entries → 1 (treated as one notional section).

---

## Part 0 / Orientation

| ID | Author | Title | Lang | Pages | Class | Flag | n_chapters | Notes |
|---|---|---|---|---|---|---|---|---|
| 0.1 | Celikates & Jaeggi | Sozialphilosophie: Eine Einführung | DE | ~250 | Layered | | 7 | Standard intro; modular by question. |
| 0.2 | Honneth | Pathologien des Sozialen (essay) | DE | ~25 | Layered | | 1 | Single programmatic essay. |
| 0.3 | Jaeggi | What (if Anything) Is Wrong with Capitalism? | EN | ~25 | Layered | | 1 | Standalone article / book chapter. |
| 0.4 | Jay | The Dialectical Imagination, chs. 1–3 | EN | ~150 | Transparent | | 3 | Anglophone intellectual history. |

---

## Part I — Historical Foundations

### Module 1: Hegel

| ID | Author | Title | Lang | Pages | Class | Flag | n_chapters | Notes |
|---|---|---|---|---|---|---|---|---|
| 1.1 | Neuhouser | Foundations of Hegel's Social Theory | EN | ~300 | Transparent | | 8 (est) | Estimated chapter count from a ~300pp analytical monograph. |
| 1.2 | Hegel | Grundlinien der Philosophie des Rechts (Preface, §§1–33, §§142–360) | DE | ~320 | Dense | | 4 | Preface + §§1–33 (will) + §§142–256 (Civil Society/Family) + §§257–360 (State). |
| 1.3 | Hegel | Phänomenologie des Geistes ch. IV.A | DE | ~30 | Dense | | 1 | Single section (master-slave dialectic). |
| 1.4 | Pippin | Hegel's Practical Philosophy, chs. 1–4 | EN | ~200 | Transparent | | 4 | [NE]. |
| 1.5 | Wood | Hegel's Ethical Thought, chs. 1–4, 10–14 | EN | ~250 | Transparent | | 9 | [NE]. 4 + 5 chs. |
| 1.6 | Khurana | Das Leben der Freiheit, Einleitung only | DE | ~20 | Systematic | | 1 | **[Backfilled 2026-07-13 (propagation pass):** row corrected from "Intro + Part I, ~150pp" per the 2026-07-12 syllabus revision — the Hegelian reconstruction is *Teil II*, not "Part I"; Module 1 now reads the *Einleitung* only (orientation tier), and the substantive read is the 1.6F pre-block row below.] Suhrkamp monograph; Khurana's prose is dense-systematic. |
| 1.6F | Khurana | Das Leben der Freiheit, Einleitung-recap + Teil II (chs. III–V + Schluss) — Module 7 Kant→Khurana pre-block | DE | ~230 | Systematic | | 4 | **[Backfilled 2026-07-13 (propagation pass).]** The *Teil II* read deferred from Module 1 per syllabus 1.6 (2026-07-12); scheduled at the Module 7 pre-block (M20–21, opt-in) with Kant prerequisites I.1.5 + I.1.7 (Appendix I section below). Same class as 1.6. |
| 1.7 | Honneth | Leiden an Unbestimmtheit | DE | ~130 | Systematic | | 3 (est) | **[Added 2026-07-13 (coverage audit).]** Special rule #3 — Honneth monograph → Systematic. Lecture-based, ~3 parts. |

### Module 2: Marx

| ID | Author | Title | Lang | Pages | Class | Flag | n_chapters | Notes |
|---|---|---|---|---|---|---|---|---|
| 2.1 | Marx | ÖpM, "Entfremdete Arbeit" | DE | ~40 | Dense | | 1 | Single essay/manuscript fragment. |
| 2.2a | Marx | Das Kapital Bd. 1 ch. 1 §§1–4 | DE | ~40 | Dense | | 4 | Per syllabus & session_state: 4 sub-sections; the fetishism §4 is its own unit. |
| 2.2b | Marx | Das Kapital Bd. 1 chs. 2–3 + ch. 10 | DE | ~160 | Dense | | 3 | Chs. 2, 3, 10. |
| 2.3 | Heinrich | Kritik der politischen Ökonomie, chs. 1–5 | DE | ~200 | Transparent | | 5 | Special rule #1 — Heinrich is an intro text. |
| 2.4 | Wood | Karl Marx, chs. 1–4, 9–12 | EN | ~250 | Transparent | | 8 | [NE]. |
| 2.5 | Marx & Engels | Die deutsche Ideologie (Feuerbach-chapter selections) + Thesen über Feuerbach | DE | ~45 | Dense | | 2 (est) | **[Added 2026-07-13 (coverage audit).]** Marx primary → Dense per framework; Feuerbach selections + Thesen as 2 units. Read between 2.1 and 2.2a. |

### Module 3: Weber

| ID | Author | Title | Lang | Pages | Class | Flag | n_chapters | Notes |
|---|---|---|---|---|---|---|---|---|
| 3.1 | Weber | Wissenschaft als Beruf | DE | ~30 | Dense | | 1 | Special rule #2 — methodological prose, dense. |
| 3.2 | Weber | Die "Objektivität" sozialwissenschaftlicher und sozialpolitischer Erkenntnis | DE | ~60 | Dense | | 1 | Special rule #2. |
| 3.3 | Weber | Wirtschaft und Gesellschaft I.1 (§§1–17) | DE | ~80 | Systematic | | 1 | Special rule #2 — definitional / structured. |
| 3.4 | Ringer | Max Weber: An Intellectual Biography, chs. 1–5 | EN | ~200 | Transparent | | 5 | [NE]. |

### Module 3A: Lukács

| ID | Author | Title | Lang | Pages | Class | Flag | n_chapters | Notes |
|---|---|---|---|---|---|---|---|---|
| 3A.1 | Lukács | Geschichte und Klassenbewußtsein, "Verdinglichung" | DE | ~100 | Dense | | 3 | Three sections per syllabus. |
| 3A.2 | Feenberg | The Philosophy of Praxis, chs. 3–5 | EN | ~100 | Transparent | | 3 | |

### Module 4: First Frankfurt School

| ID | Author | Title | Lang | Pages | Class | Flag | n_chapters | Notes |
|---|---|---|---|---|---|---|---|---|
| 4.1 | Horkheimer | Traditionelle und kritische Theorie | DE | ~40 | Dense | | 1 | Programmatic essay. |
| 4.2 | Horkheimer & Adorno | DdA, "Begriff der Aufklärung" + Exkurs I | DE | ~80 | Dense | | 2 | |
| 4.3 | Pollock | State Capitalism | EN | ~20 | Layered | | 1 | Pollock is more readable than Adorno; placed Layered, not Dense. |
| 4.4 | Adorno | Minima Moralia, §§1–18, 29, 36, 67–68, 153 | DE | ~50 | Dense | Aphoristic | 1 | Special rule #4 — aphoristic flag; treated as one selection. |
| 4.5 | Adorno | Negative Dialektik, Intro + Part III | DE | ~100 | Dense | | 2 | Intro + Meditationen zur Metaphysik. |
| 4.6 | Freyenhagen | Adorno's Practical Philosophy, chs. 1–5 | EN | ~200 | Transparent | | 5 | Analytic-clear despite Adorno-content. |
| 4.7 | Wiggershaus | Die Frankfurter Schule, ch. 7 | DE | ~60 | Transparent | | 1 | |
| 4.8 | Marcuse | One-Dimensional Man, chs. 1–6 | EN | ~200 | Layered | | 6 | Thesis-driven but conceptually layered; not transparent prose. |
| 4.9 | Benjamin | Über den Begriff der Geschichte (Theses) | DE | ~15 | Dense | Aphoristic | 1 | Special rule #4 — aphoristic flag. |
| 4.10 | Benjamin | Das Kunstwerk im Zeitalter seiner technischen Reproduzierbarkeit | DE | ~40 | Dense | | 1 | Special rule #4 — Kunstwerk essay = Dense, no aphoristic flag. |
| 4.11 | Adorno | Drei Studien zu Hegel ("Aspekte" + "Skoteinos") | DE | ~120 | Dense | | 3 | **[Backfilled 2026-06-27 — present in syllabus/phase3 but absent from this table.]** Adorno → Dense per framework. |
| 4.12 | Freud | Das Unbehagen in der Kultur | DE | ~80 | Layered | | 8 | **[Added 2026-06-27.]** Eight untitled sections. Freud's prose is lucid (Goethe-Prize stylist) but the argument is conceptually layered — Layered, not Dense. See borderline note. |
| 4.13 | Nietzsche | Zur Genealogie der Moral, Abhandlungen I–II | DE | ~90 | Layered | | 2 | **[Added 2026-06-27.]** Two continuous essays (not aphoristic — no flag). Reads fast but argument-dense; borderline Dense — see note. |
| 4.14 | Benjamin + Horkheimer | *Lebensphilosophie* reckoning (thread): Benjamin, "Über einige Motive bei Baudelaire" §§I–III + Horkheimer, "Zu Bergsons Metaphysik der Zeit" | DE | ~70 | Dense | | 2 | **[Backfilled 2026-07-13 (propagation pass).]** Syllabus 4.14 (added 2026-07-12). **Bonus thread, not a scheduled slot — not in any hour baseline** (headroom/Phase IV; conditional MUST-Engage only if Track D Adornian-negativism commits). Benjamin essay → Dense (cf. 4.10 Kunstwerk, no aphoristic flag); Horkheimer → Dense per framework. The Jay *Songs of Experience* chapters and the *Lebensphilosophie* trunk (Bergson/Dilthey/Simmel/Klages) are map-only — no rows. |
| 4.15 | Neumann | Behemoth (selections on totalitarian monopoly capitalism) | EN | ~25 | Layered | | 1 (est) | **[Added 2026-07-13 (coverage audit).]** Written in English. Institutional-economic Frankfurt analysis; clearer prose than Adorno — Layered, cf. Pollock 4.3. |

### Module 4A: Pragmatism

| ID | Author | Title | Lang | Pages | Class | Flag | n_chapters | Notes |
|---|---|---|---|---|---|---|---|---|
| 4A.1 | Dewey | The Public and Its Problems | EN | ~200 | Transparent | | 6 (est) | Dewey's prose is unusually transparent for the period. |
| 4A.2 | Joas | Die Kreativität des Handelns, chs. 1–5 | DE | ~200 | Layered | | 5 | |
| 4A.3 | Mead | Mind, Self, and Society, Part III | EN | ~100 | Analytic | | 1 | Mead is analytic in framework though dated prose; treat as one part. |
| 4A.4 | Dewey | Logic: The Theory of Inquiry, chs. 1–6 | EN | ~150 | Transparent | | 6 | [RS]. |
| 4A.5 | Frega | Pragmatism and the Wide View of Democracy, chs. 1–4 | EN | ~150 | Analytic | | 4 | [RS]. |

### Module 5: Positivismusstreit / Hermeneutics Debate

| ID | Author | Title | Lang | Pages | Class | Flag | n_chapters | Notes |
|---|---|---|---|---|---|---|---|---|
| 5.1 | McCarthy | The Critical Theory of Jürgen Habermas, chs. 1–3 | EN | ~150 | Transparent | | 3 | |
| 5.2 | Habermas | Erkenntnis und Interesse, chs. 1–3 + Nachwort | DE | ~200 | Systematic | | 4 | |
| 5.3 | Adorno + Habermas | Positivismusstreit, two contributions | DE | ~40 | Dense | | 2 | Adorno's "Zur Logik der Sozialwissenschaften" + Habermas's contribution. |
| 5.4 | Gadamer | Wahrheit und Methode, Part II chs. 1–2 | DE | ~150 | Systematic | | 2 | |
| 5.5 | Habermas | Zur Logik der Sozialwissenschaften, selections / "Universalitätsanspruch der Hermeneutik" | DE | ~60 | Systematic | | 1 | Selection treated as one essay-unit. |

---

## Part II — Systematic Core

### Module 6: Habermas

| ID | Author | Title | Lang | Pages | Class | Flag | n_chapters | Notes |
|---|---|---|---|---|---|---|---|---|
| 6.1 | Outhwaite | Habermas: A Critical Introduction, chs. 3–6 | EN | ~120 | Transparent | | 4 | |
| 6.2 | McCarthy | Critical Theory of Habermas, chs. 4–5 | EN | ~80 | Transparent | | 2 | |
| 6.3 | Habermas | TKH Bd. 1 ch. I | DE | ~80 | Systematic | | 1 | |
| 6.4 | Habermas | TKH Bd. 1 chs. II–III | DE | ~200 | Systematic | | 2 | [RS] — Weber + Frankfurt School reconstructions. |
| 6.5 | Habermas | TKH Bd. 2 ch. VI + ch. VIII | DE | ~150 | Systematic | | 2 | |
| 6.6 | Habermas | Faktizität und Geltung, chs. 1–4 | DE | ~200 | Systematic | | 4 | [NE]. |
| 6.9 | Habermas | Diskursethik — Notizen zu einem Begründungsprogramm | DE | ~75 (est) | Systematic | | 1 | **[Added 2026-07-13 (coverage audit).]** Habermas → Systematic per framework; single long programmatic essay (~60–90pp). Read between 6.5 and 6.6. |

### Module 7: Honneth

| ID | Author | Title | Lang | Pages | Class | Flag | n_chapters | Notes |
|---|---|---|---|---|---|---|---|---|
| 7.1 | Honneth | Kampf um Anerkennung | DE | ~250 | Systematic | | 9 | Special rule #3 — monograph → Systematic. ~9 chapters per standard Suhrkamp text. |
| 7.2 | Honneth | Anerkennung als Ideologie (essay) | DE | ~30 | Layered | | 1 | Special rule #3 — essay → Layered. |
| 7.3 | Fraser | From Redistribution to Recognition? (NLR article) | EN | ~25 | Analytic | | 1 | Fraser articles → Analytic. |
| 7.4 | Fraser & Honneth | Umverteilung oder Anerkennung? | DE | ~300 | Systematic | | 4 (est) | Co-authored debate volume; treated as 4 sections (2 essays + 2 replies). |
| 7.5 | Honneth | Das Recht der Freiheit (selections) | DE | ~150 | Systematic | | 3 | Methodological intro + Persönliche Beziehungen + Der Markt. |
| 7.6 | Honneth | Verdinglichung (OUP 2008 Tanner ed., incl. Butler/Geuss/Lear commentaries + reply) | DE/EN | ~130 | Layered | | 5 (est) | [ES]. Essay-length monograph; Layered. **[Updated 2026-07-13 (coverage audit):** Tanner-Lectures edition — +~50pp for the three commentaries + Honneth's reply (commentaries in English); n_chapters 1 → 5 (lecture text + 3 commentaries + reply). Marker also corrected [NE] → [ES] per syllabus revision 2026-05-22.] |
| 7.7 | Forst | Das Recht auf Rechtfertigung, chs. 1–4 | DE | ~150 | Systematic | | 4 | Forst monographs → Systematic. |
| 7.8 | Forst | Noumenal Power (article) | EN | ~25 | Analytic | | 1 | Forst article → Analytic. |
| 7.9 | Forst | Normativität und Macht, Part I + further chs. | DE/EN | ~180 | Systematic | | 5 (est) | Forst monograph. |
| 7.10 | Forst | The Noumenal Republic, Intro + Parts I–II | EN | ~200 | Systematic | | 6 (est) | Forst monograph. Selection from Polity 2024. |
| 7.11 | Benjamin | The Bonds of Love, chs. 1–3 | EN | ~100 | Layered | | 3 | |
| 7.12 | Fraser | Rethinking the Public Sphere (article) | EN | ~30 | Analytic | | 1 | |
| 7.13 | Renault | Souffrances sociales / Leiden an der Gesellschaft | DE/FR | ~200 | Layered | | 5 (est) | Phenomenological-empirical apparatus; Layered. |
| 7.14 | Taylor | "The Politics of Recognition" | EN | ~50 | Analytic | | 1 | **[Added 2026-06-27.]** Single essay (Gutmann volume). Taylor → Analytic per framework; cf. 10.3. |
| 7.15 | Ikäheimo & Laitinen eds. | Recognition and Social Ontology (Intro + chs.) | EN | ~150 | Analytic | | 4 (est) | Analytic social-ontology in recognition idiom. |
| 7.16 | Gregoratto | Selected essays on recognition & affect | EN | ~60 | Layered | | 3 (est) | 2–3 articles. |
| 7.17 | Bedorf | Verkennende Anerkennung, chs. 1–3 | DE | ~120 | Layered | | 3 | Phenomenological-Levinasian register. |
| 7.18 | Honneth | Anerkennung: Eine europäische Ideengeschichte (selections) | DE | ~250 | Systematic | | 5 | Intro + 3 tradition chs. (French / British / German) + concluding systematic chapter. |
| 7.19 | Honneth | Der arbeitende Souverän (Einleitung + Teil II + Schluss) | DE | ~250 | Systematic | | 5 (est) | Einleitung + Teil II (~3 chs.) + Schluss; Special rule #3. |
| 7.22 | Jütten | Is the Market a Sphere of Social Freedom? (article) | EN | ~25 | Analytic | | 1 | [Relocated from 8.10, 2026-05-29 — Honneth item.] |
| 7.23 | Neuhouser | Honneth's Theory of Social Freedom (essay) | EN | ~30 | Analytic | | 1 | [Relocated from 8.11, 2026-05-29.] Single essay in edited volume. |
| 7.24 | Herzog | Inventing the Market (selections) | EN | ~150 (est) | Analytic | | 4 (est) | **[Added 2026-07-13 (coverage audit).]** OUP analytical political theory / philosophy of economics; Analytic (conservative — clear prose but argument-dense). |

### Module 8: Jaeggi

| ID | Author | Title | Lang | Pages | Class | Flag | n_chapters | Notes |
|---|---|---|---|---|---|---|---|---|
| 8.1 | Jaeggi | Entfremdung | DE | ~200 | Layered | | 5 (est) | |
| 8.2 | Jaeggi | Kritik von Lebensformen | DE | ~350 | Layered | | 10 | Per syllabus emphasis on chs. 1–3 + 8–10; full text has ~10 chs. |
| 8.3 | Zurn | Social Pathologies as Second-Order Disorders (essay) | EN | ~30 | Analytic | | 1 | |
| 8.4 | Laitinen & Särkelä | Four Conceptions of Social Pathology | EN | ~20 | Analytic | | 1 | |
| 8.5 | Jaeggi & Fraser | Capitalism: A Conversation in Critical Theory | EN | ~200 | Layered | | 4 (est) | Dialogue + responses. |
| 8.6 | Allen | The End of Progress, chs. 1–3 + 6 | EN | ~150 | Layered | | 4 | |
| 8.7 | Menke | Kritik der Rechte, Intro + Part I | DE | ~120 | Layered | | 4 (est) | [NE]. Adornian register; Layered. |
| 8.8 | Stahl | Immanente Kritik, chs. 1–4 | DE | ~200 | Layered | | 4 | |
| 8.9 | Rosa | Resonanz, Intro + Part I + Part IV | DE | ~200 | Layered | | 6 (est) | Intro + chs. 1–3 + chs. 12–13. |
| 8.12 | Jaeggi | Fortschritt und Regression | DE | ~252 | Layered | | 6 (est) | Suhrkamp 2023; multi-part structure. |
| 8.13 | Allen & Mendieta eds. | From Alienation to Forms of Life (selected essays) | EN | ~150 | Layered | | 5 (est) | [Relocated from 7.14, 2026-05-29 — Jaeggi volume.] Mixed essays — Layered as composite. |

### Module 8A: Außereuropäische Kritik

| ID | Author | Title | Lang | Pages | Class | Flag | n_chapters | Notes |
|---|---|---|---|---|---|---|---|---|
| 8A.1 | Said | Orientalism, Introduction | EN | ~30 | Layered | | 1 | Introduction only. |
| 8A.2 | Chakrabarty | Provincializing Europe, Intro + ch. 1 | EN | ~80 | Layered | | 2 | |
| 8A.3 | Spivak | Can the Subaltern Speak? | EN | ~40 | Layered | | 1 | Dense rhetorical-theoretical prose — borderline Dense; Layered consistent with module-typical pace. |
| 8A.4 | Quijano | Coloniality of Power, Eurocentrism, and Latin America | EN | ~30 | Layered | | 1 | |
| 8A.5 | Mignolo | The Darker Side of Western Modernity, Intro + chs. 1–2 | EN | ~80 | Layered | | 3 | |
| 8A.6 | Robinson | Black Marxism, Foreword + chs. 1 + 11 | EN | ~120 | Layered | | 3 | Historical-theoretical mix. |
| 8A.7 | Wilderson | Afropessimism, Intro + chs. 1–2 | EN | ~120 | Layered | | 3 | |
| 8A.8 | Mbembe | Critique de la raison nègre, Intro + chs. 1, 6 | FR/EN | ~100 | Transparent | | 3 | Mbembe's prose is comparatively clear; Transparent. |
| 8A.9 | Fanon | Peau noire, masques blancs, ch. 5 + Hegel section of ch. 7 | FR/DE/EN | ~50 (est) | Layered | | 2 | **[Added 2026-07-13 (coverage audit).]** Original French; read in DE/EN translation. Phenomenological-essayistic; Layered, consistent with module. ~40–60pp edition-dependent. |

---

## Part III — Instrumental Readings

### Module 9: Social Epistemology

| ID | Author | Title | Lang | Pages | Class | Flag | n_chapters | Notes |
|---|---|---|---|---|---|---|---|---|
| 9.1 | Mannheim | Ideologie und Utopie, Part I | DE | ~100 | Dense | | 1 | Mannheim's prose is genuinely dense per framework. |
| 9.2 | Fricker | Epistemic Injustice | EN | ~180 | Analytic | | 7 (est) | Standard Oxford monograph. |
| 9.3 | Celikates | Kritik als soziale Praxis | DE | ~250 | Layered | | 7 (est) | |
| 9.4 | Jaeggi | Was ist Ideologiekritik? (essay) | DE | ~30 | Layered | | 1 | |
| 9.5 | Shelby | Ideology, Racism, and Critical Social Theory | EN | ~25 | Analytic | | 1 | |
| 9.6 | Vogelmann | Die Wirksamkeit des Wissens (Intro + Parts II + conclusion) | DE | ~180 | Layered | | 4 (est) | |
| 9.7 | Boltanski | De la critique, chs. 1–4 | FR/EN | ~180 | Layered | | 4 | |
| 9.8 | Hartsock | The Feminist Standpoint (essay) | EN | ~30 | Analytic | | 1 | |
| 9.9 | Harding | Whose Science? Whose Knowledge?, chs. 1–3 | EN | ~80 | Transparent | | 3 | [O]; Harding's prose is clear. |
| 9.10 | Hill Collins | Black Feminist Thought, Intro + chs. 1, 5, 11 | EN | ~150 | Layered | | 4 | |

### Module 10: Philosophy of Social Science

| ID | Author | Title | Lang | Pages | Class | Flag | n_chapters | Notes |
|---|---|---|---|---|---|---|---|---|
| 10.1 | Hollis | The Philosophy of Social Science: An Introduction | EN | ~200 | Analytic | | 8 (est) | Textbook; analytic register. |
| 10.2 | Woodward | Making Things Happen, chs. 1–3 | EN | ~150 | Analytic | | 3 | |
| 10.3 | Taylor | Interpretation and the Sciences of Man | EN | ~40 | Analytic | | 1 | |
| 10.4 | Winch | The Idea of a Social Science, chs. 1–3 | EN | ~120 | Analytic | | 3 | [NE]. |
| 10.5 | Cartwright | Hunting Causes and Using Them, chs. 1–3 | EN | ~100 | Analytic | | 3 | [NE]. |

### Module 11A: Foucault

| ID | Author | Title | Lang | Pages | Class | Flag | n_chapters | Notes |
|---|---|---|---|---|---|---|---|---|
| 11A.1 | Foucault | Surveiller et punir, Part I + Part III ch. 3 | FR/DE/EN | ~150 | Layered | | 2 | Part I + the panopticism chapter. |
| 11A.2 | Foucault | "Il faut défendre la société" (Lecture 14 Jan 1976) | FR/EN | ~25 | Layered | | 1 | Single lecture. |
| 11A.3 | Habermas | Der philosophische Diskurs der Moderne, Lectures IX–X | DE | ~100 | Systematic | | 2 | Habermas monograph register. |
| 11A.4 | Allen | Power, Subjectivity, and Agency (article) | EN | ~25 | Analytic | | 1 | |
| 11A.5 | Foucault | Naissance de la biopolitique (ordoliberalism lectures, ~2 lectures) | FR/DE/EN | ~50 (est) | Layered | | 2 | **[Added 2026-07-13 (coverage audit).]** Lecture prose — Layered, consistent with 11A.2. |

### Module 11B: Luhmann

| ID | Author | Title | Lang | Pages | Class | Flag | n_chapters | Notes |
|---|---|---|---|---|---|---|---|---|
| 11B.1 | Horster | Niklas Luhmann (intro) | DE | ~150 | Transparent | | 5 (est) | Compact intro. |
| 11B.2 | Luhmann | Soziale Systeme, chs. 1–2 | DE | ~100 | Systematic | | 2 | Luhmann is dense-and-structured; Systematic. |
| 11B.3 | Habermas & Luhmann | Theorie der Gesellschaft oder Sozialtechnologie (Habermas's contributions) | DE | ~80 | Systematic | | 2 (est) | |

### Module 11C: Bourdieu

| ID | Author | Title | Lang | Pages | Class | Flag | n_chapters | Notes |
|---|---|---|---|---|---|---|---|---|
| 11C.1 | Bourdieu | Le sens pratique, Book I | FR/DE/EN | ~150 | Systematic | | 4 (est) | Bourdieu monograph → Systematic. |
| 11C.2 | Bourdieu | La distinction, Intro + Part I | FR/DE/EN | ~120 | Systematic | | 2 | |
| 11C.3 | Reckwitz | Toward a Theory of Social Practices (article) | EN | ~25 | Analytic | | 1 | |
| 11C.4 | Boltanski & Thévenot | De la justification, Intro + chs. 1–3 | FR/EN | ~150 | Systematic | | 4 | |

### Module 11D: Critical Realism

| ID | Author | Title | Lang | Pages | Class | Flag | n_chapters | Notes |
|---|---|---|---|---|---|---|---|---|
| 11D.1 | Sayer | Method in Social Science, chs. 1–4 | EN | ~120 | Transparent | | 4 | |
| 11D.2 | Sayer | Why Things Matter to People, chs. 1–4 | EN | ~150 | Transparent | | 4 | |
| 11D.3 | Bhaskar | The Possibility of Naturalism, chs. 1–3 | EN | ~100 | Transparent | | 3 | "Denser than Sayer" per syllabus but in the framework class — Bhaskar reads at orientation-text pace once topic known; kept Transparent. Borderline → Analytic. |

### Module 12: Political Philosophy

| ID | Author | Title | Lang | Pages | Class | Flag | n_chapters | Notes |
|---|---|---|---|---|---|---|---|---|
| 12.1 | Freeman | Rawls, chs. 1–3 | EN | ~100 | Transparent | | 3 | |
| 12.2 | Rawls | A Theory of Justice, chs. 1–3 | EN | ~200 | Analytic | | 3 | [NE]. |
| 12.3 | Young | Justice and the Politics of Difference, chs. 1–3 | EN | ~100 | Analytic | | 3 | |
| 12.4 | Sen | Development as Freedom, chs. 1–4 | EN | ~120 | Transparent | | 4 | [RS]. |
| 12.5 | Anderson | What Is the Point of Equality? (article) | EN | ~30 | Analytic | | 1 | |
| 12.6 | Mills | The Racial Contract | EN | ~130 | Analytic | | 4 (est) | |
| 12.7 | Benhabib | Situating the Self, chs. 1–5 | EN | ~180 | Analytic | | 5 | |
| 12.8 | Pettit | Republicanism, chs. 1–3 | EN | ~120 | Analytic | | 3 | |
| 12.9 | Skinner | Liberty before Liberalism | EN | ~120 | Transparent | | 3 (est) | [NE]. Historical-philosophical lecture-book. |
| 12.10 | Graeber | Debt: The First 5,000 Years (selections) | EN | ~200 | Transparent | | 4 | Intro + chs. 5, 8, 11. |
| 12.11 | Scott | Seeing Like a State, Intro + chs. 1, 9–10 | EN | ~150 | Transparent | | 4 | |
| 12.12 | Gutiérrez | Teología de la liberación, Intro + ch. 11 | ES/EN | ~50 | Layered | | 2 | Theological-philosophical register; Layered. |
| 12.13 | Dussel | Filosofía de la liberación (selections) | ES/EN | ~80 | Layered | | 3 | Intro + chs. 2, 5. |

### Module 13: Marxist Theoretical Foundations

| ID | Author | Title | Lang | Pages | Class | Flag | n_chapters | Notes |
|---|---|---|---|---|---|---|---|---|
| 13.1 | Backhaus | Dialektik der Wertform, Intro + chs. 1–3 | DE | ~120 | Dense | | 4 | Neue Marx-Lektüre; resistant prose. |
| 13.2 | Reichelt | Social Reality as Appearance (article) | EN | ~25 | Layered | | 1 | |
| 13.3 | Gramsci | Quaderni del carcere (selections) | IT/EN | ~120 | Layered | | 3 | Three notebook-selections (Q11, Q6+Q25, Q22). Fragmentary but clearer than Adorno → Layered. |
| 13.4 | Thomas | The Gramscian Moment, chs. 1–4 | EN | ~150 | Layered | | 4 | |
| 13.5 | Althusser | Idéologie et appareils idéologiques d'État | FR/EN | ~40 | Layered | | 1 | |
| 13.6 | Sohn-Rethel | Geistige und körperliche Arbeit (Intellectual and Manual Labour) | DE | ~150 | Dense | | 4 (est) | **[Added 2026-06-29 — branch B.]** Real-abstraction; epistemologically dense. Read German (Brill 2021 ed.). |
| 13.7 | Arthur | The New Dialectic and Marx's Capital | EN | ~180 | Systematic | | 6 (est) | **[Added 2026-06-29 — branch B.]** Systematic dialectics; dense-but-structured. |
| 13.8 | Bonefeld | Critical Theory and the Critique of Political Economy | EN | ~200 | Layered | | 7 (est) | **[Added 2026-06-29 — branch B.]** Open-Marxism / Adornian register. |

### Module 14: Capitalism as Social Form

| ID | Author | Title | Lang | Pages | Class | Flag | n_chapters | Notes |
|---|---|---|---|---|---|---|---|---|
| 14.1 | Streeck | Gekaufte Zeit | DE | ~250 | Transparent | | 5 (est) | Streeck reads at sociology-of-political-economy pace; Transparent per framework. |
| 14.2 | Fraser | Cannibal Capitalism | EN | ~200 | Layered | | 5 (est) | Fraser monograph; Layered. |
| 14.3 | Bhattacharya | Mapping Social Reproduction Theory (Intro to ed. vol.) | EN | ~30 | Layered | | 1 | |
| 14.4 | Postone | Time, Labor, and Social Domination, chs. 1–5 | EN | ~200 | Systematic | | 5 | Most philosophically demanding text in module; Systematic. |
| 14.5 | Wright | Envisioning Real Utopias, chs. 1–4 | EN | ~150 | Layered | | 4 | |
| 14.6 | Brown | Undoing the Demos | EN | ~200 | Layered | | 6 (est) | |
| 14.7 | Honneth | Die Idee des Sozialismus | DE | ~180 | Systematic | | 5 (est) | Special rule #3 — monograph → Systematic. |
| 14.8 | Redecker | Selected articles + Revolution für das Leben | DE | ~120 | Layered | | 3 (est) | Articles + accessible companion. |
| 14.9 | Aglietta | Régulation et crises du capitalisme, Intro + ch. 1 | FR/EN | ~120 | Layered | | 2 | Régulation-school technical-economic register; borderline Layered/Analytic — went Layered. |
| 14.10 | Lordon | Capitalisme, désir et servitude, chs. 1–4 | FR/EN | ~100 | Layered | | 4 | |
| 14.11 | Mau | Mute Compulsion (Intro + Parts I–II) | EN | ~180 | Layered | | 5 (est) | **[Backfilled 2026-06-29 — present in syllabus/phase3 but absent here.]** Marxist; accessible to economist. |
| 14.12 | Castel | Les métamorphoses de la question sociale (Intro + Parts III–IV) | FR/DE | ~200 | Layered | | 4 (est) | **[Backfilled 2026-06-29.]** Sociology of work; long-historical. |
| 14.13 | Engster | Das Geld als Maß, Mittel und Methode | DE | ~200 | Systematic | | 5 (est) | **[Added 2026-06-29 — branch B.]** Value-form-as-measurement; technical, German. |
| 14.14 | Lapavitsas | Profiting Without Producing (Intro + chs. 1–4 + CB ch.) | EN | ~180 | Layered | | 6 (est) | **[Added 2026-06-29 — branch B.]** Marxist monetary theory; economist-accessible. |
| 14.15 | Jaeggi & Loick (eds.) | Nach Marx (selected contributions) | DE | ~150 | Layered | | 4 (est) | **[Added 2026-06-29 — branch B.]** Essay collection; the recognition↔CPE bridge. |
| 14.16 | Habermas + Offe | Legitimationsprobleme im Spätkapitalismus, Teil II + Offe selection | DE | ~70 (est) | Systematic | | 2 (est) | **[Added 2026-07-13 (coverage audit).]** Habermas → Systematic per framework; Offe selection rides in the same unit. Read before/with 14.1. |

### Module 15: Zeitdiagnose

| ID | Author | Title | Lang | Pages | Class | Flag | n_chapters | Notes |
|---|---|---|---|---|---|---|---|---|
| 15.1 | Schimank & Volkmann (eds.) | Soziologische Gegenwartsdiagnosen | DE | ~200 | Transparent | | 1 | Survey collection; reads at orientation pace. |
| 15.2 | Beck | Risikogesellschaft, Parts I–II | DE | ~200 | Layered | | 2 | |
| 15.3 | Boltanski & Chiapello | Le nouvel esprit du capitalisme, Part I + theoretical chs. | FR/DE/EN | ~250 | Layered | | 5 (est) | |
| 15.4 | Reckwitz | Die Gesellschaft der Singularitäten, Parts I–II | DE | ~200 | Layered | | 2 | |
| 15.5 | Rosa | Beschleunigung, Parts I–II | DE | ~250 | Layered | | 2 | |
| 15.6 | Polanyi | The Great Transformation, Parts I–II | EN | ~200 | Transparent | | 2 | |
| 15.7 | Illouz | Cold Intimacies | EN | ~120 | Layered | | 4 (est) | |

### Module 16: Social Phenomenology

| ID | Author | Title | Lang | Pages | Class | Flag | n_chapters | Notes |
|---|---|---|---|---|---|---|---|---|
| 16.1 | Schütz | Der sinnhafte Aufbau der sozialen Welt, chs. 1–3 | DE | ~150 | Systematic | | 3 | |
| 16.2 | Berger & Luckmann | The Social Construction of Reality | EN | ~200 | Transparent | | 3 (est) | Clear and structured. |
| 16.3 | Husserl | Die Krisis, §§28–55 | DE | ~100 | Dense | | 1 | [NE]. Husserl's prose is dense per framework. |

### Module 17: Social Ontology

| ID | Author | Title | Lang | Pages | Class | Flag | n_chapters | Notes |
|---|---|---|---|---|---|---|---|---|
| 17.1 | Epstein | The Ant Trap | EN | ~200 | Analytic | | 8 (est) | |
| 17.2 | List & Pettit | Group Agency, chs. 1–4 | EN | ~150 | Analytic | | 4 | |
| 17.3 | Searle | The Construction of Social Reality, chs. 1–4 | EN | ~100 | Analytic | | 4 | [NE]. |

### Module 18: Philosophical Anthropology

| ID | Author | Title | Lang | Pages | Class | Flag | n_chapters | Notes |
|---|---|---|---|---|---|---|---|---|
| 18.1 | Plessner / Fischer | Stufen des Organischen, Intro + chs. 7–8 (or Fischer substitute) | DE | ~150 | Layered | | 3 | [NE]. Plessner is dense but Fischer substitute is Transparent; assigned Layered as compromise. Borderline. |
| 18.2 | Gehlen | Der Mensch, chs. 1–5 | DE | ~180 | Layered | | 5 | [NE]. |
| 18.3 | Graeber & Wengrow | The Dawn of Everything (selections) | EN | ~250 | Transparent | | 7 | [NE]. Chs. 1–4, 8, 12. |

---

## Part V — Craft Block

(Re-readings; some entries cross-reference other modules. Listed here for completeness; downstream agent should not double-count hours.)

| ID | Author | Title | Lang | Pages | Class | Flag | n_chapters | Notes |
|---|---|---|---|---|---|---|---|---|
| W1.1 | Stahl | Immanente Kritik, chs. 1–4 (re-read) | DE | ~200 | Layered | | 4 | Cross-ref to 8.8. |
| W1.2 | Celikates | From Critical Social Theory to a Social Theory of Critique (article) | EN | ~20 | Analytic | | 1 | |
| W1.3 | Jaeggi | Kritik von Lebensformen, chs. 1–3 (re-read) | DE | ~120 | Layered | | 3 | Cross-ref to 8.2. |
| W1.4 | Honneth | Pathologien des Sozialen (re-read) | DE | ~25 | Layered | | 1 | Cross-ref to 0.2. |
| W2.1 | Honneth | Recht der Freiheit, "Der Markt" chapter (re-read) | DE | ~60 | Systematic | | 1 | Cross-ref to 7.5. |
| W2.2 | Rosa | Beschleunigung, Part III | DE | ~50 | Layered | | 1 | Additional section beyond 15.5. |
| W2.3 | Jaeggi & Fraser | Capitalism: A Conversation, chs. 1–3 (re-read) | EN | ~120 | Layered | | 3 | Cross-ref to 8.5. |

---

## Appendix A — Social Epistemology (deeper)

| ID | Author | Title | Lang | Pages | Class | Flag | n_chapters | Notes |
|---|---|---|---|---|---|---|---|---|
| A.0.1 | Fricker et al. (eds.) | Routledge Handbook of Social Epistemology (selections) | EN | ~500 | Transparent | | 8 | Handbook orientation. |
| A.1.1 | Goldman | Knowledge in a Social World, chs. 1–5 | EN | ~200 | Analytic | | 5 | |
| A.1.2 | Coady | Testimony: A Philosophical Study, chs. 1–5 | EN | ~150 | Analytic | | 5 | |
| A.1.3 | Lackey (ed.) | Essays in Collective Epistemology (Intro + selections) | EN | ~200 | Analytic | | 5 (est) | |
| A.1.4 | Goldman & Blanchard | Social Epistemology (SEP) | EN | ~150 | Transparent | | 1 | SEP entry, treat as one unit. |
| A.2.1 | Mannheim | Ideologie und Utopie (complete) | DE | ~150 | Dense | | 4 (est) | Full text beyond Module 9. |
| A.2.2 | Harding | Whose Science? Whose Knowledge?, chs. 1–5 | EN | ~30 | Transparent | | 5 | Syllabus page count is anomalously low (~30 vs. chs. 1–5); kept (?) flag warranted but listed verbatim. |
| A.2.3 | Medina | The Epistemology of Resistance, chs. 1–4 | EN | ~200 | Analytic | | 4 | |
| A.2.4 | Habermas | Erkenntnis und Interesse (remaining chapters) | DE | ~200 | Systematic | | 5 (est) | |
| A.3.1 | Haslanger | Resisting Reality (selected essays) | EN | ~200 | Analytic | | 6 (est) | |
| A.3.2 | Shelby | Ideology, Racism, and Critical Social Theory | EN | ~180 | Analytic | | 1 | Page count in syllabus (~180) conflicts with Module 9.5 (~25); listed verbatim per syllabus. Likely error in syllabus; treat as ~25. |
| A.3.3 | Jaeggi | Rethinking Ideology (essay) | EN | ~150 | Layered | | 1 | Page count in syllabus (~150) appears inflated for an essay (Jaeggi's "Rethinking Ideology" is ~25–30pp); listed verbatim. |

---

## Appendix B — Philosophy of Social Science (deeper)

| ID | Author | Title | Lang | Pages | Class | Flag | n_chapters | Notes |
|---|---|---|---|---|---|---|---|---|
| B.0.1 | McIntyre & Rosenberg (eds.) | Routledge Companion to Philosophy of Social Science (selections) | EN | ~500 | Transparent | | 8 | Handbook. |
| B.0.2 | Little | Philosophy of Social Science (SEP) | EN | ~50 | Transparent | | 1 | |
| B.0.3 | Rosenberg | Philosophy of Social Science (5th ed.) | EN | ~280 | Transparent | | 10 (est) | Textbook. |
| B.1.1 | Hempel | Function of General Laws + Aspects of Scientific Explanation chs. 10–12 | EN | ~80 | Analytic | | 4 | Hempel essay + 3 chapters. |
| B.1.2 | Elster | Nuts and Bolts for the Social Sciences | EN | ~130 | Analytic | | 5 (est) | |
| B.1.3 | Hedström & Swedberg (eds.) | Social Mechanisms (Intro + selections) | EN | ~150 | Analytic | | 5 (est) | |
| B.1.4 | Little | Varieties of Social Explanation | EN | ~200 | Transparent | | 6 (est) | |
| B.1.5 | von Wright | Explanation and Understanding | EN | ~180 | Analytic | | 4 (est) | |
| B.2.1 | Woodward | Making Things Happen, chs. 4–7 | EN | ~150 | Analytic | | 4 | |
| B.2.2 | Hausman | The Inexact and Separate Science of Economics | EN | ~250 | Analytic | | 10 (est) | |
| B.2.3 | Reiss | Causation, Evidence, and Inference, chs. 1–6 | EN | ~200 | Analytic | | 6 | |
| B.2.4 | Cartwright | The Dappled World, chs. 1–4 | EN | ~100 | Analytic | | 4 | [RS]. |
| B.3.1 | Putnam | The Collapse of the Fact/Value Dichotomy | EN | ~100 | Analytic | | 4 (est) | Essay collection. |
| B.3.2 | Douglas | Science, Policy, and the Value-Free Ideal, chs. 1–5 | EN | ~200 | Analytic | | 5 | |
| B.3.3 | Kitcher | Science, Truth, and Democracy, chs. 6–10 | EN | ~150 | Analytic | | 5 | [RS]. |
| B.4.1 | Morgan | The World in the Model (selected chs.) | EN | ~200 | Analytic | | 5 (est) | |
| B.4.2 | Mäki (ed.) | The Methodology of Positive Economics (Intro + essays) | EN | ~200 | Analytic | | 5 (est) | |
| B.4.3 | Sugden | Credible Worlds, Capacities and Mechanisms (article) | EN | ~100 | Analytic | | 1 | Page count (~100) elevated for an article — likely error; treat as ~30. |

---

## Appendix C — Marxist Deepening [MX]

(Items C.1–C.5 promoted to Module 13; C.0 orientation + C.6+ deepening only.)

| ID | Author | Title | Lang | Pages | Class | Flag | n_chapters | Notes |
|---|---|---|---|---|---|---|---|---|
| C.0.1 | Anderson | Considerations on Western Marxism | EN | ~120 | Layered | | 1 | Short polemical book; treat as one unit. |
| C.0.2 | Henning | Philosophie nach Marx (selections) | DE/EN | ~600 | Layered | | 5 (est) | Selections. |
| C.0.3 | Haug et al. (eds.) | HKWM (Historisch-kritisches Wörterbuch des Marxismus) | DE | ref | Transparent | | 1 | Reference only; not read-through. |
| C.0.4 | Wolff & Leopold | Karl Marx (SEP) | EN | ~60 | Transparent | | 1 | SEP entry. |
| C.0.5 | — | Critical Theory (Frankfurt School) (SEP) | EN | ~60 | Transparent | | 1 | SEP entry. |
| C.6 | Brenner | Origins of Capitalist Development (NLR article) | EN | ~60 | Analytic | | 1 | Syllabus mentions "~40 pages" inline; ~60 in column. Listed as ~60. |
| C.7 | Harvey | The Right to the City (NLR article) | EN | ~20 | Analytic | | 1 | Syllabus column says ~200 but inline note says ~20; the ~20 is correct (NLR article). |
| C.8 | Wright | Understanding Class (NLR article) | EN | ~30 | Analytic | | 1 | Syllabus column says ~150 but inline says ~30; ~30 correct. |
| C.9 | Heller | Theorie der Bedürfnisse bei Marx | DE/EN | ~180 | Layered | | 5 (est) | |
| C.10 | Heller | Das Alltagsleben, chs. 1–5 | DE/EN | ~200 | Layered | | 5 | |
| C.11 | Márkus | Language and Production, chs. 1–4 | EN | ~200 | Layered | | 4 | Philosophically rigorous but accessible — Layered. |
| C.12 | Kosík | Dialektik des Konkreten | DE | ~150 | Layered | | 4 (est) | |
| C.13 | Kołakowski | Main Currents of Marxism, vol. 3 (selected chs.) | EN/DE | ~200 | Transparent | | 4 (est) | Kołakowski writes lucidly; orientation-tier reading. |
| C.14 | Tronti | Operai e capitale (selections) | IT/EN | ~120 | Layered | | 3 | Intro + 2 chapters. |
| C.15 | Hardt & Negri | Empire, Intro + Part 1 chs. 1.1–1.3 | EN | ~150 | Layered | | 4 | |
| C.16 | Federici | Caliban and the Witch, Intro + chs. 2, 3, 5 | EN | ~150 | Layered | | 4 | |
| C.17 | Federici | Revolution at Point Zero (selected essays) | EN | ~80 | Layered | | 3 | 3 essays per syllabus. |
| C.17a | Dalla Costa & James | The Power of Women and the Subversion of the Community | EN | ~40 | Layered | | 1 | |
| C.18 | Cohen | Karl Marx's Theory of History, chs. 1–4 | EN | ~150 | Analytic | | 4 | [NE]. Analytical Marxism. |
| C.19 | Roemer | A General Theory of Exploitation and Class, Intro + chs. 1–3 | EN | ~150 | Analytic | | 4 | [NE]. |
| C.20 | Wright | Class Counts, Intro + chs. 1–2 | EN | ~120 | Analytic | | 3 | [NE]. |
| C.21 | Saito | Marx in the Anthropocene, Intro + chs. 1–3 | EN | ~150 | Layered | | 4 | [NE]. |
| C.22 | Moore | Capitalism in the Web of Life, Intro + chs. 1, 3, 7 | EN | ~180 | Layered | | 4 | [NE]. |
| C.23 | Malm | Fossil Capital, Intro + chs. 1, 11–12 | EN | ~180 | Layered | | 4 | [NE]. |
| C.24 | Boyer | The Regulation School (Intro + chs. 1–4) | FR/EN | ~150 | Layered | | 4 | [NE]. |
| C.25 | Lipietz | Mirages and Miracles, Intro + ch. 1 | FR/EN | ~100 | Layered | | 2 | [NE]. |

---

## Appendix D — Capitalism Critique (supplementary)

| ID | Author | Title | Lang | Pages | Class | Flag | n_chapters | Notes |
|---|---|---|---|---|---|---|---|---|
| D.0.1 | Kocka | Geschichte des Kapitalismus | DE | ~144 | Transparent | | 6 (est) | C.H. Beck Wissen short-form. |
| D.0.2 | Ingham | Capitalism (Polity Key Concepts) | EN | ~280 | Transparent | | 7 (est) | |
| D.0.3 | Henning | Philosophie nach Marx (selections) | DE/EN | ~600 | Layered | | 5 (est) | Cross-listed with C.0.2 — *primary entry in C.0.2; do not double-count.* |
| D.1.1 | Hall & Soskice | Varieties of Capitalism, Introduction | EN | ~70 | Transparent | | 1 | |
| D.1.2 | Beckert | Imaginierte Zukunft | DE | ~300 | Layered | | 8 (est) | |
| D.2.1 | Hickel | Less Is More, chs. 1–5 | EN | ~150 | Transparent | | 5 | [RS]. |
| D.2.2 | Karatani | The Structure of World History, Intro + Part I | EN | ~150 | Layered | | 4 (est) | [RS]. |
| D.2.3 | Wallerstein | The Modern World-System vol. 1, Intro + chs. 1–2 | EN | ~120 | Transparent | | 3 | |
| D.2.4 | Arrighi | The Long Twentieth Century, Intro + ch. 1 | EN | ~100 | Transparent | | 2 | |
| D.3.1 | Staab | Digitaler Kapitalismus | DE | ~280 | Layered | | 6 (est) | [RS]. |

---

## Appendix E — Zeitdiagnose (deeper)

| ID | Author | Title | Lang | Pages | Class | Flag | n_chapters | Notes |
|---|---|---|---|---|---|---|---|---|
| E.0.1 | Schimank & Volkmann (eds.) | Soziologische Gegenwartsdiagnosen I | DE | ~250 | Transparent | | 1 | Survey volume; cross-listed with 15.1. |
| E.0.2 | Volkmann & Schimank (eds.) | Soziologische Gegenwartsdiagnosen II | DE | ~250 | Transparent | | 1 | Companion survey. |
| E.1.1 | Joas & Knöbl | Sozialtheorie: Zwanzig einführende Vorlesungen (selected) | DE | ~200 | Transparent | | 5 (est) | |
| E.1.2 | Durkheim | De la division du travail social, Preface 2nd ed. + Book III | FR/DE/EN | ~80 | Layered | | 2 | |
| E.1.3 | Simmel | Philosophie des Geldes, final chapter | DE | ~60 | Layered | | 1 | |
| E.1.4 | Bourdieu | La distinction, Intro + Part I | FR/DE/EN | ~150 | Systematic | | 2 | Cross-ref to 11C.2; primary there. |
| E.1.5 | Luhmann / Horster | Soziale Systeme chs. 3–4 (or Horster substitute) | DE | ~150 | Systematic | | 2 | Cross-ref to 11B; extension beyond Module 11B. |
| E.2.1 | Bell | The Coming of Post-Industrial Society, chs. 1–3 | EN | ~120 | Transparent | | 3 | |
| E.2.2 | Foucault | Surveiller et punir, Parts I–II | FR/DE/EN | ~150 | Layered | | 2 | Cross-ref to 11A.1; extended scope. |
| E.2.3 | Bauman | Liquid Modernity, chs. 1–3 | EN | ~200 | Transparent | | 3 | |
| E.2.4 | Sennett | The Corrosion of Character | EN | ~200 | Transparent | | 8 (est) | |
| E.2.5 | Han | Müdigkeitsgesellschaft | DE | ~120 | Transparent | | 5 (est) | Short, accessible. |
| E.2.6 | Nassehi | Muster: Theorie der digitalen Gesellschaft, Parts I–II | DE | ~150 | Layered | | 2 | |
| E.2.7 | Rosa | Resonanz, Parts I + IV | DE | ~200 | Layered | | 2 | Cross-ref to 8.9 (overlapping scope). |
| E.3.1 | Schulze | Die Erlebnisgesellschaft, Intro + chs. 1–3 | DE | ~150 | Layered | | 4 | |
| E.3.2 | Boltanski | De la critique, chs. 1–4 | FR/EN | ~150 | Layered | | 4 | Cross-ref to 9.7; primary there. |

---

## Appendix F — Social Ontology (deeper)

| ID | Author | Title | Lang | Pages | Class | Flag | n_chapters | Notes |
|---|---|---|---|---|---|---|---|---|
| F.0.1 | Epstein | Social Ontology (SEP) | EN | ~60 | Transparent | | 1 | |
| F.0.2 | Collins, Epstein, Haslanger & Schmid (eds.) | Oxford Handbook of Social Ontology (selections) | EN | ~700 | Transparent | | 8 | |
| F.1.1 | Gilbert | On Social Facts, chs. 1–4 | EN | ~200 | Analytic | | 4 | [NE]. |
| F.1.2 | Tuomela | Social Ontology, chs. 1–5 | EN | ~200 | Analytic | | 5 | [NE]. |
| F.1.3 | Bratman | Shared Agency | EN | ~100 | Analytic | | 5 (est) | [NE]. |
| F.1.4 | Searle | Making the Social World, chs. 1–5 | EN | ~200 | Analytic | | 5 | [NE]. |
| F.2.1 | Hacking | The Social Construction of What? | EN | ~250 | Analytic | | 6 (est) | |
| F.2.2 | Khalidi | Natural Categories and Human Kinds, chs. 5–8 | EN | ~200 | Analytic | | 4 | |
| F.2.3 | Epstein | The Ant Trap (remaining chapters) | EN | ~150 | Analytic | | 5 (est) | Cross-ref to 17.1. |
| F.2.4 | Hindriks | How Autonomous Are Collective Agents? (article) | EN | ~20 | Analytic | | 1 | |
| F.3.1 | Bicchieri | The Grammar of Society | EN | ~200 | Analytic | | 6 (est) | |
| F.3.2 | Hodgson | What Are Institutions? (article) | EN | ~150 | Analytic | | 1 | Page count ~150 elevated for an article — likely error; treat as ~30. |
| F.3.3 | Guala | Understanding Institutions | EN | ~200 | Analytic | | 8 (est) | |

---

## Appendix G — Social Phenomenology (deeper, [NE])

| ID | Author | Title | Lang | Pages | Class | Flag | n_chapters | Notes |
|---|---|---|---|---|---|---|---|---|
| G.0.1 | Zahavi | Phenomenology: The Basics | EN | ~190 | Transparent | | 6 (est) | |
| G.0.2 | Luft & Overgaard (eds.) | Routledge Companion to Phenomenology (selections) | EN | ~600 | Transparent | | 8 | |
| G.0.3 | Smith | Phenomenology (SEP) | EN | ~50 | Transparent | | 1 | |
| G.0.4 | — | Alfred Schutz (SEP) | EN | ~50 | Transparent | | 1 | |
| G.1 | Schütz | Der sinnhafte Aufbau (remaining chs.) | DE | ~150 | Systematic | | 4 (est) | [NE]. Cross-ref to 16.1. |
| G.2 | Schütz & Luckmann | Strukturen der Lebenswelt vol. 1 | DE | ~200 | Systematic | | 5 (est) | [NE]. |
| G.3 | Husserl | Die Krisis (complete) | DE | ~300 | Dense | | 5 (est) | [NE]. |
| G.4 | Merleau-Ponty | Phénoménologie de la perception, Intro + Part I | FR/DE/EN | ~250 | Dense | | 4 (est) | [NE]. Borderline Dense/Systematic; classed Dense per Merleau-Ponty's prose. |
| G.5 | Staudigl & Berguno (eds.) | Schutzian Phenomenology and Hermeneutic Traditions (selections) | EN | ~150 | Layered | | 5 (est) | [NE]. |
| G.6 | Guenther | Solitary Confinement: Social Death and Its Afterlives | EN | ~200 | Layered | | 6 (est) | [NE]. |
| G.7 | Zahavi | Self and Other, chs. 1–5 | EN | ~200 | Layered | | 5 | [NE]. |

---

## Appendix H — Socialisation, Child Development, Bildung

| ID | Author | Title | Lang | Pages | Class | Flag | n_chapters | Notes |
|---|---|---|---|---|---|---|---|---|
| H.0.1 | Hurrelmann & Bauer | Einführung in die Sozialisationstheorie | DE | ~320 | Transparent | | 8 (est) | Textbook. |
| H.0.2 | Koller | Bildung anders denken | DE | ~190 | Transparent | | 6 (est) | Textbook. |
| H.0.3 | Tippelt & Schmidt-Hertha (eds.) | Handbuch Bildungsforschung | DE | ref | Transparent | | 1 | Reference only. |
| H.0.4 | Hurrelmann, Bauer, Grundmann & Walper (eds.) | Handbuch Sozialisationsforschung | DE | ref | Transparent | | 1 | Reference only. |
| H.1.1 | Whitebook | The Marriage of Marx and Freud (essay) | EN | ~30 | Layered | | 1 | |
| H.1.2 | Benjamin | The Bonds of Love, chs. 1–3 | EN | ~120 | Layered | | 3 | Cross-ref to 7.11; primary there. |
| H.1.3 | Honneth | Objektbeziehungstheorie und postmoderne Identität (essay) | DE | ~25 | Layered | | 1 | |
| H.1.4 | Whitebook | Perversion and Utopia, chs. 1–3 | EN | ~120 | Layered | | 3 | [NE]. |
| H.1.5 | Marcuse | Triebstruktur und Gesellschaft (Eros and Civilization) | EN | ~180 | Layered | | 8 (est) | **[Added 2026-06-27.]** Freudo-Marxist counter to Freud 4.12; cf. 4.8 ODM (also Layered). ~180pp core selection. |
| H.1.6 | Fromm | Die Furcht vor der Freiheit (Escape from Freedom) | EN | ~270 | Layered | | 7 | **[Added 2026-06-27.]** Orig. English (1941); accessible theoretical prose; 7 chapters + appendix. |
| H.1.7 | Mitscherlich | Auf dem Weg zur vaterlosen Gesellschaft | DE | ~200 | Layered | | 6 (est) | **[Added 2026-06-27.]** [RS]. Essayistic-clinical German prose; ~200pp selection. |
| H.1.8 | Layton | Toward a Social Psychoanalysis | EN | ~200 | Layered | | 6 (est) | **[Added 2026-06-29 — branch E.]** Normative unconscious processes. |
| H.1.9 | Ikäheimo | Recognition and the Human Life-Form | EN | ~200 | Analytic | | 6 (est) | **[Added 2026-06-29 — branch E.]** Analytic recognition theory; cf. 7.15. |
| H.1.10 | Allen | Critique on the Couch | EN | ~250 (est) | Layered | | 7 (est) | **[Added 2026-07-13 (coverage audit).]** Allen → Layered per framework. Verify subtitle (Columbia UP 2021). Read after H.1.8. |
| H.2.1 | Gerhardt | Why Love Matters | EN | ~280 | Transparent | | 9 (est) | Popular-science synthesis. |
| H.2.2 | Allen | The Politics of Our Selves, chs. 1–4 | EN | ~150 | Layered | | 4 | |
| H.3.1 | Bhattacharya | Mapping Social Reproduction Theory | EN | ~30 | Layered | | 1 | Cross-ref to 14.3; primary there. |
| H.3.2 | Arruzza, Bhattacharya & Fraser | Feminism for the 99%: A Manifesto | EN | ~80 | Transparent | | 1 | Short manifesto. |
| H.3.3 | Federici | Revolution at Point Zero (essays) | EN | ~80 | Layered | | 3 | Cross-ref to C.17 (primary). |
| H.3.4 | Federici | Caliban and the Witch | EN | ~150 | Layered | | 4 | Cross-ref to C.16 (primary). |
| H.3.5 | Dalla Costa & James | The Power of Women | EN | ~40 | Layered | | 1 | Cross-ref to C.17a (primary). |
| H.3.6 | Winker | Care Revolution | DE | ~150 | Layered | | 5 (est) | **[Added 2026-06-29 — branch E.]** German care-revolution; SRT counterpart. |
| H.4.1 | Plessner / Fischer | Stufen des Organischen (selection) | DE | ~150 | Layered | | 3 | Cross-ref to 18.1. |
| H.4.2 | Gehlen | Der Mensch, chs. 1–5 | DE | ~180 | Layered | | 5 | Cross-ref to 18.2. |
| H.5.1 | Siegler, Saffran & Gershoff | How Children Develop (selected chs.) | EN | ~250 | Transparent | | 5 | Chs. 1, 5, 9, 10, 11. |
| H.5.2 | Bowlby | Attachment and Loss vol. 1, chs. 1–4 + 11–13 | EN | ~200 | Transparent | | 7 | Bowlby writes clearly. |
| H.5.3 | Cassidy & Shaver (eds.) | Handbook of Attachment, chs. 1, 19, 30 | EN | ~120 | Transparent | | 3 | |
| H.5.4 | Vygotsky | Mind in Society | EN | ~120 | Transparent | | 6 (est) | Vygotsky's prose is clear. |
| H.5.5 | Shonkoff & Phillips (eds.) | From Neurons to Neighborhoods (Exec Summary + chs. 1–3 + 8–10) | EN | ~200 | Transparent | | 7 | |
| H.5.6 | Felitti et al. | Relationship of Childhood Abuse and Household Dysfunction (article) | EN | ~15 | Analytic | | 1 | Empirical-quantitative article. |
| H.6.1 | Adorno | Theorie der Halbbildung (essay) | DE | ~30 | Dense | | 1 | Adorno essay → Dense per framework. |
| H.6.2 | Heydorn | Über den Widerspruch von Bildung und Herrschaft (Intro + Parts I + III) | DE | ~120 | Layered | | 3 | |
| H.6.3 | Humboldt | Theorie der Bildung des Menschen + Ideen (selections) | DE | ~30 | Dense | | 2 | 1793 fragment + 1792 essay selections; classical-philosophical prose. |
| H.6.4 | Mollenhauer | Vergessene Zusammenhänge | DE | ~200 | Layered | | 6 (est) | |
| H.6.5 | English | Discontinuity in Learning, chs. 1–5 | EN | ~200 | Analytic | | 5 | |
| H.6.6 | Krappmann | Soziologische Dimensionen der Identität | DE | ~200 | Layered | | 5 (est) | |
| H.6.7 | Hurrelmann & Bauer | Einführung in die Sozialisationstheorie (12th ed.) | DE | ~300 | Transparent | | 8 (est) | Cross-ref to H.0.1; same text. *Do not double-count.* |
| H.6.8 | Stojanov | Bildungsgerechtigkeit, chs. 1–4 | DE | ~120 | Analytic | | 4 | Analytic-philosophical-pedagogical register. |
| H.6.9 | Drerup & Schweiger (eds.) | Philosophy and Child Poverty (selected essays) | EN | ~80 | Analytic | | 3 (est) | |
| H.6.10 | Klafki | Neue Studien zur Bildungstheorie und Didaktik (selections) | DE | ~100 (est) | Layered | | 3 (est) | **[Added 2026-07-13 (coverage audit).]** German Pädagogik register, cf. Heydorn H.6.2 / Mollenhauer H.6.4 → Layered. Verify edition (1985, rev. 1991). Belongs to sub-section H.6a. |

---

## Appendix I — Building Toward Hegel (scheduled items only)

**[Section backfilled 2026-07-13 (propagation pass).]** Syllabus Appendix I (added 2026-05-29) is the full deep-Hegel build-up programme (~725–940h) and is mostly [NE]/deferred with no scheduled slots; rows below cover only the items the schedule actually executes — the two Kant items of the Module 7 Kant→Khurana pre-block (2026-07-12; see 1.6F above). Remaining Appendix I items (I.1.1–I.1.4, I.1.6, I.1.8–I.1.10, the I.4.x deep-Hegel tracks, I.0a) get rows if and when they are scheduled — a known, flagged gap against this file's "every text" claim, accepted because unscheduled appendix material generates no hour budget.

| ID | Author | Title | Lang | Pages | Class | Flag | n_chapters | Notes |
|---|---|---|---|---|---|---|---|---|
| I.1.5 | Kant | Grundlegung zur Metaphysik der Sitten (complete: Vorrede + Abschnitte I–III) | DE | ~80 | Systematic | | 4 | **[Backfilled 2026-07-13 (propagation pass).]** Scheduled via the Module 7 pre-block (M20–21, opt-in; Layer-2 *retained* — also underwrites Forst 7.7). Classical German primary but tightly structured and largely self-standing; borderline Dense — see borderline note. Syllabus estimate 8–10h ≈ 8–10 pp/h. |
| I.1.7 | Kant | Kritik der Urteilskraft — Kritik der teleologischen Urteilskraft, §§64–66 | DE | ~20 | Dense | | 1 | **[Backfilled 2026-07-13 (propagation pass).]** Scheduled via the Module 7 pre-block (M20–21, opt-in; Layer-2 first cut); direct prerequisite for Khurana 1.6F's life–freedom analogy. Late-Kant teleology → Dense (syllabus 4–6h ≈ 3–5 pp/h). |

---

## Notes on cross-listings and special cases

**Cross-listed (counted once at primary):**
- 7.11 Benjamin = H.1.2
- 8.8 Stahl = W1.1
- 8.2 Jaeggi = W1.3
- 0.2 Honneth = W1.4
- 7.5 Honneth = W2.1 (Markt chapter only)
- 8.5 Jaeggi & Fraser = W2.3
- 11C.2 Bourdieu = E.1.4
- 14.3 Bhattacharya = H.3.1
- C.16 Federici = H.3.4
- C.17 Federici = H.3.3
- C.17a Dalla Costa & James = H.3.5
- 18.1 Plessner = H.4.1
- 18.2 Gehlen = H.4.2
- 17.1 Epstein = F.2.3 (remaining chapters)
- 9.5 Shelby = A.3.2
- H.0.1 / H.6.7 Hurrelmann & Bauer (same text)
- C.0.2 / D.0.3 Henning (same text)
- 15.1 = E.0.1 (Schimank/Volkmann survey)
- 9.7 / E.3.2 Boltanski *De la critique*
- 8.9 / E.2.7 Rosa *Resonanz*
- 16.1 / G.1 Schütz *Sinnhafte Aufbau* (different scopes)
- 11A.1 / E.2.2 Foucault *Surveiller et punir* (different scopes)

**Borderline classifications worth flagging (Class column = chosen value, not `?`):**
- 11D.3 Bhaskar — Transparent (orientation-tier) vs. Analytic (philosophical density). Went Transparent because all of 11D is [O].
- 14.9 Aglietta — Analytic (technical Régulation prose) vs. Layered (sociology-of-economic-form). Went Layered.
- 8A.3 Spivak — Dense (deliberately resistant rhetorical theory) vs. Layered. Went Layered for module consistency.
- 4.3 Pollock — Dense (Frankfurt-internal critical theory) vs. Layered. Went Layered; clearer prose than DdA.
- 4.8 Marcuse — Layered vs. Transparent. Went Layered; thesis-driven but conceptually layered.
- 18.1 Plessner / Fischer — depends on which (substitute) is read; Layered as compromise.
- 7.16 Gregoratto — Layered (composite of 2–3 articles); could vary.
- G.4 Merleau-Ponty — Dense vs. Systematic. Went Dense.
- 4.12 Freud *Unbehagen* — Layered vs. Transparent. Went Layered; lucid prose but a conceptually demanding primary theory, not an intro/secondary text.
- 4.13 Nietzsche *Genealogie* I–II — Layered vs. Dense. Went Layered (German-fluent reader; vivid continuous prose, not Hegel-slow), but read slowly for the argument despite the surface pace.
- I.1.5 Kant *Grundlegung* — Systematic vs. Dense. Went Systematic **[Backfilled 2026-07-13 (propagation pass)]**: scholastic but tightly structured treatise prose, faster than Hegel/KrV pace; the syllabus/plan estimate (~8–10h for ~80pp) sits at the Systematic/Layered boundary, not at Dense. The KU teleology sections (I.1.7) stay Dense.

**Page-count anomalies in syllabus (listed verbatim per syllabus, but likely errors — flagged for downstream sanity-check):**
- A.2.2 Harding chs. 1–5 listed as ~30 (syllabus column) — likely should be ~150–200. Listed verbatim.
- A.3.2 Shelby listed as ~180 in App. A — Module 9.5 lists same text as ~25; likely error in App. A. Listed verbatim.
- A.3.3 Jaeggi "Rethinking Ideology" listed as ~150 — likely should be ~25–30 (essay). Listed verbatim.
- C.7 Harvey "Right to the City" — column says ~200; inline says ~20; the ~20 is correct. Used ~20.
- C.8 Wright "Understanding Class" — column says ~150; inline says ~30; the ~30 is correct. Used ~30.
- F.3.2 Hodgson "What Are Institutions?" listed as ~150 — likely should be ~30 (article). Listed verbatim.
- B.4.3 Sugden listed as ~100 — likely should be ~30 (article). Listed verbatim.

**No `Class: ?` entries needed.** Every text was assignable to a class with reasonable confidence given the framework's deliberately broad bands (Dense / Systematic / Layered / Analytic / Transparent map well onto the texts in this syllabus; the borderlines above are noted in-row).
