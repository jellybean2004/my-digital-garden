---
{"dg-publish":true,"permalink":"/content/012/px-280-b-environmental-physics/b-light-and-matter/px-280-b4-einstein-coefficient/","noteIcon":"1","created":"2025-01-13T12:21:26.780+00:00","updated":"2025-01-13T13:52:10.357+00:00"}
---

- see [section 2.2.1] of reference textbook for derivation

- considering a system with discrete energy levels, $E_n$
- at $t=0$, the system is in the ground state $(n=1)$, and it starts to interact with light of frequency $\omega$
- therefore, the probability of the system being in the excited state, $k$, at time, $t$, is:
$$P_{k}(t) \propto \bigg| \langle{\psi_{k} | \hat\mu | \psi_{1}\rangle}\bigg|^{2} = \bigg| \int \psi_{k}  \mu \psi_{1}\,dt \bigg|^{2}$$
	where, $\mu_{k_{1}}$ is the transition dipole moment

- the transmission probability:
$$\boxed{\frac{dP_{k}(t)}{dt} = B_{1k}\cdot W(\omega)} \tag{5}$$
	where, $B_{1k}$ is the einstein coefficient
$$\boxed{B_{1k} = \frac{\pi}{3\varepsilon_{0}\hbar^{2}} \cdot |\mu_{k_{1}}|^{2} } \tag{6}$$
- considering a two-state system, with energy levels, $E_{1}$ and $E_{2}$, with the populations of $N_{1}$ and $N_{2}$, respectively
- the transition rates are:
	- spontaneous emission: $A_{21}$
	- absorption: $B_{12}\, W(\omega)$
	- stimulated emission: $B_{21}\, W)(omega)$

- therefore, the rate of change of the population in $E_1:$
$$\frac{dN_{1}}{dt} = - B_{12}W(\omega) N_{1} + B_{21}W(\omega)N_{2} + A_{21}N_{2}$$
- **note:** equation $(5)$ is applied to both absorption and simulated emission

- assuming a steady state $\implies dN_{1}/dt =0$
$$\begin{gather}
\implies A_{21}N_{1} = B_{12}W(\omega) N_{1} - B_{21}W(\omega)N_{2} \\\\
W(\omega) = \frac{A_{21}N_{2}}{B_{12}N_{1}-B_{21}N_{2}}
\end{gather}$$
- from equation $(3):$
$$W(\omega) = \frac{\hbar\omega^{3}}{\pi^{2}c^{3}}  \frac{1}{e^{E-k_{B}T}-1}$$

- using the [[content/012/PX284 - statistical mechanics/C - entropy and temperature/PX284 - C3 - boltzmann distribution\|boltzmann distribution]] to find the probability of the system being in a state with energy, $E_i:$
$$\begin{gather}
N_{1} \propto \exp(-E_{1}/k_{B}T) \\
N_{2} \propto \exp(-E_{2}/k_{B}T) \\\\
\therefore \frac{N_{2}}{N_{1}}= \exp(-\hbar\omega/k_B T)
\end{gather}$$
	where, $E_2-E_1=\hbar\omega$
$$W(\omega) = \frac{A_{21}}{B_{12}\cfrac{N_{1}}{N_{2}}-B_{21}} = \frac{\hbar\omega^{3}}{\pi^{2}c^{3}} \left( \frac{1}{\exp(\frac{\hbar\omega}{k_{B}T})-1} \right)$$
$$\therefore B_{12}= B_{21}$$
$$A_{21}= \frac{\hbar\omega^{3}}{\pi^{2}c^{3}}B_{12} =  \frac{\hbar\omega^{3}}{\pi^{2}c^{3}} |\mu_{21}|^{2}$$
$$\boxed{A_{21} = \frac{\omega^{3}}{3\pi\hbar\varepsilon_{0}c^3}|\mu_{21}|^{2}}$$
- $|\mu_{21}|^{2}$ controls the rates of all three radiative processes
