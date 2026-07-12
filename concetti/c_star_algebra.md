# C*-Algebra

**Defined in thesis**: §1.5
**Links**: [[cap1]], [[cap2]], [[gelfand_theorem]], [[gns_construction]]

---

## Definition

A **C*-algebra** is a Banach algebra 𝒜 over ℂ equipped with an involution * : 𝒜 → 𝒜 satisfying the **C* condition**:

‖a*a‖ = ‖a‖² for all a ∈ 𝒜

The C* condition is the key axiom — it makes the algebraic and metric structures lock together.

---

## State

A **state** on a C*-algebra 𝒜 is a linear functional ω: 𝒜 → ℂ satisfying:
- **Positivity**: ω(a*a) ≥ 0 for all a
- **Normalisation**: ω(I) = 1 (if 𝒜 is unital)

Expectation value of observable a in state ω: ω(a).

*Same definition for classical (§1.5) and quantum (§2.1). This parallel is structural, not incidental.*

---

## Two realisations in this thesis

| | Classical (Ch. 1) | Quantum (Ch. 2) |
|---|---|---|
| Algebra | C_0(M) | B(ℋ) |
| Commutative? | Yes | No |
| Classification | Gelfand | Gelfand–Naimark |
| Lie-bracket | {f,g} (Poisson) | (1/iℏ)[A,B] |

---

## C^∞_c(M) vs C_0(M) — critical distinction

| Statement | Truth value |
|-----------|------------|
| C^∞_c(M) ⊂ C_0(M) | **FALSE** — C_0 contains only continuous functions |
| C^∞_c(M) dense in C_0(M) | **TRUE** |
| Poisson bracket extends to C_0(M) | **FALSE** — it is a 1st-order differential operator, not sup-norm continuous |

*For M compact: C_0(M) = C(M) and C^∞_c(M) = C^∞(M).*

---

## Sources

- Strocchi (2008): main source for the operational/algebraic approach
- Bratteli & Robinson, Vol. I: full technical development
- Moretti: Gelfand–Naimark theorem

---

## Letteratura collegata

- [[letteratura/strocchiIntroductionMathematicalStructure2005]] — fonte primaria approccio operazionale
- [[letteratura/bratteliOperatorAlgebrasQuantum]] — Vol. I: definizioni, GNS, Gelfand
- [[letteratura/bratteliOperatorAlgebrasQuantum1981]] — Vol. II: algebra di Weyl, Stone–von Neumann
- [[letteratura/rieffelDeformationQuantizationActions1993]] — strict DQ: A_ℏ come C*-algebra per ogni ℏ
- [[letteratura/landsmanFoundationsQuantumTheory2017]] — trattazione moderna e comprensiva


---

## Testo LaTeX pronto per la tesi (§1.5, riusato senza ripetizione in §2.1)

```latex
\begin{definition}[C*-algebra]\label{def:c-star-algebra}
A \emph{C*-algebra} is a Banach algebra $\mathcal{A}$ over $\mathbb{C}$, equipped with an
involution $*:\mathcal{A}\to\mathcal{A}$, $a\mapsto a^*$, satisfying $(ab)^*=b^*a^*$,
$(a+\lambda b)^*=a^*+\bar\lambda b^*$, and the \emph{C*-identity}
\[
\|a^*a\| = \|a\|^2 \qquad \forall a\in\mathcal{A}.
\]
$\mathcal{A}$ is \emph{unital} if it contains an identity $I$ with $\|I\|=1$.
\end{definition}

\begin{remark}
The C*-identity is not an independent metric requirement compatible with an
arbitrarily chosen norm: it forces the norm to be entirely determined by the
algebraic structure, since $\|a\|^2=\|a^*a\|=r(a^*a)$, the spectral radius of $a^*a$.
\end{remark}

\begin{definition}[State]\label{def:state}
A \emph{state} on a unital C*-algebra $\mathcal{A}$ is a linear functional
$\omega:\mathcal{A}\to\mathbb{C}$ such that
\[
\omega(a^*a)\ge 0 \quad \forall a\in\mathcal{A}, \qquad \omega(I)=1.
\]
For $a$ self-adjoint, $\omega(a)$ is the expectation value of the observable $a$ in
the state $\omega$.
\end{definition}

\begin{remark}
Definitions~\ref{def:c-star-algebra} and~\ref{def:state} are stated once, in
\S\ref{cap:cm-c-star}, and are \emph{not} repeated in
Chapter~\ref{cap:qm-algebraic}: the same algebraic notion of state covers both the
commutative case $\mathcal{A}=C_0(M)$ and the non-commutative case
$\mathcal{A}=B(\mathcal{H})$.
\end{remark}

\begin{remark}[$C_c^\infty(M)$ versus $C_0(M)$]
$C_c^\infty(M)\subset C_0(M)$ densely, but the inclusion is not the whole story:
$C_c^\infty(M)$ carries a Lie-algebra structure (Definition~\ref{def:poisson-bracket})
that does \emph{not} extend continuously to $C_0(M)$, since the Poisson bracket is a
first-order differential operator, not sup-norm continuous. If $M$ is compact,
$C_0(M)=C(M)$ and $C_c^\infty(M)=C^\infty(M)$.
\end{remark}
```

*Fonte: \cite{strocchiIntroductionMathematicalStructure2005}, \cite{bratteliOperatorAlgebrasQuantum}.*
