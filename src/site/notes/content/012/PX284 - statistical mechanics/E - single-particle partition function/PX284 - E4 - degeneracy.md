---
{"dg-publish":true,"permalink":"/content/012/px-284-statistical-mechanics/e-single-particle-partition-function/px-284-e4-degeneracy/","created":"2024-11-29T17:37:55.071+00:00","updated":"2024-11-29T17:52:22.874+00:00"}
---

- degenerate states are two or more states that have the same energy
- eg: spin (angular momentum intrinsic to a particle)
	- the spin angular momentum: $S = \hbar\sqrt{s(s+1)}$
	- the component of $S$ along a particular direction: $S_{z} = \hbar m_{s}$, where $m_{s}$ is the magnetic spin quantum number
	- each energy level of a particle with spin, $s$ is $(2s+1)$ degenerate
	- these levels are split by a magnetic field
- eg: for an electron $(s = 1/2)$, there are $(2s+1=)2$ spin states
![Pasted image 20241129174217.png|500](/img/user/pics/Pasted%20image%2020241129174217.png)

- to account for degeneracy, the partition function:
$$Z = \sum\limits_{i} g(E_{i}) \exp(-\beta E_{i})$$
	where, $g(E_i)$ is the number of distinct states associated with $E_i$ 
- eg: for a particle with spin, $s$, in a quantum system with zero field:
$$Z = \sum\limits_{i} (2s+1)\exp(-\beta E_{i})$$
- eg: two level system with degeneracies $g_1$ and $g_2:$
![Pasted image 20241129174623.png|500](/img/user/pics/Pasted%20image%2020241129174623.png)
$$\begin{gather*}
	Z = g_{1} + g_{2}\exp(-\beta\Delta)\\
	\ln Z  = \ln(g_{1} +  g_{2}\exp(-\beta\Delta)) \\\\
	U = \frac{d}{d\beta} (\ln Z) = g_{2}\Delta \exp(-\beta\Delta \exp(-\beta\Delta))
\end{gather*}$$
