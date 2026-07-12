# CLAUDE.md — Hamiltonian Structures in Quantum Mechanics

> **Read this file at the start of every session before doing anything else.**
> This is the single source of truth for the thesis project.

---

## 1. Project Overview

| Field | Value |
|-------|-------|
| **Title (EN)** | Hamiltonian Structures in Quantum Mechanics |
| **Title (IT)** | Strutture Hamiltoniane in Meccanica Quantistica |
| **Author** | Tommaso Pedroni |
| **Supervisor** | Prof. Claudio Dappiaggi |
| **Institution** | Università degli Studi di Pavia (UNIPV) |
| **Degree** | Undergraduate thesis in Mathematical Physics |
| **Language** | **English** (planning documents in Italian) |
| **Typesetting** | LaTeX (`final.tex`, currently index v7) |
| **Target length** | ~120 pages (hard constraint: 100–150 pages) |

---

## 2. Central Research Question

Why do structures from classical mechanics — symplectic manifolds, Poisson brackets, Hamiltonian flow, Noether's theorem — reappear in quantum mechanics without being postulated in its axioms?

### Answer (two complementary readings)

**Bottom-up** (Ch. 1–2 + Ch. 4): Both CM and QM are C*-algebras — one commutative, one not — connected by a continuous field via Rieffel's strict deformation quantization. The classical Lie-bracket and the quantum commutator are the *same abstract structure* in two distinct representations.

**Top-down** (Ch. 3): The quantum state space ℙℋ is a Kähler symplectic manifold. Symplectic form, Hamiltonian fields, moment map, and Noether's theorem do not come from outside: they emerge from the decomposition of the inner product of ℋ.

> **Warning**: Do not frame the answer as "structures reappear." The correct framing is "they never left." The question dissolves once the shared algebraic structure is made explicit.

---

## 3. Thesis Structure

### Chapter 1 — Classical Mechanics as a Commutative C*-Algebra

| Section | Content |
|---------|---------|
| §1.1 | Lie Algebras — prerequisite for all brackets in the thesis |
| §1.2 | Symplectic Geometry — introduces C^∞(M), Darboux, Liouville |
| §1.3 | Poisson Brackets and Lie Algebra Structure |
| §1.4 | Symplectic Group Actions and Noether's Theorem |
| §1.5 | C_0(M) as C*-Algebra and Gelfand's Theorem — **C*-algebra definitions live HERE** |
| §1.6 | **Qubit I** — S² as phase space of classical spin |

**Chapter conclusion**: CM *is* the theory of commutative C*-algebras (Gelfand).

---

### Chapter 2 — Algebraic Construction of Quantum Mechanics

| Section | Content |
|---------|---------|
| §2.1 | Strocchi's Operational Approach (no Hilbert space assumed) |
| §2.2 | GNS Theorem, Gelfand–Naimark, Technical Complements |
| §2.3 | Wintner's Obstruction and the Weyl Algebra — **Stone's theorem marked here for reuse in Ch. 3** |
| §2.4 | Bridge to the Geometry of States |
| §2.5 | **Qubit II** — M₂(ℂ) as a C*-Algebra |

**Critical constraint**: C*-algebra definitions are NOT repeated in Ch. 2 (already in §1.5).

---

### Chapter 3 — Kähler Geometry of ℙℋ and Recovery of Classical Structures

| Section | Content |
|---------|---------|
| §3.1 | ℙℋ as a Manifold (real structure, finite vs. infinite dimension) |
| §3.2 | Decomposition of the Inner Product and Kähler Structure |
| §3.3 | Schrödinger Equation as Hamiltonian Flow |
| §3.4 | Quantum Noether Theorem |
| §3.5 | Uncertainty Relations as Corollary |
| §3.6 | **Qubit III** — ℙℂ¹ ≅ S²: Geometric Closure |

---

### Chapter 4 — Strict Deformation Quantization (Rieffel)

| Section | Content |
|---------|---------|
| §4.1 | The Meaning of ℏ as a Parameter (three regimes) |
| §4.2 | Why Formal Deformation is Not Enough |
| §4.3 | Rieffel's Definition and Dirac's Condition |
| §4.4 | Main Example: Weyl Quantization on ℝ² |
| §4.5 | Groenewold–van Hove Obstruction |
| §4.6 | **Qubit IV** — Dirac Condition on 𝔰𝔲(2): Explicit Verification |

**Important**: Ch. 4 retains full dignity regardless of page constraints. If the thesis must be shortened, other sections are cut first.

---

## 4. The Qubit Thread

A transversal worked example runs across all four chapters.

| # | Location | Content |
|---|----------|---------|
| **Qubit I** | §1.6 | S² as classical phase space; {xᵢ, xⱼ} = εᵢⱼₖ xₖ |
| **Qubit II** | §2.5 | M₂(ℂ) as C*-algebra; [σᵢ, σⱼ] = 2i εᵢⱼₖ σₖ — same Lie algebra 𝔰𝔲(2) |
| **Qubit III** | §3.6 | ℙℂ¹ ≅ S² as symplectic manifolds (same ω up to normalization) |
| **Qubit IV** | §4.6 | Dirac condition holds *exactly* on 𝔰𝔲(2) generators (not asymptotically) |

The four Qubits form a closed loop: same physical system, four mathematical perspectives.

---

### C^∞_c(M) vs C_0(M)

| Statement | Status |
|-----------|--------|
| C^∞_c(M) ⊂ C_0(M) | **FALSE** — C_0 contains only continuous functions |
| C^∞_c(M) dense in C_0(M) | **TRUE** — correct statement |
| Poisson bracket extends to all of C_0(M) | **FALSE** — first-order differential operator, not sup-norm continuous |

---

