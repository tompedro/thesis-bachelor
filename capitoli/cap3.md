# Chapter 3 — Kähler Geometry of ℙℋ and Recovery of Classical Structures

**Status**: Index v7 complete — writing in progress
**Open issues**: C1 (Qubit III normalization), C3 (state-dependence notation in §3.3), S4 (Noether overuse in §3.4)
**Links**: [[concetti/kahler_geometry]], [[concetti/stone_theorem]], [[concetti/symplectic_geometry]], [[concetti/qubit_thread]]

---

## Logical spine

ℙℋ as manifold → inner product decomposition produces Kähler structure → Stone on ℋ, flow descends to ℙℋ → Schrödinger equation as Hamiltonian flow → Noether from Jacobi → uncertainty from Kähler geometry.

**Top-down answer**: the geometric structures of Ch. 1 are literally present in ℙℋ as consequences of its intrinsic geometry. They are not imported from the classical theory.

**Key reuse**: Stone's theorem (§2.3) is used here explicitly. The theorem acts on ℋ; the flow descends to ℙℋ via linearity.

---

## §3.1 — ℙℋ as a Manifold

**To cover**:
- Phase redundancy: |ψ⟩ and e^{iθ}|ψ⟩ give identical expectation values; ℙℋ = (ℋ \ {0})/∼
- Real differentiable structure of dimension 2(dim ℋ − 1)
- **Finite-dimensional case** (dim ℋ = n): ℙℋ ≅ ℂP^{n−1}, compact
- **Infinite-dimensional case** (separable ℋ): Hilbert manifold, non-compact; local properties (symplectic form, Hamiltonian fields) remain valid; global existence of flow requires Ĥ essentially self-adjoint — guaranteed by spectral theorem of §2.3

**Sources**: Ashtekar & Schilling (gr-qc/9706069); Cirelli, Lanzavecchia & Mania (J. Math. Phys. 31, 1990).

---

## §3.2 — Decomposition of the Inner Product and Kähler Structure

*Kähler is defined here — one line — at the moment it is needed.*

**Links**: [[concetti/kahler_geometry]]

**To cover**:
- **Fundamental decomposition** on ℋ as real vector space:
  ⟨ψ|φ⟩ = g(ψ,φ) + i ω(ψ,φ)
  where g = Re⟨·|·⟩ is a Riemannian metric and ω = Im⟨·|·⟩ is an antisymmetric 2-form
- Non-degeneracy of ω: ω is symplectic
- Complex structure J: ψ ↦ iψ; J² = −Id; compatibility ω(ψ,φ) = g(Jψ,φ)
- **Kähler triple** (g, J, ω): the three structures are mutually compatible and ω is closed
- **Descent to ℙℋ**: the triple (g, J, ω) descends to the quotient and satisfies Kähler compatibility conditions
- Kähler potential and closure of ω: in local chart U_0 with coordinates z_j = ψ_j/ψ_0, potential K = log(1 + Σ|z_j|²) generates ω = i∂∂̄K; closure dω = 0 follows from nilpotency ∂² = 0
- **Fubini–Study metric**: the Riemannian component g is the Fubini–Study metric

**Note on Nijenhuis/Newlander–Nirenberg**: integrability of complex structure is NOT needed here; verified directly via Kähler potential.

**Sources**: Ashtekar & Schilling; Cirelli, Lanzavecchia & Mania.

---

## §3.3 — Schrödinger Equation as Hamiltonian Flow

**Links**: [[concetti/stone_theorem]]

**To cover**:
- Observable as smooth function: given self-adjoint Â, f_A([ψ]) = ⟨ψ|Â|ψ⟩/⟨ψ|ψ⟩ is smooth on ℙℋ; direct analogue of classical observable in §1.3
- Hamiltonian vector field: X_{f_H} from ι_{X_{f_H}} ω = df_H
- **Stone on ℋ, flow on ℙℋ** (Ashtekar–Schilling Prop. 3.1):
  1. Stone (§2.3) produces unitary flow U(t) = e^{-iĤt/ℏ} on ℋ
  2. U(t) is linear and commutes with scalar multiplication
  3. Therefore U(t) *descends* to ℙℋ: Φ_t([ψ]) = [e^{-iĤt/ℏ} ψ]
  4. The descended flow coincides with the Hamiltonian flow of X_{f_H} w.r.t. ω
- **Stone acts on ℋ. The flow descends to ℙℋ. Stone is never applied directly to ℙℋ.**
- Schrödinger equation: orbits of Φ_t satisfy iℏ ∂_t|ψ⟩ = Ĥ|ψ⟩ — consequence of the descended unitary flow, not an independent axiom
- **Fundamental geometric identity**:

$$\{f_A, f_B\}_\omega \big|_{[\psi]} = \omega(X_{f_A}, X_{f_B})\big|_{[\psi]} = \frac{\langle\psi|[\hat{A},\hat{B}]|\psi\rangle}{i\hbar\langle\psi|\psi\rangle}$$

---

## §3.4 — Quantum Noether Theorem

**To cover**:
- **Statement**: if [Ĥ,Â] = 0, then d/dt ⟨Â⟩_ψ = 0 along every solution of the Schrödinger equation
- **Geometric proof**: [Ĥ,Â] = 0 implies {f_H, f_A}_ω = 0 by §3.3 identity; by Noether's theorem of §1.4 applied to (ℙℋ, ω), f_A is conserved along flow of X_{f_H}; conservation follows from Jacobi identity, guaranteed by dω = 0 on ℙℋ (§3.2)
- Quantum moment map: μ_Q: ℙℋ → g* defined by ⟨μ_Q([ψ]), ξ⟩ = ⟨ψ|T̂_ξ|ψ⟩; exact counterpart of classical moment map of §1.4

**Sources**: Cirelli, Lanzavecchia & Mania; Ashtekar & Schilling.

---

## §3.5 — Uncertainty Relations as Corollary

**To cover**:
- Origin from symplectic structure: Cauchy–Schwarz on ℋ gives
  Δ_ψ A · Δ_ψ B ≥ ½|⟨ψ|[Â,B̂]|ψ⟩|
  Via §3.3 identity, the RHS is (ℏ/2)|{f_A, f_B}_ω|_{[ψ]}
- **Nature of result**: intrinsic to the Kähler geometry of ℙℋ, without direct classical analogue
- Some structures of CM reappear identically (Noether, flow); uncertainty relations are genuinely quantum

**Sources**: Reed & Simon Vol. I; Moretti.

---

## §3.6 — Qubit III: ℙℂ¹ ≅ S² — Geometric Closure

**Links**: [[concetti/qubit_thread]]

**To cover**:
- For ℋ = ℂ², construction of §3.1 gives ℙℋ = ℙℂ¹ ≅ S² (stereographic projection via chart U_0 = {[ψ_0,ψ_1]: ψ_0 ≠ 0}, coordinate z = ψ_1/ψ_0)
- Kähler potential on ℙℂ¹: K = log(1 + |z|²)
- Fubini–Study form in spherical coordinates z = tan(θ/2)e^{iφ}:
  ω_FS = i dz∧dz̄/(1+|z|²)² = **½ sinθ dθ∧dφ**
- Larmor precession as Hamiltonian flow: Ĥ = −(γB/2)σ_z; flow U(t) descends to rotation φ ↦ φ + γBt on S²