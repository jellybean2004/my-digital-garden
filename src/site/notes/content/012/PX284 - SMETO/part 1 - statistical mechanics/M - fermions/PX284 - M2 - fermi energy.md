---
{"dg-publish":true,"permalink":"/content/012/px-284-smeto/part-1-statistical-mechanics/m-fermions/px-284-m2-fermi-energy/","noteIcon":"1","created":"2025-01-30T15:21:37.069+00:00","updated":"2025-01-30T15:53:08.880+00:00"}
---

- putting $N$ electrons into a metal one by one
- the energy levels fill up one by one because of [[content/012/PX284 - SMETO/part 1 - statistical mechanics/L - exchange symmetry/PX284 - L2 - pauli exclusion principle\|pauli exclusion principle]]
- the highest energy reached is called the **fermi energy**, $E_{F}$
- this is seen from $F_{FD}(E)$ as $R\to0$
- #fig 
$$E_{F} \equiv \mu(T=0)$$
- to evaluate $E_F:$ 
$$N = \int_{0}^{\infty} g(E)\, f_{FD}(E)\,dE = \int_{0}^{E_{F}} g(E)\,dE = \frac{V}{2\pi^{2}} \left(\frac{2m}{\hbar}\right)^{3/2}\frac{E_{F}^{3/2}}{3/2}$$
$$E_{F}= \frac{\hbar^{2}}{2m} (3\pi^{2}n)^{2/3}$$
	where, $n = N/V$ is the carrier density

- alternatively:
$$E_{F}= \frac{\hbar^{2}k_{F}^{2}}{2m} $$
	where, $k_{F}$ is the fermi wavevector
- the **fermi surface** separates filled from empty states, and it is a sphere of radius, $k_F$, in the $k$-space
#fig 

$$\begin{align*} 
N &= \frac{\text{volume of fermi surface}}{\text{volume of one state}} \\
&= \frac{\cfrac{4}{3} \pi k_{F}^{3}}{12(\cfrac{2\pi}{L})^{3}} \\
 \implies k_{F}^{3} &= 3\pi ^{2}n
\end{align*}$$
$$E_{F} = \frac{\hbar^{2}}{2m} (3\pi^{2}n)^{2/3}$$

- eg: copper, $n = 8.5 \times10^{28}$ m$^{-3}$, $E_{F }= 7.0$ eV, $T_{F}= E_F /k_{B} = 80\,000$ K
- this is much higher than room temperature, so the low temperature limit approximation holds

## degeneracy pressure
- pressure due to the electron gas at $T=0$
$$\begin{align*}
\langle{E}\rangle &= \frac{U}{N} \\
&= \frac{\int_{0}^{\infty} Eg(E)f_{FD}(E)dE}{\int_{0}^{\infty} g(E)f_{FD}(E)dE} \\
&= \frac{\int_{0}^{E_{F}} Eg(E)dE}{\int_{0}^{E_{F}} g(E)dE} \\
&= \frac{3}{5}E_{F}
\end{align*}$$
$$U = \frac{3N}{5}E_{F}$$

$$