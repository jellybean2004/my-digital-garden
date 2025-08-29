---
{"dg-publish":true,"permalink":"/content/012/px-284-smeto/part-1-statistical-mechanics/e-single-particle-partition-function/px-284-e5c-spin-half-paramagnet/","noteIcon":"1","created":"2025-08-27T13:15:25.043+01:00","updated":"2025-01-03T12:31:00.000+00:00"}
---

- a single spin$-1/2$ particle in a magnetic field is a two-state system
$$\begin{gather}
\uparrow & \_\_\_\_\_\_\_\_ &E_{1}=\mu_{B}B \\\\
\downarrow & \_\_\_\_\_\_\_\_  &E_{1}=-\mu_{B}B
\end{gather}$$
- the magnetic moment along $z$ is:
$$\mu = - g\mu_B m_{s}= \mp\mu_B$$
	where, $\mu_B$ is the 'bohr magneton' $= e\hbar/2m$, $g=2$, and $m_{s}= \pm 1/2$
- the energy is:
$$E = - \vec\mu \cdot \vec B$$
- the single particle partition function is:
$$Z_{1} = \exp(\beta\mu_{B}B) + \exp(-\beta\mu_{B}B) = 2\cosh(\beta\mu_{B}B)$$

- a **paramagnet** is an array of $N$ *non-interacting* spins

- here, the $N$-particle partition function is:
$$Z_{N} = (Z_{1})^N$$
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
	where, $m = - \left(\frac{\partial F}{\partial B}\right)_{T}$, and ${} M = m/V$ is the magnetization
$$\begin{align*}
F &= -k_{B} T \ln Z_{n} \\
&= -k_{B}T \ln (Z)^{n} \\
&= -Nk_{B}T \ln [2\cosh(\mu_{B}\beta B)]
\end{align*}$$
$$\therefore M = n \mu_{B} \tanh(\beta\mu_{B} B)$$
	where, $n = N/V$

![Pasted image 20241129183445.png|500](/img/user/pics/Pasted%20image%2020241129183445.png)
- $(A)$ is at high $B/T$, the ground state is favoured $\implies U$ wins
- $(B)$ is at low $B/T$, all microstates are equiprobable $\implies S$ wins
