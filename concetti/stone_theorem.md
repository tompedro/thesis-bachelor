# Stone's Theorem

**Stated in thesis**: §2.3 *(marked for reuse)*
**Reused in thesis**: §3.3 (descent to ℙℋ)
**Links**: [[cap2]], [[cap3]]

---

## Statement

Let {U(t)}_{t∈ℝ} be a strongly continuous one-parameter unitary group on a Hilbert space ℋ. Then there exists a unique self-adjoint operator H on ℋ such that:

U(t) = e^{-iHt/ℏ}

Conversely, every self-adjoint operator generates such a group.

---

## Where it acts

**Stone acts on ℋ, not on ℙℋ.**

This is the most important constraint in the thesis regarding Stone's theorem.

---

## Descent to ℙℋ (Ashtekar–Schilling Prop. 3.1)

Given self-adjoint Ĥ on ℋ:

1. Stone produces U(t) = e^{-iĤt/ℏ} on ℋ
2. U(t) is linear: U(t)(λψ) = λU(t)ψ
3. U(t) commutes with scalar multiplication
4. Therefore U(t) **descends** to a well-defined flow on ℙℋ:
   Φ_t : [ψ] ↦ [e^{-iĤt/ℏ} ψ]
5. This descended flow coincides with the Hamiltonian flow of X_{f_H} with respect to ω on ℙℋ

**Source**: Ashtekar & Schilling, Prop. 3.1.

---

## Convention

In §2.3, check whether ℏ = 1 is used — if so, **declare this explicitly** [Issue S3].

---

## Prerequisite

Self-adjointness (not just symmetry) is required. The distinction between symmetric and self-adjoint unbounded operators is stated in the spectral theory prerequisite of §2.3.

---

## Sources

- Reed & Simon, Vol. I, Thm VIII.7 (Stone's theorem)
- Ashtekar & Schilling, gr-qc/9706069, Prop. 3.1 (descent to ℙℋ)

---

## Letteratura collegata

- [[letteratura/reedMethodsModernMathematical2003]] — Thm VIII.7: enunciato e dimostrazione
- [[letteratura/ashtekarGeometricalFormulationQuantum1997]] — Prop. 3.1: discesa a ℙℋ ⭐
- [[letteratura/hallQuantumTheoryMathematicians2013]] — trattazione accessibile alternativa
- [[letteratura/morettiSpectralTheoryQuantum]] — teoria spettrale per operatori non limitati


---

## Testo LaTeX pronto per la tesi (§2.3, riusato in §3.3)

```latex
\begin{theorem}[Stone]\label{thm:stone}
Let $\{U(t)\}_{t\in\mathbb{R}}$ be a strongly continuous one-parameter unitary group
on a Hilbert space $\mathcal{H}$. Then there exists a unique self-adjoint operator
$H$ on $\mathcal{H}$, possibly unbounded, such that $U(t)=e^{-iHt/\hbar}$. Conversely,
every self-adjoint $H$ generates such a group.
\end{theorem}

\begin{remark}
Stone's theorem acts on $\mathcal{H}$, not on $\mathbb{P}\mathcal{H}$. [Declare here
whether the convention $\hbar=1$ is adopted from this point on.]
\end{remark}

\begin{proposition}[Descent to $\mathbb{P}\mathcal{H}$]\label{prop:stone-descent}
Let $\hat H$ be self-adjoint on $\mathcal{H}$ and $U(t)=e^{-i\hat Ht/\hbar}$ its
Stone flow. Since $U(t)$ is linear, it commutes with scalar multiplication and
descends to a well-defined flow
\[
\Phi_t:\mathbb{P}\mathcal{H}\to\mathbb{P}\mathcal{H}, \qquad
\Phi_t([\psi]) = [e^{-i\hat Ht/\hbar}\psi].
\]
$\Phi_t$ coincides with the Hamiltonian flow of $f_H([\psi])=\langle\psi|\hat
H|\psi\rangle/\langle\psi|\psi\rangle$ with respect to the symplectic form $\omega$
of Proposition~\ref{prop:PH-kahler}.
\end{proposition}

\begin{remark}
Self-adjointness of $\hat H$, not merely symmetry, is required for
Theorem~\ref{thm:stone}.
\end{remark}
```

*Fonte: \cite{reedMethodsModernMathematical2003} Thm. VIII.7; \cite{ashtekarGeometricalFormulationQuantum1997} Prop. 3.1.*
