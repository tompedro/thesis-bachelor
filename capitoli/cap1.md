# Chapter 1 — Classical Mechanics as a Commutative C*-Algebra

**Status**: Index v7 complete — writing in progress
**Open issues**: S1 (redundant C^∞_c(M) description in §1.5)
**Links**: [[concetti/symplectic_geometry]], [[concetti/poisson_brackets]], [[concetti/c_star_algebra]], [[concetti/gelfand_theorem]], [[concetti/gns_construction]]

---

## Logical spine

Lie algebras (language) → symplectic geometry (arena) → Poisson brackets (Lie structure on C^∞(M)) → C_0(M) as C*-algebra (Banach completion) → Gelfand (recognition).

**Chapter conclusion**: CM *is* the theory of commutative C*-algebras. The Lie-bracket is internal structure, not an added axiom.

---

## §1.1 — Lie Algebras

*Prerequisite for every bracket in the thesis — classical and quantum.*

**To cover**:
- Axiomatic definition (g, [·,·]): bilinearity, antisymmetry, Jacobi identity
- Jacobi flagged here as structural coherence condition — link to dω = 0 in §1.3 is the crucial technical thread
- Homomorphisms, representations, universal enveloping algebra (statement only)
- Relevant examples: 𝔰𝔲(2), 𝔲(n); exponential map exp: g → G

**Note**: Every bracket in the thesis — {·,·} in §1.3, [·,·] in §2.1, Poisson on ℙℋ in §3.3 — is a representation of the abstract structure defined here.

---

## §1.2 — Symplectic Geometry

*Introduces C^∞(M) as the natural algebra of observables.*

**Compactness flag**: M is locally compact Hausdorff unless stated otherwise. Results requiring compactness of M are marked *(M compact)*.

**To cover**:
- Symplectic manifold (M, ω): ω closed (dω = 0) and non-degenerate; even dimension, canonical orientation
- Musical isomorphisms ♭: TM → T*M and #: T*M → TM induced by ω
- Hamiltonian vector fields X_f via ι_{X_f} ω = df; existence and uniqueness from musical isomorphism
- **Darboux theorem**: *local* existence of coordinates (qⁱ, pᵢ) with ω = Σ dqⁱ∧dpᵢ. Global Darboux coordinates do NOT exist on compact manifolds like S²
- Symplectomorphisms and Liouville theorem: flow of every Hamiltonian field is a one-parameter group of symplectomorphisms *(completeness guaranteed if M compact, or with growth assumptions on H)*; invariance of Liouville measure ω^n/n!

**Why C^∞(M) here**: defining X_f via ι_{X_f}ω = df requires f differentiable. The passage to C_0(M) happens in §1.5.

---

## §1.3 — Poisson Brackets and Lie Algebra Structure

**Key point**: {f,g} = ω(X_f, X_g). Jacobi ⟺ dω = 0.

**To cover**:
- Poisson bracket: {f,g} = ω(X_f, X_g); bilinearity, antisymmetry, Leibniz rule
- **Jacobi ⟺ dω = 0**: proof via Cartan formula L_X = ι_X d + d ι_X and closure of ω. Ref: Abraham–Marsden Thm 2.4.6; Cannas da Silva Prop. 2.3
- (C^∞(M), {·,·}) as Lie algebra: all axioms of §1.1 satisfied
- Map f ↦ X_f: Lie algebra homomorphism (C^∞(M), {·,·}) → (𝔛(M), [·,·]); kernel = constant functions
- Evolution of observables: d/dt (f∘φ_t^H) = {f,H}∘φ_t^H

**Thread to §3.3**: the same equivalence Jacobi ⟺ dω = 0 guarantees Jacobi on ℙℋ in Chapter 3.

---

## §1.4 — Symplectic Group Actions and Noether's Theorem

**To cover**:
- Lie group G: Lie algebra g = T_e G; exponential map; examples U(1), SU(2), U(n)
- Symplectic action: Φ: G × M → M with Φ_g* ω = ω; infinitesimal generator ξ_M
- Moment map: μ: M → g* defined by d⟨μ,ξ⟩ = ι_{ξ_M} ω. *(For non-compact M, global existence requires completeness of flow of ξ_M; automatic if M compact.)*
- **Noether's theorem**: if H is G-invariant, then d/dt ⟨μ∘φ_t^H, ξ⟩ = {⟨μ,ξ⟩, H} = 0

**Critical note**: this proof uses only symplectic structure and Jacobi identity → applies identically to (ℙℋ, ω) in §3.4. This is why Noether is a theorem, not an axiom, in both theories.

