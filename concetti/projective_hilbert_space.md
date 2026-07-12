# Projective Hilbert Space

**Introdotto in tesi**: §3.1
**Links**: [[geometry_of_states_bridge]], [[kahler_geometry]], [[capitoli/cap3]]

---

## Contenuto

Definizione dello spazio delle fasi quantistico $\mathbb{P}\mathcal{H}$, con distinzione esplicita caso finito/infinito-dimensionale (rilevante per tutte le flag di compattezza disseminate nel Cap. 3).

---

## Testo LaTeX pronto per la tesi (§3.1)

```latex
\begin{definition}[Projective Hilbert space]\label{def:projective-hilbert-space}
Let $\mathcal{H}$ be a complex Hilbert space. On $\mathcal{H}\setminus\{0\}$ define
$\psi\sim\varphi \iff \varphi=\lambda\psi$ for some $\lambda\in\mathbb{C}\setminus\{0\}$.
The \emph{projective Hilbert space} is $\mathbb{P}\mathcal{H} :=
(\mathcal{H}\setminus\{0\})/\sim$, with $[\psi]$ the class of $\psi$. Equivalently,
$\mathbb{P}\mathcal{H}$ is the space of unit rays $\{\psi\in\mathcal{H}:\|\psi\|=1\}/U(1)$.
\end{definition}

\begin{remark}
If $\dim\mathcal{H}=n<\infty$, $\mathbb{P}\mathcal{H}\cong\mathbb{CP}^{n-1}$ is a
compact complex manifold of real dimension $2(n-1)$. If $\dim\mathcal{H}=\infty$,
$\mathbb{P}\mathcal{H}$ is a Hilbert manifold modelled on $\mathcal{H}$ itself, and
the compactness-dependent statements flagged in this chapter (global Darboux
coordinates, completeness of Hamiltonian flows, cf.\ Theorem~\ref{thm:darboux})
require separate justification.
\end{remark}

\begin{remark}
$[\psi]$, not $\psi$, is the physically meaningful object
(Proposition~\ref{prop:pure-states-PH}); every state-dependent expression in this
chapter is written as a function of $[\psi]$, e.g.\
$f_H([\psi])=\langle\psi|\hat H|\psi\rangle/\langle\psi|\psi\rangle$.
\end{remark}
```

## Sources

- Ashtekar & Schilling, gr-qc/9706069.

## Letteratura collegata

- [[letteratura/ashtekarGeometricalFormulationQuantum1997]]
