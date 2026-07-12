# Strocchi's Operational Approach

**Introdotto in tesi**: §2.1 (apertura del Cap. 2)
**Links**: [[c_star_algebra]], [[gns_construction]], [[capitoli/cap2]]

---

## Contenuto

Non è un singolo enunciato ma l'impostazione metodologica di apertura del Cap. 2: osservabili e stati come nozioni primitive operazionali, da cui la struttura di C*-algebra è *derivata* (assiomi di Segal), non postulata. Nessuno spazio di Hilbert è assunto a questo stadio — compare solo dopo, via GNS.

---

## Testo LaTeX pronto per la tesi (§2.1)

```latex
Following \cite{strocchiIntroductionMathematicalStructure2005}, we take as primitive
the notions of \emph{observable} and \emph{state}: an observable is identified
operationally with an equivalence class of measuring procedures, a state with a
preparation procedure. Each state $\omega$ assigns to every observable $a$ its
expectation value $\omega(a)\in\mathbb{R}$, linearly on convex combinations of
preparations and positively on squares. This operational data equips the set of
observables with the structure of an ordered normed real vector space; its
complexification, completed in the induced norm, is postulated to satisfy the
C*-identity of Definition~\ref{def:c-star-algebra} (Segal's axioms). The C*-algebra
of Chapter~\ref{cap:cm-c-star} is thereby recovered as a \emph{consequence} of
operationally motivated axioms on observables and states, not as an independent
starting point.

\begin{remark}
No Hilbert space is assumed at this stage. $\mathcal{H}$ appears only downstream, via
the GNS construction applied to a chosen state $\omega$ (Theorem~\ref{thm:gns}).
\end{remark}
```

## Sources

- Strocchi (2008), Ch. 1–2.
- Haag, Local Quantum Physics, for the wider operational/algebraic tradition.

## Letteratura collegata

- [[letteratura/strocchiIntroductionMathematicalStructure2005]]
- [[letteratura/haagLocalQuantumPhysics1996]]
