---
dg-publish: true
---

## geiger-nuttall law
$$\ln \lambda = - C_{1} \frac{Z-2}{\sqrt{E}}+ C_{2}$$
	$\lambda=$ decay constant
	$Z =$ atomic number
	$E=$ energy of the emitted $\alpha$ particle
	$C_{1}, C_{2}=$ constants

![Pasted image 20240326121351.png](/img/user/pics/Pasted%20image%2020240326121351.png)

- the alpha particle is in the potential well of the nucleus
- a classical particle must have an energy greater than the barrier to escape, but a quantum particle doesn't have to
- classically, alpha decay cannot be explained
- alpha decay happens due to quantum tunnelling

- $N(t)=$ number of nuclei remaining at time, $t:$ $$\frac{dN}{dt}= -\lambda N$$
	$\tau= \frac{1}{\lambda} =$ life time 
$$\begin{align*}
	N(t_\frac{1}{2}) &= \frac{1}{2}N(0) = N(0) \exp \left({-\lambda t_\frac{1}{2}}\right)\\
	\therefore t_\frac{1}{2} &= \ln\left(\frac{2}{\lambda}\right) = \tau \ln(2)
\end{align*}$$

- an $\alpha$ particle: $2p^{+},\; 2n^{0}$
- atomic number of nucleus$:Z$
- charges $:Q_{1}=2^{+},\; Q_{2} = (Z-2)^{+}$
- potential energy: 
$$V(r) = \frac{2(Z-2)e^{2}}{4\pi \epsilon_{0}r}$$
- if the particle escapes: 
$$E_{K} = V(r) = \frac{2(Z-2)e^{2}}{4\pi \epsilon_{0}d}$$
	where, $d=$ width of barrier
$$\begin{gather}
	d = \frac{(Z-2)e^{2}}{2\pi\epsilon_{0}E_{K}} \\
	T \sim \exp\left(- \frac{(Z-2)e^{2}\sqrt{2m(V-E_{K})}}{\pi\epsilon_{0}E_{K}\hbar}\right)
\end{gather}$$
- for $V>>E_{K}:$ 
$$T \sim \exp\left(- \frac{A(Z-2)}{E_{K}}\right)$$
	where, $A=$ collection of constants

 - in reality, there are a range of kinetic energies, so to account for that, an integral must be taken: 
 $$\begin{align*}
	T &\sim \exp\left(- \frac{2\sqrt{2m}}{\hbar} \int_{R}^{r'} \sqrt{\frac{2(Z-2)e^{2}}{r} -E_{K}} \,dr\right) \\
	&= \exp\left(-C_{1}\frac{Z-2}{\sqrt{E_{K}}}\right)
\end{align*}$$
- $\lambda=$ decay rate = number of attempts at the barrier per unit time $\times T:$ 
$$\begin{align*}
		\lambda &= \frac{v}{2R} T \\
		\ln \lambda &= - C_{1} \frac{Z-2}{\sqrt{E}}+ C_{2}		
	\end{align*}$$
	where, ${} v=$  velocity if $\alpha$ particle inside
- **note:** $\lambda$ as well as $25$ orders of magnitude, while $E_{K}$ changes very little ($4-9\, MeV$)