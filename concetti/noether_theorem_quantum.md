# Quantum Noether Theorem

**Stated in tesi**: §3.4
**Links**: [[noether_theorem_classical]], [[schrodinger_hamiltonian_flow]], [[stone_theorem]], [[capitoli/cap3]]

---

## Contenuto

Applicazione letterale del Noether classico (§1.4) su $(\mathbb{P}\mathcal{H},\omega)$: la conservazione di $\langle\hat\mu^X\rangle$ per simmetrie che commutano con $\hat H$ non è un fatto quantistico indipendente, ma un caso particolare del Noether classico del Cap. 1, una volta stabilita la struttura Hamiltoniana di §3.3.

---

## Testo LaTeX pronto per la tesi (§3.4)

```latex
\begin{theorem}[Quantum Noether]\label{thm:noether-quantum}
Let $U:G\to\mathcal{U}(\mathcal{H})$ be a strongly continuous unitary representation
of a Lie group $G$, with self-adjoint generators $\{\hat\mu^X\}_{X\in\mathfrak g}$
($U(\exp tX)=e^{-it\hat\mu^X/\hbar}$), descending via
Proposition~\ref{prop:stone-descent} to a Hamiltonian $G$-action on
$(\mathbb{P}\mathcal{H},\omega)$ with moment map
$\mu([\psi])^X=\langle\psi|\hat\mu^X|\psi\rangle/\langle\psi|\psi\rangle$. If
$[\hat H,U(g)]=0$ for all $g\in G$, then $\{\mu^X,f_H\}=0$ for all $X\in\mathfrak g$,
i.e.\ $\mu$ is conserved along the flow of Theorem~\ref{thm:schrodinger-hamiltonian}.
\end{theorem}

\begin{remark}
Theorem~\ref{thm:noether-quantum} is Theorem~\ref{thm:noether-classical} applied
verbatim on $(\mathbb{P}\mathcal{H},\omega)$: conservation of $\langle\hat\mu^X\rangle$
under $[\hat H,\hat\mu^X]=0$ is recovered as a special case of the classical Noether
theorem of Chapter~\ref{cap:cm-c-star}, not as an independently postulated quantum
fact.
\end{remark}
```

## Sources

- Cirelli, Manià & Pizzocchero (1990), Parte I — trattazione del sistema Hamiltoniano su $\mathbb{P}\mathcal{H}$.

## Letteratura collegata

- [[letteratura/cirelliQuantumMechanicsInfinitedimensional1990]]