### Kähler Structure on ℙℋ (§3.2)

Inner product decomposition: ⟨ψ|φ⟩ = g(ψ,φ) + i ω(ψ,φ)

- **g** = Re⟨·|·⟩ → Fubini–Study metric (Riemannian part)
- **ω** = Im⟨·|·⟩ → symplectic form
- **J**: ψ ↦ iψ → complex structure, J² = −Id, ω(ψ,φ) = g(Jψ,φ)

Kähler potential in chart U_0: K = log(1 + Σ|z_j|²) → ω = i∂∂̄K → dω = 0 from ∂² = 0.

---

## Supervisor Context

**Prof. Claudio Dappiaggi** suggested:
- C*-algebras via Strocchi
- Symplectic structure on ℙℋ via inner product decomposition (without naming Kähler)
- Landsman for classical limit and strict deformation quantization

Tom introduced the **Kähler framework independently** — accepted by supervisor, not further developed by him.

> **Kähler is a tool, not a thesis.** It should emerge as the earned name of an already-constructed object, never foregrounded as motivation.

---

## Hard Constraints and Principles

### Forbidden moves

- ❌ Foregrounding Kähler geometry as motivation or conclusion
- ❌ Claiming B(ℋ) contains C_0(M) — false
- ❌ Applying Stone's theorem directly to ℙℋ
- ❌ Adding content not strictly necessary for the logical argument
- ❌ Repeating C*-algebra definitions in Ch. 2

### Required behaviors

- ✅ Flag compactness requirements explicitly: *(M compact)*
- ✅ Include [ψ] in all state-dependent expressions
- ✅ Declare ℏ = 1 convention whenever used
- ✅ Each section must logically necessitate the next
- ✅ Minimalism over comprehensiveness

---

##  Key References

| Reference | Role |
|-----------|------|
| Strocchi (2008) | C*-algebras, Wintner's theorem |
| Landsman, *Mathematical Topics Between Classical and Quantum Mechanics* | Classical limit, strict DQ |
| Ashtekar & Schilling, gr-qc/9706069 | ℙℋ geometry, Stone descent (Prop. 3.1) |
| Rieffel, Mem. AMS (1993) | Strict DQ definition |
| Abraham & Marsden, *Foundations of Mechanics* | Symplectic geometry |
| Cannas da Silva, *Lectures on Symplectic Geometry* | Symplectic geometry |
| Reed & Simon, Vol. I | Spectral theory |
| Moretti, *Spectral Theory and QM* | Spectral theory, Noether |
| Bratteli & Robinson, Vols. I–II | Operator algebras |
| Cirelli, Lanzavecchia & Mania, J. Math. Phys. 31 (1990) | Quantum Noether, ℙℋ structure |

Detailed notes on each reference live in `letteratura/`.

---

## Vault Structure

```
Tesi/
├── _contesto/
│   └── CLAUDE.md          ← YOU ARE HERE
├── capitoli/
│   ├── cap1.md            ← Chapter 1 draft and section notes
│   ├── cap2.md
│   ├── cap3.md
│   └── cap4.md
├── letteratura/
│   ├── Landsman_1998.md
│   ├── Strocchi_2008.md
│   ├── Ashtekar_Schilling_1997.md
│   └── ...
└── concetti/
    ├── c_star_algebra.md
    ├── kahler_geometry.md
    ├── stone_theorem.md
    ├── gelfand_theorem.md
    ├── gns_construction.md
    └── ...
```

---

## Session Protocol

1. **Read this file first.**
2. Check the outstanding issues table (§6) — know which are open.
3. Open the relevant chapter file in `capitoli/`.
4. Open relevant concept files in `concetti/` as needed.
5. When adding new content, ask: *is this strictly necessary for the argument?*
6. When an issue is resolved, mark it with ~~strikethrough~~ and add the date.
---
## Claude's Operational Directives (Slash Commands)

Claude operates exclusively through explicit modes invoked by the user via slash commands. If a text is provided without a command, Claude must halt and ask which skill to apply. 

### 🛠️ The Toolset

* **/academic-proofreader**
    * **Goal:** Transcode hybrid Italian/English drafts into rigorous Academic English or fix existing English text.
    * **Action:** Corrects grammar, ensures appropriate mathematical physics vocabulary (e.g., "self-adjoint", "pullback", "manifold"), and enforces the impersonal/plural register ("We consider", "It follows that").
    * **Output:** The fully corrected text, followed by a brief bulleted list of the major syntactical errors fixed, serving as pedagogical feedback.

* **/academic-condenser**
    * **Goal:** Actively enforce the 100-150 page limit constraint.
    * **Action:** Takes the user's text and ruthlessly strips verbose transitions, redundant philosophical digressions, and over-explained trivial steps. Maximizes information density.
    * **Constraint:** Must NEVER alter, skip, or condense the LaTeX mathematical blocks (`$` and `$$`). Math remains exactly as provided.

* **/humanizer**
    * **Goal:** Eradicate "AI-like" repetitive cadences and predictable sentence structures.
    * **Action:** Refines the text to ensure it reads like a natural, high-level academic paper written by a human mathematician. Varies sentence length, uses natural academic transitional phrases, and eliminates overly dramatic or robotic vocabulary (e.g., avoids words like "delve", "crucial", "tapestry").

* **/thesis-reviewer-lite**
    * **Goal:** Heavy, rigorous structural and logical critique (invoked ONLY when explicitly called).
    * **Action:** Does NOT rewrite the text. Instead, acts as a peer reviewer. Identifies logical leaps in mathematical derivations, checks for alignment with the thesis ontology (e.g., ensuring Stone's theorem is not misapplied, checking for the `[ψ]` notation), and points out weak arguments. 
    * **Output:** A structured critique with actionable bullet points.