# Renumbering Bridge: Syllabus v5 → v6

**Date:** 2026-05-20 (updated)
**Purpose:** Complete mapping of all identifier changes between syllabus v5 and v6. Designed to be applied by an automated agent to dependent documents (execution_plan, programme_parameters, y3_critical_path, audit documents, etc.).

---

## 0. How to Use This Bridge

**For an agent applying these changes to a dependent document:**

1. Read the document to be updated.
2. Apply substitutions in the order specified in §6 (Substitution Ordering) to avoid double-replacement.
3. Each substitution is a find → replace pair. Apply globally unless a scope restriction is noted.
4. After all substitutions, verify by searching for old identifiers listed in §7 (Verification Checklist).
5. Flag ambiguous references for human review.

**Key constraint:** Many substitutions are order-dependent. "Module 12A" must be replaced before "Module 12" (otherwise "Module 12A" becomes "Module 10A"). The ordering in §6 resolves all such conflicts.

---

## 1. Module Renumbering

### Parts I–II (unchanged)
Phase 0, Modules 1–5 (incl. 3A, 4A), Modules 6–8A: **no changes**.

### Letter-suffixed items now continuously numbered
| v5 | v6 | Module |
|----|----| ------|
| 4.2a (Pollock) | **4.3** | Module 4 (renumber 4.3→4.4, 4.4→4.5, …, 4.9→4.10) |
| 7.8a (Forst *Normativität*) | **7.9** | Module 7 (renumber 7.9→7.10, …, 7.17→7.18, 7.18→7.19) |
| 7.8b (Forst *Noumenal Republic*) | **7.10** | Module 7 (same cascade) |
| 14.2a (Bhattacharya) | **14.3** | Module 14 (renumber 14.3→14.4, …) |
| 14.6a (von Redecker) | **14.8** | Module 14 (renumber 14.7→14.9, 14.8→14.10) |

### Part III (restructured)

| v5 | v6 | Content | Change |
|----|----|---------|--------|
| Module 9 | **Module 9** | Social Epistemology | Unchanged |
| Module 12 | **Module 10** | Philosophy of Social Science | Renumbered |
| *(new header)* | **Modules 11A–11D** | Rival Paradigms | New category header |
| Module 12A | **Module 11A** | Foucault | Renumbered |
| Module 12B | **Module 11B** | Luhmann | Renumbered |
| Module 12C | **Module 11C** | Bourdieu | Renumbered |
| Module 12D | **Module 11D** | Critical Realism | Renumbered |
| Module 13 | **Module 12** | Political Philosophy | Renumbered |
| Module 13.B | **Module 12.B** | Alternative Diagnoses of Unfreedom | Renumbered |
| *(new)* | **Module 13** | Marxist Theoretical Foundations | New module (from App F core) |
| *(new)* | **Module 14** | Capitalism as Social Form | New module (from Part VI + Régulation) |
| Module 15 | **Module 15** | Soziologische Zeitdiagnose | Unchanged |
| Module 10 | **Module 16** | Social Phenomenology | Renumbered |
| Module 11 | **Module 17** | Social Ontology | Renumbered |
| Module 14 | **Module 18** | Philosophical Anthropology (dissolved) | Renumbered; Graeber 18.3 added |

### Part V (Craft Block) — tag change
| v5 | v6 | Content |
|----|----| ------|
| Module C1, items C1.x | **Module W1**, items **W1.x** | What Is Immanent Critique |
| Module C2, items C2.x | **Module W2**, items **W2.x** | Exemplary Diagnostics |
| Module C3, items C3.x | **Module W3**, items **W3.x** | Practical Writing Exercises |

### Part VI (dissolved)
| v5 | v6 destination |
|----|---------------|
| Part VI (section) | Dissolved. Essentials → Module 14; remainder → Appendix D |
| K.1 Streeck | Module 14 item 14.1 |
| K.2 Fraser | Module 14 item 14.2 |
| K.2a Bhattacharya | Module 14 item 14.3 |
| K.3 Postone | Module 14 item 14.4 |
| K.4 Wright | Module 14 item 14.5 |
| K.5 Brown | Module 14 item 14.6 |
| K.6 Honneth Sozialismus | Module 14 item 14.7 |
| K.6a von Redecker | Module 14 item 14.8 |
| K.6b Aglietta | Module 14 item 14.9 |
| K.6c Lordon | Module 14 item 14.10 |
| K.7 Hall & Soskice | Appendix D item D.1.1 |
| K.8 Beckert | Appendix D item D.1.2 |
| K.9 Hickel | Appendix D item D.2.1 |
| K.10 Karatani | Appendix D item D.2.2 |
| K.11 Staab | Appendix D item D.3.1 |
| K.12 Wallerstein | Appendix D item D.2.3 |
| K.13 Arrighi | Appendix D item D.2.4 |

