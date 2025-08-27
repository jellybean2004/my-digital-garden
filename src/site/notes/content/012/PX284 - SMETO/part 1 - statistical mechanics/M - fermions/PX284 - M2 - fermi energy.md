---
{"dg-publish":true,"permalink":"/content/012/px-284-smeto/part-1-statistical-mechanics/m-fermions/px-284-m2-fermi-energy/","noteIcon":"1","created":"2025-08-27T13:15:24.866+01:00","updated":"2025-02-03T19:34:15.000+00:00"}
---

- putting $N$ electrons into a metal one by one
- the energy levels fill up one by one because of the [[content/012/PX284 - SMETO/part 1 - statistical mechanics/L - exchange symmetry/PX284 - L2 - pauli exclusion principle\|pauli exclusion principle]] until no more electrons are left
- the highest energy reached is called the **fermi energy**, $E_{F}$
- this is seen from ${} f_{FD}(E)$ as $R\to0:$
$$f_{FD} = \begin{cases} 1 & E<E_{F} \\ 0 & E>E_{F}\end{cases}$$

![PX284 - M2 - fermi energy.png|500](/img/user/pics/PX284%20-%20M2%20-%20fermi%20energy.png)

$$E_{F} \equiv \mu(T=0)$$
- to evaluate $E_F:$ 
$$N = \int_{0}^{\infty} g(E)\, f_{FD}(E)\,dE = \int_{0}^{E_{F}} g(E)\,dE = \frac{V}{2\pi^{2}} \left(\frac{2m}{\hbar}\right)^{3/2}\frac{E_{F}^{3/2}}{3/2}$$

- therefore, the fermi energy is:
$$E_{F}= \frac{\hbar^{2}}{2m} (3\pi^{2}n)^{\frac{2}{3}}\tag{1}$$
	where, $n = N/V$ is the carrier density

- alternatively:
$$E_{F}= \frac{\hbar^{2}k_{F}^{2}}{2m} $$
	where, $k_{F}$ is the fermi wavevector

- the **fermi surface** separates filled from empty states
- it is a sphere of radius, $k_F$, in the $k$-space

![PX284 - M2 - fermi energy-1.png|500](/img/user/pics/PX284%20-%20M2%20-%20fermi%20energy-1.png)

$$\begin{align*} 
N &= \frac{\text{volume of fermi surface}}{\text{volume of one state}} \\
&= \frac{\cfrac{4}{3} \pi k_{F}^{3}}{\cfrac{1}{2}\left(\cfrac{2\pi}{L}\right)^{3}} \\\\
\implies k_{F}^{3} &= 3\pi ^{2}n \\
E_{F} &= \frac{\hbar^{2}}{2m} (3\pi^{2}n)^{2/3}
\end{align*}$$

- eg: copper, $n = 8.5 \times10^{28}$ m$^{-3}$, $E_{F }= 7.0$ eV, $T_{F}= E_F /k_{B} = 80\,000$ K
- this is much higher than room temperature, so the low temperature limit approximation holds
