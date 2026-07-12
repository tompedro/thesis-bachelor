# Bridge to the Geometry of States

**Introdotto in tesi**: §2.4 (cerniera Cap. 2 → Cap. 3)
**Links**: [[gns_construction]], [[projective_hilbert_space]], [[capitoli/cap2]], [[capitoli/cap3]]

---

## Contenuto

§2.4 non introduce definizioni nuove: impacchetta l'output del Cap. 2 — la coppia $(\mathcal{A},\omega)$ e lo spazio di Hilbert GNS $\mathcal{H}_\omega$ — come input del Cap. 3. L'unico fatto tecnico necessario è che gli stati puri sono etichettati fedelmente da $\mathbb{P}\mathcal{H}$, non da $\mathcal{H}$: questa è la motivazione operazionale (non ancora geometrica) per passare a $\mathbb{P}\mathcal{H}$.

---

## Testo LaTeX pronto per la tesi (§2.4)

```latex
\begin{proposition}\label{prop:pure-states-PH}
Let $\mathcal{H}$ be the GNS Hilbert space of a pure state $\omega$ on
$B(\mathcal{H})$ (i.e.\ $\omega(a)=\langle\psi|a|\psi\rangle$ for a unit vector
$\psi$). Two unit vectors $\psi,\psi'\in\mathcal{H}$ induce the same state,
$\omega_\psi=\omega_{\psi'}$, if and only if $\psi'=\lambda\psi$ for some
$\lambda\in U(1)$.
\end{proposition}

\begin{remark}
Proposition~\ref{prop:pure-states-PH} identifies the space of pure states with
$\mathbb{P}\mathcal{H}$ (Definition~\ref{def:projective-hilbert-space}), not
$\mathcal{H}$: this is the operational justification, prior to any geometric
structure, for studying $\mathbb{P}\mathcal{H}$ in Chapter~\ref{cap:kahler}.
\end{remark}
```

## Sources

- Segue direttamente da GNS (§2.2); nessuna fonte aggiuntiva necessaria.
