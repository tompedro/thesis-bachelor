# Gelfand's Theorem

**Stated in thesis**: §1.5
**Used in thesis**: Ch. 1 conclusion
**Links**: [[c_star_algebra]], [[cap1]]

---

## Statement

Every commutative C*-algebra is isometrically *-isomorphic to C_0(X) for some locally compact Hausdorff space X.

*For unital algebras / compact X: isomorphic to C(X).*

---

## Role in the thesis

This theorem is the logical endpoint of Chapter 1:

Classical mechanics → (via Poisson structure and Gelfand) → commutative C*-algebra

**Conclusion**: CM *is* the theory of commutative C*-algebras. This is not a reformulation — it is a recognition.

---

## Counterpart

The quantum counterpart is **Gelfand–Naimark**: every (abstract) C*-algebra embeds isometrically into B(ℋ) for some Hilbert space ℋ. This justifies the use of Hilbert spaces as the natural support for C*-algebras.

---

## Sources

- Strocchi (2008)
- Bratteli & Robinson, Vol. I, Thm. 2.1.10

---

## Letteratura collegata

- [[letteratura/strocchiIntroductionMathematicalStructure2005]] — fonte primaria
- [[letteratura/bratteliOperatorAlgebrasQuantum]] — Thm 2.1.10: dimostrazione completa
- [[letteratura/landsmanFoundationsQuantumTheory2017]] — trattazione moderna


---

## Testo LaTeX pronto per la tesi (§1.5, conclusione del Cap. 1)

```latex
\begin{theorem}[Gelfand]\label{thm:gelfand}
Every commutative C*-algebra $\mathcal{A}$ is isometrically $*$-isomorphic to
$C_0(X)$, where $X=\Delta(\mathcal{A})$ is the space of characters of $\mathcal{A}$
(the Gelfand spectrum), with the weak-$*$ topology, locally compact Hausdorff. If
$\mathcal{A}$ is unital, $X$ is compact and $\mathcal{A}\cong C(X)$.
\end{theorem}

\begin{remark}
Together with \S\ref{cap:cm-c-star}, Theorem~\ref{thm:gelfand} closes the argument
of Chapter~\ref{cap:cm-c-star}: classical mechanics, encoded as the commutative Lie
algebra $(C_c^\infty(M),\{\cdot,\cdot\})$ densely embedded in the C*-algebra
$C_0(M)$, \emph{is} the theory of commutative C*-algebras. No further postulate is
needed to justify the appearance of the manifold $M$: it is recovered as the
spectrum of the algebra of observables.
\end{remark}

\begin{remark}
The non-commutative counterpart of Theorem~\ref{thm:gelfand} is the
Gelfand–Naimark theorem, stated and proved in \S\ref{cap:qm-algebraic} once the GNS
construction is available (Theorem~\ref{thm:gelfand-naimark}).
\end{remark}
```

*Fonte: \cite{strocchiIntroductionMathematicalStructure2005}, \cite{bratteliOperatorAlgebrasQuantum} Thm. 2.1.10.*
