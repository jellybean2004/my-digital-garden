---
{"dg-publish":true,"permalink":"/content/012/px-284-statistical-mechanics/e-single-particle-partition-function/px-284-e4-degeneracy/","noteIcon":"1","created":"2024-11-29T17:37:55.071+00:00","updated":"2024-12-23T22:58:34.331+00:00"}
---

[[content/012/PX262 - quantum mechanics/term 1/C - the basic postulates/PX262 - C9a - degeneracy\|PX262 - C9a - degeneracy]]

- degenerate states are two or more states that have the same energy

- considering the [[content/012/PX262 - quantum mechanics/term 1/G - additional interactions/PX262 - G2b - spin\|spin]] of a particle: $S = \hbar\sqrt{s(s+1)}$
- the component of $S$ along a particular direction: $S_{z} = \hbar m_{s}$, where $m_{s}$ is the magnetic spin quantum number
- each energy level of a particle with spin, $s$ is $(2s+1)$ degenerate
- these levels are split by a magnetic field, [[content/012/PX262 - quantum mechanics/term 1/G - additional interactions/PX262 - G6c - zeeman effect\|PX262 - G6c - zeeman effect]]

- eg: for an electron $(s = 1/2)$, there are $(2s+1=)~2$ spin states

![Pasted image 20241129174217.png|500](/img/user/pics/Pasted%20image%2020241129174217.png)

- to account for degeneracy, the partition function:
$$Z = \sum\limits_{i} g(E_{i}) \exp(-\beta E_{i})$$
	where, $g(E_i)$ is the number of distinct states associated with $E_i$ 

- eg: for a particle with spin, $s$, in a quantum system with zero field:
$$Z = \sum\limits_{i} (2s+1)\exp(-\beta E_{i})$$
- eg: two level system with degeneracies $g_1$ and $g_2:$
$$\begin{gather}
E & & g(E) \\\\
\Delta & \_\_\_\_\_& g_{1} \\\\
0 & \_\_\_\_\_& g_{2}
\end{gather}$$
$$\begin{gather*}
	Z = g_{1} + g_{2}\exp(-\beta\Delta)\\
	\ln Z  = \ln(g_{1} +  g_{2}\exp(-\beta\Delta)) \\\\
	U = \frac{d}{d\beta} (\ln Z) = g_{2}\Delta \exp(-\beta\Delta \exp(-\beta\Delta))
\end{gather*}$$
