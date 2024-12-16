---
{"dg-publish":true,"permalink":"/content/012/px-284-statistical-mechanics/e-single-particle-partition-function/px-284-e6-harmonic-oscillator-in-3-d/","noteIcon":"1","created":"2024-11-29T18:14:58.089+00:00","updated":"2024-11-29T18:38:36.098+00:00"}
---

- the energy is given by:
$$E = \left(n_{x} + \frac{1}{2}\right) \hbar \omega +  \left(n_{y} + \frac{1}{2}\right) \hbar \omega +  \left(n_{z} + \frac{1}{2}\right) \hbar \omega$$
- the partition function:
$$Z_{3D} = Z_{x} Z_{y} Z_{z} = (Z_{1D})^{3}$$
- the internal energy:
$$U_{3D} = 2\,U_{1D} $$
- eg: spin$-1/2$ paramagnet
- a single spin$-1/2$ particle in a magnetic field is a two-state system
![Pasted image 20241129182336.png|500](/img/user/pics/Pasted%20image%2020241129182336.png)
- the spin$-1/2$ magnetic moment along $z$:
$$M = - g\mu_BM_{s}= \mp\mu_B$$
	where, $\mu_B$ is the 'bohr magneton' $= e\hbar/2m$, $g=2$, and $M_{s}= \pm 1/2$
- the energy:
$$E = - \vec\mu \cdot \vec B$$
$$Z_{1} = \exp(\beta\mu_{B}B) + \exp(-\beta\mu_{B}B) = 2\cosh(\beta\mu_{B}B)$$
- a paramagnet is an array of $N$ non-interacting spins
- here, the $N$-particle partition function is:
$$Z_{N} = (Z)^N$$
- for a magnetic system, the first law of thermodynamics can be written as:
$$dU = T\,dS - m\,dB$$
- two possible configurations of the paramagnet could be:
- $(A):$ all moments up, $m = N\mu_B$
	- saves internal energy when $B=0$
	- there is only one microstate
- $(B):$ random orientation with half up and half down
	- does not save internal energy
	- lots of microstates
	- maximum entropy

![Pasted image 20241129182920.png|500](/img/user/pics/Pasted%20image%2020241129182920.png)

- the hemholtz free energy:
$$\begin{align*}
F &= U-T\,dS \\
dF  &= S\,dT - m\,dB
\end{align*}$$
	where, $m = - \left(\frac{\partial F}{\partial B}\right)_{T}$, and ${} M = m/V {}$ is the magnetization
$$\begin{align*}
F &= -k_{B} T \ln Z_{n} \\
&= -k_{B}T \ln (Z)^{n} \\
&= -nk_{B}T \ln [2\cosh(\mu_{B}\beta B)]
\end{align*}$$
$$\therefore M = n \mu_{B} \tanh(\beta\mu_{B} B)$$
	where, $n = N/V$

![Pasted image 20241129183445.png|500](/img/user/pics/Pasted%20image%2020241129183445.png)
- $(A)$ is at high $B/T$, the ground state is favoured $\implies U$ wins
- $(B)$ is at low $B/T$, all microstates are equiprobable $\implies S$ wins
