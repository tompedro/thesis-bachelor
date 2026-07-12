# Chapter 2 — Algebraic Construction of Quantum Mechanics

**Status**: Index v7 complete — writing in progress
**Open issues**: S3 (undeclared ℏ=1 convention in angular momentum commutation relations)
**Links**: [[concetti/c_star_algebra]], [[concetti/gns_construction]], [[concetti/wintner_theorem]], [[concetti/stone_theorem]], [[concetti/qubit_thread]]

---

## Logical spine

Operational axioms (no ℋ) → [a,b] = ab − ba as internal structure → GNS produces ℋ as consequence → Wintner forces unbounded operators → Weyl algebra resolves CCR → Stone marks flow generator → bridge to ℙℋ geometry.

**Parallel with Ch. 1**: as C_0(M) is recognised as commutative C*-algebra by Gelfand, B(ℋ) is recognised as non-commutative C*-algebra by Gelfand–Naimark. The Lie-bracket [a,b] = ab − ba is internal structure, not an axiom.

**Constraint**: C*-algebra definitions and states are NOT reintroduced here — they live in §1.5.

---

## §2.1 — Strocchi's Operational Approach

*Starting point: preparations and measurements. No Hilbert space assumed.*

**To cover**:
- The C*-algebra structure is already known from §1.5; now the algebra is non-commutative
- The Lie-bracket [a,b] = ab − ba: antisymmetry and Jacobi follow from algebra structure alone
- **Parallel §1.3**: in classical mechanics the Lie-bracket was also internal structure, not an axiom
- State as positive normalised functional: same definition as §1.5

**Source**: Strocchi (2008), Ch. 1–2.

---

## §2.2 — GNS Theorem, Gelfand–Naimark, Technical Complements

**To cover**:
- GNS inner product: given state ω, ⟨a,b⟩_ω = ω(a*b)
- Gelfand ideal: 𝒥_ω = {a : ω(a*a) = 0}
- GNS space ℋ_ω: completion of 𝒜/𝒥_ω; representation π_ω: 𝒜 → B(ℋ_ω); cyclic vector Ω_ω = [I]
- **GNS theorem**: every state determines a unique (up to unitary equivalence) representation (ℋ_ω, π_ω, Ω_ω). ℋ *emerges* from the algebraic structure. Uniqueness proof via explicit construction of unitary isomorphism (full proof in Appendix A)
- **Gelfand–Naimark theorem**: every abstract C*-algebra embeds isometrically into B(ℋ); Hilbert space is the natural support of any C*-algebra
- Technical complement: Weyl algebra CCR(ℝ^{2n}) for n > 1 (needed for §2.3 and §4.4); see Appendix A

**Source**: Reed & Simon Vol. I §VIII; Moretti §8–9; Strocchi; Bratteli & Robinson Vol. I.

---

## §2.3 — Wintner's Obstruction and the Weyl Algebra

*Before Wintner: minimal spectral theory prerequisites.*

**Links**: [[concetti/wintner_theorem]], [[concetti/stone_theorem]]

### Spectral theory prerequisite

- Symmetric vs. self-adjoint operators on ℋ: distinction is essential because q̂, p̂ are unbounded and symmetric, but Stone's theorem requires self-adjointness
- Spectral theorem for unbounded operators (statement); measurable functional calculus
- These tools reappear in §2.3 (Stone) and Ch. 3

### Wintner–Wielandt theorem

**Statement**: In any unital Banach algebra, there exist no elements A, B with AB − BA = I.

**Proof**: By induction, AB^n − B^n A = nB^{n−1}. Therefore n‖B‖^{n−1} ≤ ‖AB^n − B^n A‖ ≤ 2‖A‖‖B‖^n, giving n ≤ 2‖A‖‖B‖ for all n — contradiction.

**Scope**: valid for any Banach algebra, without trace argument, without dimension restriction.

**Consequence**: the CCR [q,p] = iℏI cannot be satisfied by bounded operators in any unital Banach algebra.

### Weyl algebra

- Weyl operators: W(α) = e^{i(sq̂+tp̂)}, α = (s,t) ∈ ℝ²; unitary (bounded) even though q̂, p̂ are not
- Weyl relations: W(α)W(β) = e^{(i/2)ω(α,β)} W(α+β); CCR in exponentiated form, no domain issues
- C*-algebra of Weyl CCR(ℝ²): completion in C*-norm; uniqueness of norm (‖W(α)‖ = 1 from C* condition)

### Stone's theorem *(marked: reused in §3.3)*

**Statement**: Every strongly continuous unitary group {U(t)}_{t∈ℝ} on ℋ admits a unique self-adjoint generator H with U(t) = e^{-iHt/ℏ}; conversely, every self-adjoint operator generates such a group.

⚠️ **Convention**: ℏ = 1 must be declared explicitly if used here [S3].

### Stone–von Neumann theorem

