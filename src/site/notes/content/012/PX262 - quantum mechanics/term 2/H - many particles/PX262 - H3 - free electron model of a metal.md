---
{"dg-publish":true,"permalink":"/content/012/px-262-quantum-mechanics/term-2/h-many-particles/px-262-h3-free-electron-model-of-a-metal/","noteIcon":"1","created":"2025-01-09T17:19:33.338+00:00","updated":"2025-01-09T18:20:04.145+00:00"}
---

- loosely bound valence electrons $(\sim 10^{24})$ in a metal are modelled as non-interacting fermions in a potential form a uniform, positively charged background
- the system charge is neutral

- putting a large number of electrons, $N$, in a large box

![PX262 - H3 - free electron model of a metal.png|500](/img/user/pics/PX262%20-%20H3%20-%20free%20electron%20model%20of%20a%20metal.png)

- considering a 1D case
- feeding in $N$ electrons with two per state (spin $\uparrow,\downarrow$) to find the ground state energy:
$$N = 2n_{F}$$
	where, $F$ stands for fermi
- and the wavenumber of the highest occupied state, the fermi wavenumber is:
$$k_{F} = \frac{n_{F}\pi}{L} = \frac{N\pi}{2L} = \frac{\pi}{2}\rho_{e}$$
	where, $\rho_{e}$ is the density, $N/L$
- the energy of the highest occupied state, the fermi energy is:
$$E_{F} = \frac{\hbar^{2}}{2m} \left(\frac{N\pi}{2L}\right)^{2} = \frac{\hbar^{2}\pi^{2}}{8m_{e}} \rho^{2}_{e}$$
- for a large $N$, large $L$, it is useful to impose periodic boundary conditions instead and consider running wave solutions: $\phi(x) = Ae^{ikx}$
$$\phi(x) = \phi(x+L) = \phi(x+2L) = \dots$$
- this means that $e^{ikL} = 1$ and ${} kL = n2\pi {}$ with $n=\pm1, \pm2, \dots$

![PX262 - H3 - free electron model of a metal-1.png|500](/img/user/pics/PX262%20-%20H3%20-%20free%20electron%20model%20of%20a%20metal-1.png)

- the energy levels are given as:
$$E_{n} = \frac{\hbar^{2}}{2m_{e}}k_{n}^{2}$$
- and the states are:
$$\phi_{n}(x) = Ae^{ik_{n}x}$$
- the wavenumbers are separated by $\frac{2\pi}{L}$

#review
$$N = 2 \times 2 n_{F} = 4n_{F}$$
$$\begin{gather}
k_{F} = \frac{N}{4} \frac{2\pi}{L} = \frac{\pi}{2}\rho_{e} \\\\
N = \frac{2L}{\pi}k_F
\end{gather}$$
- the fermi energy:
$$E_{F} = \frac{\hbar^{2}}{2m_{e}} \left(\frac{N\pi}{2L}\right)^{2} = \frac{ \hbar^{2}\pi^{2}}{8m_{e}}\rho_{e}^{2}$$
- the number of states with energies less than a given value, $E_{n} \le E_{F}:$
$$N(E_{n}) = \frac{2L}{\pi}k_{n} = \frac{2L}{\pi}\left(\frac{2m_{e}}{\hbar^{2}}\right)^{1/2} E_{n}^{1/2}$$
- in a large, effectively infinite system, $L\to\infty$, there is a continuum of states

![PX262 - H3 - free electron model of a metal-2.png|500](/img/user/pics/PX262%20-%20H3%20-%20free%20electron%20model%20of%20a%20metal-2.png)

- **note:** the states are distributed with respect to energy:
$$N(E+\Delta E) \simeq N(E) + \frac{dN}{dt}\Delta E = N(E) + n(E) \Delta E$$
	where, $n(E)$ is the **density of states (DOS)**

[[content/012/PX284 - statistical mechanics/H - gases/PX284 - H1 - density of states (DOS)\|PX284 - H1 - density of states (DOS)]]

- sometimes, $g(E)$ is used to denote the DOS
$$n(E) = \frac{L}{\pi}\left(\frac{2m_{e}}{\hbar^{2}}\right)^{1/2}\sqrt{E_F}$$
- this can be used to calculate properties:
- the total energy:
$$\begin{align*}
E_{TOT} &= \int_{0}^{E_{F}} E\,n(E) \,dE \; \left(=\sum\limits_{n+1}^{N/2} E_{n+2} \right) \\
&= \frac{L}{\pi}\left(\frac{2m_{e}}{\hbar^{2}}\right)^{1/2} \int_{0}^{E_{F}} \frac{E}{\sqrt{E}}\,dE\\
&= \frac{L}{\pi} \left(\frac{2m_{e}}{\hbar}\right)^{1/2} \frac{2}{3}E_{F}^{3/2} 
\end{align*}$$
- the average energy per electron:
$$\frac{E_{TOT}}{N} = \frac{E_{F}}{3}$$
