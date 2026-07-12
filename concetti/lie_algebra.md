# Lie Algebra

**Introdotto in tesi**: §1.1 (prerequisito per tutte le parentesi della tesi)
**Links**: [[symplectic_geometry]], [[poisson_brackets]], [[c_star_algebra]], [[capitoli/cap1]]

---

## Contenuto

Definizione astratta di algebra di Lie, presentata prima di simplettica/Poisson perché sia la parentesi di Poisson (Cap. 1) sia il commutatore (Cap. 2) ne sono realizzazioni concrete. È il concetto-cerniera che rende precisa l'affermazione "stessa struttura, due rappresentazioni".

---

## Testo LaTeX pronto per la tesi (§1.1)

```latex
\begin{definition}[Lie algebra]\label{def:lie-algebra}
A \emph{Lie algebra} over $\mathbb{K}\in\{\mathbb{R},\mathbb{C}\}$ is a
$\mathbb{K}$-vector space $\mathfrak{g}$ equipped with a bilinear map
$[\cdot,\cdot]:\mathfrak{g}\times\mathfrak{g}\to\mathfrak{g}$ satisfying
\[
[X,Y] = -[Y,X], \qquad
[[X,Y],Z]+[[Y,Z],X]+[[Z,X],Y]=0
\]
for all $X,Y,Z\in\mathfrak{g}$ (antisymmetry and the Jacobi identity).
\end{definition}

\begin{remark}
Every associative algebra $(\mathcal{A},\cdot)$ carries a canonical Lie algebra
structure via the commutator $[a,b]:=ab-ba$. The Poisson bracket
(Definition~\ref{def:poisson-bracket}) does \emph{not} arise this way from an
associative product on $C^\infty(M)$; the two Lie brackets used throughout the
thesis — Poisson and commutator — are distinguished exactly along the
classical/quantum divide of Chapters~\ref{cap:cm-c-star}–\ref{cap:qm-algebraic}, and
identified as two representations of Definition~\ref{def:lie-algebra} on the same
abstract algebra $\mathfrak{su}(2)$ in the Qubit thread (Examples~\ref{ex:qubit-1},
\ref{ex:qubit-2}).
\end{remark}
```

## Sources

- Abraham & Marsden, standard reference for the algebraic prerequisites.

## Letteratura collegata

- [[letteratura/abrahamFoundationsMechanics2008]]
- [[letteratura/humphreysIntroductionLieAlgebras2010]]