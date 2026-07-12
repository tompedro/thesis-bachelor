# Chapter 4 — Strict Deformation Quantization (Rieffel)

**Status**: Index v7 complete — writing in progress
**Open issues**: C2 (Dirac exactness overstated in §4.6), C4 (undefined Ã in §4.3), S2 (Qubit IV title), S3 (ℏ=1 convention)
**Links**: [[concetti/c_star_algebra]], [[concetti/qubit_thread]]

---

## Logical spine

Three roles of ℏ → formal deformation insufficient → Rieffel's definition (true C*-algebras + Dirac condition) → Weyl quantization as main example → Groenewold–van Hove delimits the result → Qubit IV closes the loop.

**Complementary answer**: CM and QM are fibres of the same continuous field of C*-algebras. The Dirac condition guarantees that Poisson bracket and commutator are the same structure in norm for ℏ → 0.

**Chapter dignity**: this chapter is not secondary. If page constraints require cuts, they are made elsewhere.

---

## §4.1 — The Meaning of ℏ as a Parameter

**Three regimes**:
1. **Fixed physical constant** (Chs. 1–2): kinematic regime; ℏ appears in CCR as a fixed scale
2. **Formal variable**: parameter in power series ℝ[[ℏ]]; basis of formal deformation quantization (§4.2)
3. **Continuous index ℏ ∈ [0,1]**: parametrises fibres of a continuous field of C*-algebras; classical limit ℏ → 0 is a norm limit (§§4.3–4.4)

**Source**: Landsman, *Mathematical Topics Between Classical and Quantum Mechanics*.

---

## §4.2 — Why Formal Deformation is Not Enough

**To cover**:
- Formal star-product (BFFLS): f ★_ℏ g = Σ_{k=0}^∞ ℏ^k B_k(f,g); B_0 = fg; B_1(f,g) − B_1(g,f) = i{f,g}
- **Problem**: formal power series do not define a C*-algebra; no convergence norm; the limit ℏ → 0 has no norm meaning
- **Why strict DQ is needed**: true C*-algebra for each ℏ, continuity in norm

**Sources**: Landsman; Kontsevich (Lett. Math. Phys. 66, 2003).

---

## §4.3 — Rieffel's Definition and Dirac's Condition

**Links**: [[letteratura/Rieffel_1993]]

**To cover**:
- **Definition (Rieffel, 1993)**: a strict deformation quantization of (A_0, {·,·}) is a family {A_ℏ}_{ℏ∈I} of C*-algebras with A_0 = C_0(M) and maps Q_ℏ: Ã_0 → A_ℏ defined on dense subalgebra Ã_0 ⊂ A_0
- Here Ã_0 denotes, a dense subalgebra of C_0(M) on which the Poisson bracket {·,·} is well-defined.

---

**Three conditions**:
1. Q_ℏ(f̄) = Q_ℏ(f)*  (compatibility with involution)
2. ‖Q_ℏ(f)‖_{A_ℏ} → ‖f‖_{A_0} as ℏ → 0  (norm convergence)
3. **Dirac condition**: ‖(1/iℏ)[Q_ℏ(f), Q_ℏ(g)] − Q_ℏ({f,g})‖_{A_ℏ} → 0 as ℏ → 0

- **What Dirac guarantees**: not equality between commutator and Poisson bracket, but their difference small in C*-norm for small ℏ. Classical structures persist as *norm limits*
- Continuous field: CM and QM connected by an asymptotic limit in norm topology — not an ontological discontinuity

**Sources**: Rieffel (Mem. AMS, 1993); Landsman.

---

## §4.4 — Main Example: Weyl Quantization on ℝ²

**To cover**:
- Setup: A_0 = C_0(ℝ²); A_ℏ = CCR(ℝ²); Q_ℏ^W(f) = (1/2πℏ) ∫ f(q,p) W(q,p) dq dp
- Verification of three Rieffel conditions:
  1. Involution compatibility: from properties of Weyl operators
  2. Norm limit: ‖Q_ℏ^W(f)‖ → ‖f‖_∞ via Calderón–Vaillancourt estimate
  3. Dirac condition: from explicit computation of commutator of Weyl operators
- **Hudson's theorem**: for pure state ρ = |ψ⟩⟨ψ|, Wigner function W_ψ ≥ 0 iff ψ is Gaussian
- **Conclusion**: the Dirac correspondence is not an analogy — it is a normed inequality

**Sources**: Landsman, *Mathematical Topics*, Ch. II.1; Hudson (Rep. Math. Phys. 6, 1974).

---

## §4.5 — Groenewold–van Hove Obstruction

**To cover**:
- **Theorem**: no linear map Q: 𝒫(ℝ^{2n}) → L(ℋ) exists satisfying the exact Dirac rules on the polynomial algebra; conflict emerges on monomials of degree ≤ 4
- **Compatibility with Rieffel**: the Dirac condition is *asymptotic* (ℏ → 0), not an exact equality for ℏ > 0. GvH forbids exact equality; does not forbid asymptotic continuity
- **Scope**: for fixed ℏ > 0, quantization cannot be an exact Lie algebra homomorphism on all C^∞

**Sources**: Moretti, *Spectral Theory and QM*, p. 605; Gotay (arXiv:math-ph/9809011).

---

## §4.6 — Qubit IV: Dirac Condition on 𝔰𝔲(2) — Explicit Verification

**Links**: [[concetti/qubit_thread]]

**Setup**: ℏ = 1/j with j ∈ ½ℕ, j → ∞; quantum fibre A_j = M_{2j+1}(ℂ), renormalised generators x̂_i = Ĵ_i/j; classical fibre A_0 = C(S²), coordinates xᵢ, brackets {xᵢ,xⱼ} = εᵢⱼₖ xₖ.

**Calculation**:
(1/iℏ)[x̂_i, x̂_j] = (j/i)[Ĵ_i/j, Ĵ_j/j] = (1/ij)[Ĵ_i,Ĵ_j] = εᵢⱼₖ Ĵ_k/j = εᵢⱼₖ x̂_k

**Dirac condition**: ‖(1/iℏ)[Q_j(xᵢ), Q_j(xⱼ)] − Q_j({xᵢ,xⱼ})‖_{A_j} = 0 for all j.

The condition, in this case, holds *exactly*, not asymptotically — because 𝔰𝔲(2) is a finite-dimensional Lie algebra and the quantization is one of its representations. The Dirac condition holds exactly on the generators xᵢ, because they span a finite-dimensional Lie algebra and Q_j is a Lie algebra representation. For general f ∈ C^∞(S²), only the asymptotic statement (ℏ → 0) holds.

---

**Coherent states convergence**: SU(2) coherent states |θ,φ;j⟩ satisfy, for j → ∞:
⟨θ,φ;j|x̂_i|θ,φ;j⟩ → x_i(θ,φ)

Expectation value of operator converges to classical function pointwise on S²: quantum fibre A_j converges to classical fibre A_0 = C(S²).

**Closure of algebraic loop**: Qubit I places Poisson structure on S²; Qubit II identifies M₂(ℂ) as non-commutative C*-algebra with same Lie bracket; Qubit III shows both state spaces are the same symplectic manifold; Qubit IV shows the normalised commutator *is* the Poisson bracket — by construction, not in the limit.

**Thesis answer**: the structures were never absent from the quantum theory. The question dissolves.
