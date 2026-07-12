# Wintner–Wielandt Theorem

**Stated in thesis**: §2.3
**Links**: [[cap2]], [[c_star_algebra]]

---

## Statement

In any unital Banach algebra, there exist no elements A, B such that AB − BA = I.

---

## Proof

By induction on n:

AB^n − B^n A = nB^{n−1}

Taking operator norms:

n‖B‖^{n−1} = ‖AB^n − B^n A‖ ≤ 2‖A‖·‖B‖^n

Dividing by ‖B‖^{n−1} (assuming B ≠ 0):

n ≤ 2‖A‖·‖B‖   for all n ∈ ℕ

**Contradiction.** ∎

---

## Scope

- Valid in **any** unital Banach algebra
- No trace argument required
- No dimension restriction (holds in infinite-dimensional algebras)
- The proof by induction is the correct form — older statements using the trace are wrong in infinite dimensions

---

## Consequence for QM

The canonical commutation relation [q,p] = iℏI cannot be realised by bounded operators in any unital Banach algebra. This forces the passage to unbounded operators (via Weyl algebra — see §2.3).

---

## Sources

- Wintner, Phys. Rev. 71 (1947)
- Strocchi (2008)


---

## Testo LaTeX pronto per la tesi (§2.3)

```latex
\begin{theorem}[Wintner–Wielandt]\label{thm:wintner}
In a unital Banach algebra $\mathcal{A}$, there exist no $A,B\in\mathcal{A}$ with
$AB-BA=I$.
\end{theorem}

\begin{proof}
By induction, $AB^n-B^nA=nB^{n-1}$ for all $n\ge1$. Taking norms,
$n\|B\|^{n-1}=\|AB^n-B^nA\|\le 2\|A\|\,\|B\|^n$, hence $n\le 2\|A\|\,\|B\|$ for every
$n\in\mathbb{N}$ (assuming $B\ne0$) — a contradiction.
\end{proof}

\begin{remark}
Theorem~\ref{thm:wintner} holds in \emph{any} unital Banach algebra, with no
dimension restriction and no trace argument (invalid in infinite dimensions). It
rules out a bounded-operator realisation of the canonical commutation relation
$[\hat q,\hat p]=i\hbar I$, forcing the passage to the unbounded generators of the
Weyl algebra (Definition~\ref{def:weyl-algebra}).
\end{remark}
```

*Fonte: Wintner, Phys. Rev. 71 (1947); \cite{strocchiIntroductionMathematicalStructure2005}.*