### Motivational Checkpoint
Removed entirely.

---

## 2. Item-Level Renumbering Within Renamed Modules

| v5 range | v6 range | Module |
|----------|----------|--------|
| 12.1–12.5 | 10.1–10.5 | Philosophy of Social Science |
| 12A.1–12A.4 | 11A.1–11A.4 | Foucault |
| 12B.1–12B.3 | 11B.1–11B.3 | Luhmann |
| 12C.1–12C.4 | 11C.1–11C.4 | Bourdieu |
| 12D.1–12D.3 | 11D.1–11D.3 | Critical Realism |
| 13.1–13.13 | 12.1–12.13 | Political Philosophy |
| 13.B | 12.B | Alternative Diagnoses |
| 10.1–10.3 | 16.1–16.3 | Social Phenomenology |
| 11.1–11.3 | 17.1–17.3 | Social Ontology |
| 14.1–14.2 | 18.1–18.2 | Philosophical Anthropology |

### New Module 13 items (from Appendix F)
| v5 source | v6 item |
|-----------|---------|
| App F item F.1 (Backhaus) | Module 13 item 13.1 |
| App F item F.2 (Reichelt) | Module 13 item 13.2 |
| App F item F.3 (Gramsci) | Module 13 item 13.3 |
| App F item F.4 (Thomas) | Module 13 item 13.4 |
| App F item F.5 (Althusser) | Module 13 item 13.5 |

---

## 3. Appendix Renaming

Appendices run continuously A–H (no gap).

| v5 letter | v6 letter | Content | Corresponding module |
|-----------|-----------|---------|---------------------|
| C | **A** | Social Epistemology | Module 9 |
| B | **B** | Philosophy of Social Science | Module 10 |
| F (remainder) | **C** | Marxist Traditions — Deepening | Module 13 |
| *(new, from Part VI)* | **D** | Capitalism Critique — Supplementary | Module 14 |
| A | **E** | Zeitdiagnose | Module 15 |
| D | **F** | Social Ontology | Module 17 |
| E | **G** | Phenomenology | Module 16 |
| G | **H** | Socialisation, Child Development | — |

---

## 4. Appendix-Internal Item Prefix Renaming

| v5 prefix | v6 prefix | Appendix | Examples |
|-----------|-----------|----------|----------|
| C.x.x | **A.x.x** | Social Epistemology | C.0.1→A.0.1; C.1.1→A.1.1 |
| B.x.x | **B.x.x** | Phil. Social Science | *(unchanged)* |
| F.0.x, F.6–F.25 | **C.0.x, C.6–C.25** | Marxist Traditions | F.0.1→C.0.1; F.6→C.6; F.13→C.13 |
| F.I–F.IX | **C.I–C.IX** | Marxist (section headers) | ### F.I:→### C.I: |
| K.7–K.13 | **D.1.1–D.3.1** | Capitalism Supplement | K.7→D.1.1; K.12→D.2.3 (see §1 Part VI table) |
| A.x.x | **E.x.x** | Zeitdiagnose | A.0.1→E.0.1; A.1.4→E.1.4 |
| D.x.x | **F.x.x** | Social Ontology | D.0.1→F.0.1; D.1.1→F.1.1 |
| E.x.x, E.A | **G.x.x, G.A** | Phenomenology | E.0.1→G.0.1; E.A→G.A |
| G.x.x | **H.x.x** | Socialisation | G.0.1→H.0.1; G.3.1→H.3.1 |

**Note on Appendix C (Marxist):** Items F.1–F.5 were promoted to Module 13 (13.1–13.5). They do NOT become C.1–C.5. The appendix retains F.0.x (→C.0.x) and F.6–F.25 (→C.6–C.25). References to "F.1"–"F.5" should become "Module 13 item 13.x".