Every strongly continuous irreducible representation of CCR(ℝ^{2n}) is unitarily equivalent to the Schrödinger representation on L²(ℝ^n); kinematic uniqueness for finitely many degrees of freedom *(fails in infinite dimension)*.

---

## §2.4 — Bridge to the Geometry of States

*Hinge between Ch. 2 and Ch. 3. No new technical tools — formulates the question Ch. 3 answers.*

**To cover**:
- The algebraic symmetry: CM and QM are both C*-algebras with the Lie-bracket as internal structure
- In the classical case, the bracket drives Hamiltonian flow on (M,ω), defines the moment map, makes Noether a theorem on the manifold
- **The question**: since the Lie-bracket of QM is the same abstract structure, is there a space where the geometric structures of CM — symplectic form, Hamiltonian fields, moment map — are literally present in the quantum case?
- The trace of the answer: GNS produced ℋ; Stone says every self-adjoint observable generates a unitary flow on ℋ; the quotient ℙℋ removes phase redundancy
- **Question posed**: is ℙℋ a symplectic manifold? Does the unitary flow descend to Hamiltonian flow on ℙℋ? → Ch. 3 answers yes

### Why dim 1 in the commutative case and dim ℋ in the non-commutative case: Schur's lemma

*Answers algebraically, ahead of the Kähler geometry of Ch. 3, the question posed above: the M ↔ Δ(C_0(M)) construction of §1.5 and the ℙℋ construction of Ch. 3 are the same construction — the pure-state space via GNS — applied to the two dimensional extremes of the observable algebra.*

**To cover**:
- **General fact (any C*-algebra 𝒜)**: a state ω is pure iff its GNS representation (ℋ_ω, π_ω) is irreducible. (π_ω-invariant subspaces ↔ convex decompositions of ω as a mixture of other states.)
- **Schur's lemma**: if π: 𝒜 → B(ℋ) is irreducible, the commutant π(𝒜)′ = {T ∈ B(ℋ) : Tπ(a) = π(a)T ∀a} is trivial: π(𝒜)′ = ℂ·Id
- **Commutative case (§1.5)**: 𝒜 sits inside its own commutant (π(a)π(b) = π(b)π(a) for all a,b), so π(𝒜) ⊆ π(𝒜)′ = ℂ·Id by Schur. Every operator in the representation is a scalar multiple of the identity — the only way an irreducible representation can satisfy this is dim ℋ_ω = 1. This is exactly the explicit §1.5 computation for δ_x, now derived from pure representation theory
- **Non-commutative case (𝒜 = B(ℋ) or M_n(ℂ))**: the constraint π(𝒜) ⊆ π(𝒜)′ no longer holds. For a pure state ω_ψ(a) = ⟨ψ|a|ψ⟩, the GNS representation is (unitarily equivalent to) the defining representation on ℋ_ω ≅ ℋ itself — faithful, full-dimensional; the pure state corresponds to the ray [ψ] ∈ ℙℋ
- **Synthesis**: M ≅ {pure states of C_0(M)} and ℙℋ ≅ {pure states of B(ℋ)} are not analogous by coincidence — they are the *same construction* (pure-state spectrum via irreducible GNS representation), specialised to the two dimensional extremes permitted by Schur's lemma: dim ℋ_ω = 1 if the algebra is commutative, dim ℋ_ω = dim ℋ if the algebra admits non-trivial faithful irreducible representations. Ch. 3 builds the symplectic-Kähler geometry *on* ℙℋ; this paragraph justifies its identification as the correct "space of points," at the purely algebraic level, before any geometry is introduced
- **Technical note (sectors)**: for an algebra not irreducibly represented on a single ℋ, the pure-state space decomposes as ⊔_π ℙℋ_π over unitary equivalence classes of irreducible representations (superselection sectors). For 𝒜 = B(ℋ) — the case relevant to this thesis — there is a single sector, and ℙℋ alone exhausts the pure-state space

**Source**: Bratteli & Robinson Vol. I, Prop. 2.3.27 & 2.4.4; Landsman Ch. I.2.

---

## §2.5 — Qubit II: M₂(ℂ) as a C*-Algebra

**Links**: [[concetti/qubit_thread]]

**To cover**:
- Observable algebra 𝒜 = M₂(ℂ); Hermitian matrices as observables; [σᵢ, σⱼ] = 2iεᵢⱼₖ σₖ
- States as density matrices: ρ ≥ 0, tr(ρ) = 1; pure states (ρ² = ρ) and mixed states (tr(ρ²) < 1)
- Explicit GNS for the tracial state ω(a) = ½ tr(a): space ℂ², cyclic vector Ω = (1/√2)(1,1)^T. Explicit calculation
- **Comparison with Qubit I**: [σᵢ,σⱼ] = 2iεᵢⱼₖ σₖ in M₂(ℂ) and {xᵢ,xⱼ} = εᵢⱼₖ xₖ on S² — same Lie algebra 𝔰𝔲(2), two distinct representations
