# Poisson Brackets

**Introduced in thesis**: §1.3
**Links**: [[symplectic_geometry]], [[c_star_algebra]], [[cap1]]

---

## Definition

On a symplectic manifold (M, ω), the **Poisson bracket** of f, g ∈ C^∞(M) is:

{f, g} = ω(X_f, X_g)

where X_f, X_g are the Hamiltonian vector fields of f and g.

---

## Properties

| Property | Expression |
|----------|-----------|
| Bilinearity | {αf+βg, h} = α{f,h} + β{g,h} |
| Antisymmetry | {f,g} = −{g,f} |
| Leibniz rule | {fg, h} = f{g,h} + g{f,h} |
| Jacobi identity | {{f,g},h} + {{g,h},f} + {{h,f},g} = 0 |

---

## Jacobi ⟺ dω = 0

This equivalence is the key technical result of §1.3:

Jacobi identity for {·,·} ⟺ dω = 0

*Proof via Cartan formula: L_X = ι_X d + d ι_X.*

The same equivalence guarantees the Jacobi identity for the Poisson bracket on ℙℋ (§3.3), since dω = 0 holds there by construction (§3.2).

---

## (C^∞(M), {·,·}) as Lie algebra

All axioms of §1.1 are satisfied. The Poisson bracket is an instance of the abstract Lie bracket of §1.1.

**The commutator (1/iℏ)[A,B] in B(ℋ) is the non-commutative counterpart** — not by analogy, but because both are representations of the same abstract structure.

---

## Domain constraint

The Poisson bracket is a **first-order differential operator** on M.

- It is defined on C^∞(M) and, restricting, on C^∞_c(M)
- It does **NOT** extend continuously to C_0(M) in the sup-norm
- This is why the Lie-bracket of CM is "structure of C^∞_c(M) ⊂ C_0(M)" — not of C_0(M) itself


---

## Testo LaTeX pronto per la tesi (§1.3)

```latex
\begin{definition}[Poisson bracket]\label{def:poisson-bracket}
Let $(M,\omega)$ be a symplectic manifold (Definition~\ref{def:symplectic-manifold}).
For $f\in C^\infty(M)$ let $X_f$ be its Hamiltonian vector field
(Definition~\ref{def:hamiltonian-vf}). The \emph{Poisson bracket} of
$f,g\in C^\infty(M)$ is
\[
\{f,g\} := \omega(X_f,X_g).
\]
\end{definition}

\begin{proposition}\label{prop:poisson-lie-algebra}
$(C^\infty(M),\{\cdot,\cdot\})$ is bilinear, antisymmetric, and satisfies the
Leibniz rule $\{fg,h\}=f\{g,h\}+g\{f,h\}$. The Jacobi identity
\[
\{\{f,g\},h\}+\{\{g,h\},f\}+\{\{h,f\},g\}=0
\]
holds if and only if $d\omega=0$.
\end{proposition}

\begin{proof}[Proof (sketch)]
By the Cartan formula $\mathcal{L}_X=\iota_X d+d\iota_X$ applied to $X_f,X_g,X_h$
and $\omega$, the cyclic sum in the Jacobi identity reduces to
$d\omega(X_f,X_g,X_h)$.
\end{proof}

\begin{remark}
$(C^\infty(M),\{\cdot,\cdot\})$ is an instance of the abstract Lie algebra of
Definition~\ref{def:lie-algebra}; the commutator $\frac{1}{i\hbar}[A,B]$ on
$B(\mathcal{H})$, introduced in Chapter~\ref{cap:qm-algebraic}, is its
non-commutative counterpart — not by analogy, but as another representation of the
same abstract bracket. By Proposition~\ref{prop:poisson-lie-algebra}, the closedness
$d\omega=0$ established on $\mathbb{P}\mathcal{H}$ (Proposition~\ref{prop:kahler-potential})
guarantees the Jacobi identity for the induced bracket on quantum state space.
\end{remark}

\begin{remark}
As a first-order differential operator, $\{\cdot,\cdot\}$ is defined on
$C^\infty(M)$, restricts to $C_c^\infty(M)$, and does \emph{not} extend
continuously to $C_0(M)$ in the sup norm.
\end{remark}
```