---

## 5. Structural Changes Summary

| Change | Description |
|--------|-------------|
| Motivational Checkpoint | Removed |
| Part VI | Dissolved → Module 14 (essentials) + Appendix D (remainder) |
| Module 13 (new) | Marxist Theoretical Foundations (from Appendix F core) |
| Module 14 (new) | Capitalism as Social Form (from Part VI + Régulation school) |
| Module 18.3 | Graeber & Wengrow *Dawn of Everything* [NE] added |
| Part III reorder | 9→10→11A–D→12→13→14→15→16→17→18 |
| Rival paradigms | New overarching statement before Module 11A |
| Craft Block | C1/C2/C3 → W1/W2/W3 |
| Appendices | Now A–H (continuous); old gap at C closed |
| All appendix items | Prefixes updated to match new appendix letter |
| Letter-suffixed items | 4.2a, 7.8a, 7.8b, 14.2a, 14.6a → continuous numbering |
| Appendix H in DAG | Socialisation now visible in dependency graph |

---

## 6. Substitution Ordering

**Apply in this exact order.**

### Group 1: Module sub-items (most specific first)
```
12D.  →  11D.
12C.  →  11C.
12B.  →  11B.
12A.  →  11A.
13.B  →  12.B
```

### Group 2: Module-level identifiers
```
Module 12D  →  Module 11D
Module 12C  →  Module 11C
Module 12B  →  Module 11B
Module 12A  →  Module 11A
Module 13   →  Module 12       (after 13.B handled)
Module 14   →  Module 18       (old Phil Anthro)
Module 12   →  Module 10       (after 12A-D handled)
Module 10   →  Module 16       (after 12→10 done)
Module 11   →  Module 17       (use regex: Module 11(?![A-D]) to avoid 11A-D)
```

### Group 3: Letter-suffixed items → continuous numbers
```
4.2a   →  4.3     (then shift: old 4.3→4.4, 4.4→4.5, ..., 4.9→4.10)
7.8a   →  7.9     (then shift: old 7.9→7.10, ..., 7.17→7.18, 7.18→7.19)
7.8b   →  7.10    (apply before 7.8a shift to avoid collision)
14.2a  →  14.3    (then shift: old 14.3→14.4, ..., 14.8→14.10)
14.6a  →  14.8    (apply within the 14.x cascade above)
```

### Group 4: Part VI item references
```
K.2a   →  Module 14 item 14.3       (before K.2)
K.6a   →  Module 14 item 14.8       (before K.6)
K.6b   →  Module 14 item 14.9
K.6c   →  Module 14 item 14.10
K.1    →  Module 14 item 14.1
K.2    →  Module 14 item 14.2
K.3    →  Module 14 item 14.4
K.4    →  Module 14 item 14.5
K.5    →  Module 14 item 14.6
K.6    →  Module 14 item 14.7       (after K.6a/b/c)
K.7    →  Appendix D item D.1.1
K.8    →  Appendix D item D.1.2
K.9    →  Appendix D item D.2.1
K.10   →  Appendix D item D.2.2
K.11   →  Appendix D item D.3.1
K.12   →  Appendix D item D.2.3
K.13   →  Appendix D item D.2.4
Part VI  →  Module 14 / Appendix D
```

### Group 5: Craft Block
```
Module C1  →  Module W1
Module C2  →  Module W2
Module C3  →  Module W3
C1.    →  W1.
C2.    →  W2.
C3.    →  W3.
```

### Group 6: Appendix F items promoted to Module 13
```
Appendix F item F.1  →  Module 13 item 13.1
Appendix F item F.2  →  Module 13 item 13.2
Appendix F item F.3  →  Module 13 item 13.3
Appendix F item F.4  →  Module 13 item 13.4
Appendix F item F.5  →  Module 13 item 13.5
```

### Group 7: Appendix letter renaming (placeholder approach)
**Pass 7a — old → placeholder:**
```
Appendix C  →  §APP_A§     (Social Epistemology → A)
Appendix A  →  §APP_E§     (Zeitdiagnose → E)
Appendix D  →  §APP_F§     (Social Ontology → F)
Appendix E  →  §APP_G§     (Phenomenology → G)
Appendix F  →  §APP_C§     (Marxist → C)
Appendix G  →  §APP_H§     (Socialisation → H)
```

