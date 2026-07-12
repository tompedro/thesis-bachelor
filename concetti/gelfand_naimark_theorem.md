# Gelfand–Naimark Theorem

**Stated in tesi**: §2.2
**Links**: [[c_star_algebra]], [[gelfand_theorem]], [[gns_construction]], [[capitoli/cap2]]

---

## Contenuto

Controparte non-commutativa del teorema di Gelfand: giustifica $B(\mathcal{H})$ come sede naturale delle osservabili quantistiche. La dimostrazione standard è una applicazione diretta di GNS a una famiglia separante di stati — va quindi enunciato *dopo* GNS in §2.2, non prima.

---

## Testo LaTeX pronto per la tesi (§2.2)

```latex
\begin{theorem}[Gelfand–Naimark]\label{thm:gelfand-naimark}
Every C*-algebra $\mathcal{A}$ admits a faithful $*$-representation
$\pi:\mathcal{A}\to B(\mathcal{H})$ on some Hilbert space $\mathcal{H}$; $\pi$ is
automatically isometric.
\end{theorem}

\begin{proof}[Proof (sketch)]
Let $\{\omega_i\}_{i\in I}$ be a separating family of states on $\mathcal{A}$ (e.g.\
all states), and $(\mathcal{H}_{\omega_i},\pi_{\omega_i},\Omega_{\omega_i})$ the
corresponding GNS triples (Theorem~\ref{thm:gns}). Set
$\mathcal{H}=\bigoplus_i \mathcal{H}_{\omega_i}$, $\pi=\bigoplus_i\pi_{\omega_i}$.
Faithfulness of $\pi$ follows from the separating property of $\{\omega_i\}$; every
injective $*$-homomorphism between C*-algebras is automatically isometric.
\end{proof}

\begin{remark}
Theorem~\ref{thm:gelfand-naimark} is the non-commutative counterpart of
Theorem~\ref{thm:gelfand}, and justifies working with $B(\mathcal{H})$ — rather than
an abstractly given C*-algebra — as the algebra of quantum observables in
Chapters~\ref{cap:qm-algebraic}–\ref{cap:kahler}.
\end{remark}
```

## Sources

- Bratteli & Robinson, Vol. I.

## Letteratura collegata

- [[letteratura/bratteliOperatorAlgebrasQuantum]]
