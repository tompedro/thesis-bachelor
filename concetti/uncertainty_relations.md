# Uncertainty Relations as a Kähler Corollary

**Stated in tesi**: §3.5
**Links**: [[kahler_geometry]], [[schrodinger_hamiltonian_flow]], [[capitoli/cap3]]

---

## Contenuto

Chiusura dell'argomento del Cap. 3: le relazioni di indeterminazione non sono un fatto operatoriale indipendente, ma un corollario della compatibilità Kähleriana $\omega(u,v)=g(Ju,v)$ già stabilita in §3.2.

## ⚠️ Da verificare

Il blocco LaTeX sotto è una *bozza* della derivazione (Cauchy–Schwarz su $T_{[\psi]}\mathbb{P}\mathcal{H}$ rispetto a $g$, isolando la parte antisimmetrica via $J$). Controllare i coefficienti numerici e il segno contro Ashtekar–Schilling o Cirelli–Manià–Pizzocchero prima di inserirlo definitivamente: non l'ho verificato con lo stesso rigore delle altre voci di questo file.

---

## Testo LaTeX pronto per la tesi (§3.5, da verificare)

```latex
\begin{proposition}[Uncertainty relations as a Kähler corollary]\label{prop:uncertainty}
For self-adjoint $\hat A,\hat B$ on $\mathcal{H}$ and $[\psi]\in\mathbb{P}\mathcal{H}$,
let $X_{f_A},X_{f_B}$ be the Hamiltonian vector fields at $[\psi]$ of
$f_A,f_B$ (as in Theorem~\ref{thm:schrodinger-hamiltonian}). Then
\[
(\Delta A)^2_\psi\,(\Delta B)^2_\psi \;\ge\;
g(X_{f_A},X_{f_B})^2 + \tfrac14\,\{f_A,f_B\}([\psi])^2,
\]
where $g$ is the Fubini–Study metric of Proposition~\ref{prop:PH-kahler} and
$(\Delta A)^2_\psi := g(X_{f_A},X_{f_A})$.
\end{proposition}

\begin{proof}[Proof (sketch)]
Apply Cauchy–Schwarz to $X_{f_A},X_{f_B}\in T_{[\psi]}\mathbb{P}\mathcal{H}$ with
respect to $g$, then use the Kähler compatibility
$\omega(X_{f_A},X_{f_B})=g(JX_{f_A},X_{f_B})$ together with
$\{f_A,f_B\}=\omega(X_{f_A},X_{f_B})$ (Definition~\ref{def:poisson-bracket}) to
isolate the antisymmetric part.
\end{proof}

\begin{remark}
Setting $g(X_{f_A},X_{f_B})=0$ recovers the Robertson–Schrödinger relation
$(\Delta A)_\psi(\Delta B)_\psi \ge \tfrac12|\langle[\hat A,\hat B]\rangle_\psi|$.
Proposition~\ref{prop:uncertainty} exhibits it as a corollary of the Kähler geometry
of $\mathbb{P}\mathcal{H}$, closing Chapter~\ref{cap:kahler}'s argument without
further operator-theoretic input.
\end{remark}
```

## Sources

- Cirelli, Manià & Pizzocchero (1990), Parte II — funzioni kähleriane e uncertainty.
- Ashtekar & Schilling, gr-qc/9706069.

## Letteratura collegata

- [[letteratura/cirelliQuantumMechanicsInfinitedimensional1990a]]
- [[letteratura/ashtekarGeometricalFormulationQuantum1997]]
