# Symplectic Group Actions and Noether's Theorem (classical)

**Introdotto in tesi**: §1.4
**Links**: [[symplectic_geometry]], [[poisson_brackets]], [[lie_algebra]], [[noether_theorem_quantum]], [[capitoli/cap1]]

---

## Contenuto

Momento angolare/moment map come conseguenza di un'azione Hamiltoniana di un gruppo di Lie su $(M,\omega)$; il teorema di Noether classico segue in due righe da $\{\mu^X,H\}=0$. Serve da modello diretto per il Noether quantistico di §3.4 — stesso enunciato, trasportato su $\mathbb{P}\mathcal{H}$.

---

## Testo LaTeX pronto per la tesi (§1.4)

```latex
\begin{definition}[Symplectic action and moment map]\label{def:moment-map}
Let $(M,\omega)$ be a symplectic manifold and $G$ a Lie group with Lie algebra
$\mathfrak{g}$ acting on $M$ by symplectomorphisms. The action is \emph{Hamiltonian}
if there exists $\mu:M\to\mathfrak{g}^*$, the \emph{moment map}, such that for every
$X\in\mathfrak{g}$ the vector field $X_M$ generating the action of $\exp(tX)$ is the
Hamiltonian vector field of $\mu^X:=\langle\mu(\cdot),X\rangle$:
\[
\iota_{X_M}\omega = d\mu^X.
\]
\end{definition}

\begin{theorem}[Noether]\label{thm:noether-classical}
If $H\in C^\infty(M)$ is invariant under a Hamiltonian $G$-action with moment map
$\mu$, then $\mu$ is conserved along the flow of $X_H$: $\{\mu^X,H\}=0$ for all
$X\in\mathfrak{g}$.
\end{theorem}

\begin{proof}
$\{\mu^X,H\}=X_H(\mu^X) = -X_{\mu^X}(H) = -X_M(H)=0$, the last equality by
$G$-invariance of $H$.
\end{proof}

\begin{remark}
Global existence of $\mu$ is guaranteed when $M$ is compact
(Remark following Theorem~\ref{thm:darboux}). On $S^2$ (Qubit I,
Example~\ref{ex:qubit-1}), the moment map for the $SU(2)$-action is
$\mu(x)=x\in\mathfrak{su}(2)^*\cong\mathbb{R}^3$, with $\mu^{X_k}=x_k$.
\end{remark}
```

## Sources

- Abraham & Marsden, Foundations of Mechanics.

## Letteratura collegata

- [[letteratura/abrahamFoundationsMechanics2008]]
