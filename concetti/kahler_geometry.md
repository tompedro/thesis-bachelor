# Kähler Geometry of ℙℋ

**Defined in thesis**: §3.2 (inline, one line, at the point of use)
**Links**: [[cap3]], [[symplectic_geometry]]

---

## Role in the thesis

Kähler geometry is a **tool**, not the thesis's conclusion. It should emerge as the *earned name* of an already-constructed object.

**Do not foreground Kähler geometry as motivation.** The structure is first built (inner product decomposition), then named.

---

## Kähler triple

A **Kähler manifold** is a triple (g, J, ω) where:
- g is a Riemannian metric
- J is an integrable complex structure (J² = −Id)
- ω is a symplectic form (closed, non-degenerate)

satisfying **compatibility**: ω(u,v) = g(Ju,v).

On ℙℋ this is not an assumption — it is a consequence of the inner product on ℋ.

---

## Construction on ℙℋ (from §3.2)

Starting from the inner product on ℋ, decompose:

⟨ψ|φ⟩ = g(ψ,φ) + i ω(ψ,φ)

- **g** = Re⟨·|·⟩ → Fubini–Study metric
- **ω** = Im⟨·|·⟩ → symplectic form
- **J**: ψ ↦ iψ → complex structure

Compatibility: ω(ψ,φ) = g(Jψ,φ) ✓

The triple (g,J,ω) descends to ℙℋ and satisfies Kähler conditions.

---

## Kähler potential and closure

Local chart U_0 with coordinates z_j = ψ_j/ψ_0:

K = log(1 + Σ|z_j|²)    →    ω = i∂∂̄K    →    dω = 0  (from ∂² = 0)

The closure dω = 0 — which guarantees the Jacobi identity for {·,·} — follows from the nilpotency of ∂, not from an additional assumption.

---

## Integrability

Nijenhuis tensor and Newlander–Nirenberg are NOT needed. Integrability of J is verified directly via the Kähler potential.

---

## Sources

- Ashtekar & Schilling, gr-qc/9706069
- Cirelli, Lanzavecchia & Mania, J. Math. Phys. 31 (1990)

---

## ⚠️ Correzione autori

Il file citava "Cirelli, Lanzavecchia & Manià 1990" — correggere in "Cirelli, Manià & Pizzocchero 1990".
→ [[letteratura/cirelliNormalPureStates1983]] è il paper del 1983 con Lanzavecchia.

## Letteratura collegata

- [[letteratura/ashtekarGeometricalFormulationQuantum1997]] — struttura di Kähler su ℙℋ, Prop. 3.1
- [[letteratura/cirelliQuantumMechanicsInfinitedimensional1990]] — Part I: sistema hamiltoniano su ℙℋ ⭐
- [[letteratura/cirelliQuantumMechanicsInfinitedimensional1990a]] — Part II: funzioni kähleriane e uncertainty
- [[letteratura/cirelliNormalPureStates1983]] — 1983: precursore, ℙℋ come varietà di Kähler


---

## Testo LaTeX pronto per la tesi (§3.2)

Nota: la citazione corretta è Cirelli, Manià & Pizzocchero (1990) per la parte I/II; Lanzavecchia compare solo nel precursore del 1983. Uso qui le chiavi corrette del vault.

```latex
\begin{definition}[Kähler manifold]\label{def:kahler}
A \emph{Kähler manifold} is a triple $(M,g,J,\omega)$, with $g$ a Riemannian metric,
$J$ an integrable complex structure ($J^2=-\mathrm{Id}$), and $\omega$ a symplectic
form (Definition~\ref{def:symplectic-manifold}), related by
\[
\omega(u,v) = g(Ju,v), \qquad u,v\in T_pM.
\]
\end{definition}

\begin{proposition}\label{prop:PH-kahler}
Let $\mathcal{H}$ be a Hilbert space and $\mathbb{P}\mathcal{H}$ its projective space
(Definition~\ref{def:projective-hilbert-space}). Decomposing the inner product along
a representative $\psi$ of $[\psi]\in\mathbb{P}\mathcal{H}$,
\[
\langle\psi|\varphi\rangle = g(\psi,\varphi) + i\,\omega(\psi,\varphi), \qquad
g=\mathrm{Re}\langle\cdot|\cdot\rangle,\ \ \omega=\mathrm{Im}\langle\cdot|\cdot\rangle,
\]
and setting $J:\psi\mapsto i\psi$, the triple $(g,J,\omega)$ descends to
$\mathbb{P}\mathcal{H}$ and satisfies Definition~\ref{def:kahler}: $g$ is the
Fubini–Study metric, $\omega$ the Fubini–Study symplectic form, and
$\omega(\psi,\varphi)=g(J\psi,\varphi)$.
\end{proposition}

\begin{remark}
The triple of Proposition~\ref{prop:PH-kahler} is not imposed on $\mathbb{P}\mathcal{H}$:
it is read off directly from the decomposition of the Hilbert space inner product
into real and imaginary part. Kähler geometry is the earned name of an object
already constructed, not an independent postulate.
\end{remark}

\begin{proposition}[Kähler potential]\label{prop:kahler-potential}
On the chart $U_0=\{[\psi]:\psi_0\ne 0\}\subset\mathbb{P}\mathcal{H}$ with affine
coordinates $z_j=\psi_j/\psi_0$,
\[
K(z,\bar z) = \log\Big(1+\sum_j |z_j|^2\Big)
\]
is a Kähler potential for $\omega$: $\omega = i\,\partial\bar\partial K$. In
particular $d\omega=0$ follows from $\partial^2=0$, without invoking the
Newlander–Nirenberg theorem.
\end{proposition}
```

*Fonte: \cite{ashtekarGeometricalFormulationQuantum1997} Prop. 3.1; \cite{cirelliQuantumMechanicsInfinitedimensional1990}; \cite{cirelliQuantumMechanicsInfinitedimensional1990a}.*