---

## §1.5 — C_0(M) as C*-Algebra and Gelfand's Theorem

*C*-algebra definitions live HERE and are not repeated in Chapter 2.*

**To cover**:
- Why C_0(M) and not C^∞(M)? C*-algebra requires Banach completeness; C^∞(M) admits no natural Banach norm
- C_0(M): continuous functions vanishing at infinity, sup-norm; condition ‖f*f‖ = ‖f‖² holds by construction
- **C^∞_c(M) and C_0(M)**: C^∞_c(M) is **dense** in C_0(M) (NOT a subset — C_0 contains only continuous functions). The Poisson bracket is defined on C^∞_c(M); it does not extend to C_0(M) (first-order differential operator, not sup-norm continuous). *(For M compact: C_0(M) = C(M) and C^∞_c(M) = C^∞(M).)*
- C_0(M) as commutative C*-algebra: sup-norm, involution by complex conjugation
- Self-adjoint elements as classical observables: f = f̄; real spectrum
- State as positive normalised functional: ω: C_0(M) → ℂ with ω(f̄f) ≥ 0, ω(1) = 1; expectation value as primitive physical datum. Parallel to §2.1
- **Gelfand's theorem**: every commutative C*-algebra is isometrically isomorphic to C_0(X) for some locally compact Hausdorff space X *(for M compact: isomorphic to C(X))*
- **Conclusion**: CM *is* the theory of commutative C*-algebras. The Lie-bracket is internal structure of C^∞_c(M) ⊂ C_0(M)

### Pure states and characters: M as the spectrum of C_0(M)

*Closes the parallel with GNS in §2.2/§2.4: Gelfand's theorem, read in reverse, identifies M itself as the pure-state space of C_0(M) — not merely something one derives from C_0(M).*

**To cover**:
- **Characters**: ω: C_0(M) → ℂ multiplicative (ω(fg) = ω(f)ω(g)), ω(1) = 1. Gelfand spectrum Δ(C_0(M)) ≅ M canonically, via x ↦ δ_x, δ_x(f) = f(x)
- **Characters = pure states**: for a commutative C*-algebra, characters coincide exactly with pure states.
  - (⇒) If ω is multiplicative: Gelfand ideal 𝓘_ω = ker ω has codimension 1, since ω(f̄f) = |ω(f)|². Hence ℋ_ω ≅ ℂ, automatically irreducible, so ω is pure.
  - (⇐) If ω is pure: Schur's lemma applied to an abelian algebra — which sits inside its own commutant in any representation of itself — forces dim ℋ_ω = 1, so ω is multiplicative.
- **Explicit GNS check for δ_x**: Gelfand ideal 𝓘_{δ_x} = {f : f(x) = 0}; quotient C_0(M)/𝓘_{δ_x} ≅ ℂ via f ↦ f(x); so ℋ_{δ_x} ≅ ℂ — the GNS representation of a commutative pure state collapses to the minimal possible dimension
- **Parallel with §2.4**: the same scheme (pure states ↔ irreducible GNS representations) applied to a non-commutative algebra no longer forces dim 1 — there ℋ_ω ≅ ℋ (faithful representation) and the pure state is a ray [ψ] ∈ ℙℋ. M and ℙℋ are the *same construction* — pure-state spectrum via GNS — specialised to the two dimensional extremes allowed by Schur's lemma: 1 in the commutative case, dim ℋ in the non-commutative case. Full algebraic argument in §2.4; corresponding row added to the Appendix B table

**Source**: Bratteli & Robinson Vol. I, Prop. 2.3.27 (pure states ↔ irreducible GNS representations); Strocchi Ch. 1.

---

## §1.6 — Qubit I: S² as Phase Space of Classical Spin

**Links**: [[concetti/qubit_thread]]

*S² is compact, so all global existence issues are automatic here.*

**To cover**:
- Working with 1/2 spin: Normalization constant of 1/2
- Phase space S² *(compact)*: symplectic form ω = 1/2 sinθ dθ∧dφ
- Poisson brackets on S²: {xᵢ, xⱼ} = εᵢⱼₖ xₖ — Lie algebra 𝔰𝔲(2) realised as Poisson brackets
- C(S²) as commutative C*-algebra (compact case: C_0 = C)
- State as probability measure on S²
- **Anticipation**: in Ch. 2, [σᵢ, σⱼ] = 2iεᵢⱼₖ σₖ on M₂(ℂ) — same Lie algebra 𝔰𝔲(2), not by analogy but because both are representations of §1.1
