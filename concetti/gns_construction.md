# GNS Construction

**Stated in thesis**: §2.2
**Links**: [[c_star_algebra]], [[cap2]]

---

## Setup

Given a C*-algebra 𝒜 and a state ω: 𝒜 → ℂ.

## Construction

1. **Inner product**: ⟨a,b⟩_ω = ω(a*b)
2. **Gelfand ideal**: 𝒥_ω = {a ∈ 𝒜 : ω(a*a) = 0} — the "null vectors"
3. **Pre-Hilbert space**: 𝒜/𝒥_ω with inner product ⟨[a],[b]⟩ = ω(a*b)
4. **GNS space**: ℋ_ω = completion of 𝒜/𝒥_ω
5. **Representation**: π_ω(a)[b] = [ab], extended to ℋ_ω
6. **Cyclic vector**: Ω_ω = [I] with ω(a) = ⟨Ω_ω, π_ω(a)Ω_ω⟩

## GNS Theorem

Every state determines a unique (up to unitary equivalence) triple (ℋ_ω, π_ω, Ω_ω).

**Hilbert space emerges from algebraic structure** — it is not postulated.

## Role in the thesis

The GNS construction is the bridge between:
- The **algebraic** approach (Ch. 2: 𝒜, states, no ℋ assumed)
- The **geometric** approach (Ch. 3: ℙℋ, symplectic form, Hamiltonian flow)

The Hilbert space ℋ from GNS is the one that is projectivised in Ch. 3.

## Sources

- Reed & Simon, Vol. I, §II.4 and Thm VIII.7
- Moretti, Ch. 8
- Strocchi (2008)


---

## Testo LaTeX pronto per la tesi (§2.2)

```latex
Given a C*-algebra $\mathcal{A}$ and a state $\omega$ on $\mathcal{A}$
(Definition~\ref{def:state}), define the sesquilinear form
$\langle a,b\rangle_\omega := \omega(a^*b)$ on $\mathcal{A}$ and the \emph{Gelfand
ideal}
\[
\mathcal{J}_\omega := \{a\in\mathcal{A} : \omega(a^*a)=0\}.
\]
Positivity of $\omega$ makes $\langle\cdot,\cdot\rangle_\omega$ a well-defined inner
product on the quotient $\mathcal{A}/\mathcal{J}_\omega$; let $\mathcal{H}_\omega$ be
its completion, $[a]\in\mathcal{H}_\omega$ the class of $a$, and
\[
\pi_\omega(a)[b] := [ab], \qquad \Omega_\omega := [I].
\]

\begin{theorem}[GNS]\label{thm:gns}
$\pi_\omega$ extends to a $*$-representation of $\mathcal{A}$ on $\mathcal{H}_\omega$,
$\Omega_\omega$ is a unit cyclic vector for $\pi_\omega$ (i.e.\
$\overline{\pi_\omega(\mathcal{A})\Omega_\omega}=\mathcal{H}_\omega$), and
\[
\omega(a) = \langle \Omega_\omega,\, \pi_\omega(a)\,\Omega_\omega\rangle
\qquad \forall a\in\mathcal{A}.
\]
The triple $(\mathcal{H}_\omega,\pi_\omega,\Omega_\omega)$ is unique up to unitary
equivalence among cyclic representations reproducing $\omega$ in this way.
\end{theorem}

\begin{remark}
Theorem~\ref{thm:gns} is the precise sense in which the Hilbert space of quantum
mechanics is \emph{derived}, not postulated: given only the algebra of observables
$\mathcal{A}$ and a state $\omega$, the pair $(\mathcal{H}_\omega,\pi_\omega)$ is
produced by the construction. The projective space $\mathbb{P}\mathcal{H}_\omega$
studied in Chapter~\ref{cap:kahler} is built on the Hilbert space obtained here.
\end{remark}
```

*Fonte: \cite{reedMethodsModernMathematical2003} §II.4, Thm. VIII.7; \cite{morettiSpectralTheoryQuantum} Cap. 8; \cite{strocchiIntroductionMathematicalStructure2005}.*