**Pass 7b — placeholder → final:**
```
§APP_A§  →  Appendix A
§APP_C§  →  Appendix C
§APP_E§  →  Appendix E
§APP_F§  →  Appendix F
§APP_G§  →  Appendix G
§APP_H§  →  Appendix H
```
(Appendix B unchanged. Appendix D is new, from Part VI.)

### Group 8: Appendix-internal item prefixes (placeholder approach)
**Pass 8a — old → placeholder:**
```
C.   →  §PFX_A§.     (item context only)
A.   →  §PFX_E§.
D.   →  §PFX_F§.
E.   →  §PFX_G§.
F.   →  §PFX_C§.     (F.0.x and F.6+; F.1-F.5 handled in Group 6)
G.   →  §PFX_H§.
```

**Pass 8b — placeholder → final:**
```
§PFX_A§  →  A
§PFX_C§  →  C
§PFX_E§  →  E
§PFX_F§  →  F
§PFX_G§  →  G
§PFX_H§  →  H
```

**Context rule:** Only match patterns clearly being appendix item references: `| X.N`, `### X.N:`, `#### X.Na:`, or in prose preceded by space/parenthesis and followed by digit. Do NOT match author initials (C.H. Beck, G.A. Cohen).

### Group 9: Roman numeral headers in Appendix C (was F)
```
### F.I:    →  ### C.I:
### F.II:   →  ### C.II:
(through F.IX → C.IX)
```

---

## 7. Verification Checklist

After all substitutions, search for these. Any match (outside provenance notes) indicates a missed substitution.

- [ ] `Module 10` in Phenomenology context (→ Module 16)
- [ ] `Module 11` in Ontology context (→ Module 17)
- [ ] `Module 12` in Phil. Social Science context (→ Module 10)
- [ ] `Module 12A` / `12B` / `12C` / `12D` (→ 11A–11D)
- [ ] `Module 13` in Political Philosophy context (→ Module 12)
- [ ] `Module 14` in Phil. Anthropology context (→ Module 18)
- [ ] `13.B` (→ `12.B`)
- [ ] `7.8a` or `7.8b` (→ `7.9` / `7.10`)
- [ ] `4.2a` (→ `4.3`)
- [ ] `14.2a` / `14.6a` (→ `14.3` / `14.8`)
- [ ] `Part VI` outside provenance notes (→ Module 14 / Appendix D)
- [ ] `K.1` through `K.13` (→ Module 14 or Appendix D items)
- [ ] `Module C1` / `C2` / `C3` (→ W1 / W2 / W3)
- [ ] `Appendix I` (→ Appendix H)
- [ ] `Appendix C` in Epistemology context (→ Appendix A)
- [ ] `Appendix A` in Zeitdiagnose context (→ Appendix E)
- [ ] `Appendix D` in Ontology context (→ Appendix F)
- [ ] `Appendix E` in Phenomenology context (→ Appendix G)
- [ ] `Appendix F` in Marxist context (→ Appendix C)
- [ ] `Appendix G` in Socialisation context (→ Appendix H)
- [ ] `Motivational Checkpoint`

---

## 8. Edge Cases

**"Module 12" ambiguity:** In v5 = Phil. Social Science. In v6 = Political Philosophy (was Module 13). Group 2 ordering resolves: by the time "Module 12" is processed, "Module 12A–D" are already 11A–D, so remaining "Module 12" is the old Phil. Social Science → Module 10.

**"Module 14" ambiguity:** In v5 = Phil. Anthropology. In v6 = Capitalism as Social Form (new). Group 2 converts old "Module 14" → "Module 18". Group 4 converts "K.x" → "Module 14 item 14.x".

**"Appendix C" ambiguity:** In v5 = Social Epistemology. In v6 = Marxist Traditions (was F). Group 7 placeholder approach prevents C→A→E chains.

**F.1–F.5 vs. C.1–C.5:** Items F.1–F.5 were promoted to Module 13 (13.1–13.5). They do NOT become C.x. Apply Group 6 (F.1–F.5 → Module 13) BEFORE Group 8 (remaining F.x → C.x).

**Author initials:** The regex for item prefixes must not match "C.H. Beck", "G.A. Cohen", "C.A.J. Coady". Require digit after the dot.
