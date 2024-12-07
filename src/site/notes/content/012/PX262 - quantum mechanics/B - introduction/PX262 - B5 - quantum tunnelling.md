---
{"dg-publish":true,"permalink":"/content/012/px-262-quantum-mechanics/b-introduction/px-262-b5-quantum-tunnelling/","created":"2024-11-25T10:50:32.000+00:00","updated":"2024-12-07T18:22:00.560+00:00"}
---

![Pasted image 20241207182156.png|500](/img/user/pics/Pasted%20image%2020241207182156.png)

- considering a particle travelling from $x= -\infty$, with an energy, $E$, that encounters a potential barrier: 
  $$V= \begin{cases} V_{0}& for\,x\in[0,b] \\ 0 & elsewhere \end{cases}$$
- when $E<V_{0}$, in quantum mechanics, particle may get through
- considering the wavefunctions in the regions:
$$\begin{align*}
	\phi_{I}(x) &= Ae^{ikx}+Be^{-ikx} \\
	\phi_{II}(x) &= Ce^{\kappa x} + De^{\kappa x} \\
	\phi_{III}(x) &= Fe^{ikx}
\end{align*}$$
	where, $\kappa=\sqrt{\frac{2m(V_{0}-E)}{\hbar^{2}}}$
- $\phi(x)$ and its derivative must be continuous at $x=0$ and $x=b:$ 
$$\begin{gather*}
	\phi_{I}(0) = \phi_{II}(0) & \phi_{II}(b) = \phi_{III}(b) \\
	\phi_{I}'(a) = \phi_{II}'(a) & \phi_{II}'(b) = \phi_{III}'(b) \\
\end{gather*}$$
- using these conditions, the probability of the particle passing through the barrier is: 
  $$T = \frac{|F|^{2}}{|A|^{2}} = \frac{16E(V_{0}-E)}{V_{o}^{2}}e^{-2\kappa b}$$
- phenomena like $\alpha-$decay, nuclear fission can be explained only using quantum tunnelling
