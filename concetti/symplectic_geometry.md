# Symplectic Geometry

**Introduced in thesis**: §1.2
**Reappears in**: §1.3, §1.4, §3.2, §3.3
**Links**: [[poisson_brackets]], [[kahler_geometry]], [[cap1]], [[cap3]]

---

## Symplectic manifold

A **symplectic manifold** is a pair (M, ω) where:
- M is a smooth manifold (even-dimensional)
- ω is a closed (dω = 0) and non-degenerate 2-form

**Non-degeneracy** of ω: for every p ∈ M and v ∈ T_p M, if ω(v,w) = 0 for all w ∈ T_p M, then v = 0.

---

## Musical isomorphisms

ω induces isomorphisms:
- ♭: TM → T*M, v ↦ ι_v ω
- ♯: T*M → TM, inverse of ♭

**Hamiltonian vector field** of f ∈ C^∞(M): unique X_f such that ι_{X_f} ω = df.

---

## Darboux theorem

Locally, every symplectic manifold has coordinates (qⁱ, pᵢ) with ω = Σ dqⁱ ∧ dpᵢ.

**Global Darboux coordinates do NOT exist** on compact manifolds (e.g., S²).

---

## Compactness flags

Results in this thesis that require M compact:
- Completeness of Hamiltonian flow (automatic for compact M; requires growth conditions otherwise)
- Global existence of moment map (automatic for compact M)

Non-compact M: all local results (Darboux, local Hamiltonian fields) hold; global statements require additional hypotheses.

---

## Sources

- Abraham & Marsden, *Foundations of Mechanics*, Ch. 2
- Cannas da Silva, *Lectures on Symplectic Geometry*


---

## Testo LaTeX pronto per la tesi (§1.2, riappare in §1.3, §1.4, §3.2, §3.3)

```latex
\begin{definition}[Symplectic manifold]\label{def:symplectic-manifold}
A \emph{symplectic manifold} is a pair $(M,\omega)$, with $M$ a smooth
(even-dimensional) manifold and $\omega\in\Omega^2(M)$ a closed ($d\omega=0$),
non-degenerate 2-form: for $p\in M$, $v\in T_pM$, if $\omega(v,w)=0$ for all
$w\in T_pM$ then $v=0$.
\end{definition}

\begin{definition}[Hamiltonian vector field]\label{def:hamiltonian-vf}
Non-degeneracy of $\omega$ induces the isomorphism $\flat:TM\to T^*M$,
$v\mapsto\iota_v\omega$. For $f\in C^\infty(M)$, its \emph{Hamiltonian vector field}
$X_f$ is the unique vector field with $\iota_{X_f}\omega=df$.
\end{definition}

\begin{theorem}[Darboux]\label{thm:darboux}
Every symplectic manifold admits, locally around each point, coordinates $(q^i,p_i)$
such that $\omega=\sum_i dq^i\wedge dp_i$.
\end{theorem}

\begin{remark}
Global Darboux coordinates need not exist on compact $M$ (e.g.\ $M=S^2$).
Completeness of Hamiltonian flows and global existence of the moment map
(Definition~\ref{def:moment-map}) are guaranteed automatically when $M$ is compact;
for non-compact $M$ these require additional hypotheses, while local statements
(Darboux, local Hamiltonian vector fields) always hold.
\end{remark}
```

*Fonte: \cite{abrahamFoundationsMechanics2008} Cap. 2.*
