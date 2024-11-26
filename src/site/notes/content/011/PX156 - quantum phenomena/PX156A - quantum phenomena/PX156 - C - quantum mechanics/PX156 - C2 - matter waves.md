---
{"dg-publish":true,"permalink":"/content/011/px-156-quantum-phenomena/px-156-a-quantum-phenomena/px-156-c-quantum-mechanics/px-156-c2-matter-waves/","created":"2024-11-25T10:50:32.000+00:00","updated":"2024-11-26T20:01:59.110+00:00"}
---


- *[[content/011/PX156 - quantum phenomena/PX156A - quantum phenomena/PX156 - A - light/PX156 - A3b - planck's function\|planck]]*: 
$$E = hf = \hbar \omega$$
- *[[content/011/PX156 - quantum phenomena/PX156A - quantum phenomena/PX156 - B - atomic stucture/PX156 - B3 - de broglie hypothesis\|de broglie]]*: 
$$p = \frac{h}{\lambda}= \hbar k$$
$$E = \frac{\hbar^{2}k^{2}}{2m} = \frac{p^{2}}{2m} = KE$$

- $\psi = \cos(kx-\omega t)$ is not a solution of *TDSE*
## normalization condition
$$\begin{align*}
	\psi &= \psi_{1}+ i\psi_{2} \\
	|\psi| &= \sqrt{\psi_{2}^{2}+ \psi_{2}^{2}} \\\\
	|\psi|^{2} &= \psi_{1}^{2}+\psi_{2}^{2}\\
	&= \psi\psi^{*} \\
	&= (\psi_{1}+i\psi_{2})(\psi_{1}-i\psi_{2})
\end{align*}$$
- max born proposed: 
$$\int_{a}^{b} |\psi(x,t)|^{2}\,dx = \int_{a}^{b} \psi(x,t)\,\psi^{*}(x,t)\,dx$$
	which can be used to calculate the probability of finding the particle between $a$ and $b$, at time $t$
- the normalization condition: 
$$\int_{all\, space} |\psi(x,t)|^{2}dx =1$$
	- the particle should be somewhere in all of space
	- ie: $|\psi|^{2}\to0$ as $x \to\pm\infty$

- plane wave: 
$$|\psi|^{2}= \psi\psi^{*} = A\exp(i(kx-\omega t)) \cdot A\exp(-i(kx-\omega t)) = A^{2}$$
- therefore plane waves cannot represent matter waves

- solution: [[content/011/PX156 - quantum phenomena/PX156A - quantum phenomena/PX156 - C - quantum mechanics/PX156 - C3 - wave packets\|wave packet]]
	- $\psi_{1}$ and $\psi_{2}$ are the solutions of the *TDSE*: 
	$$- \frac{\hbar^{2}}{2m} \frac{\partial^{2} {\psi_{1}}}{\partial {x}^{2}} = i\hbar \frac{\partial \psi_{1}}{\partial t}\;,\; and\; - \frac{\hbar^{2}}{2m} \frac{\partial^{2} {\psi_{2}}}{\partial {x}^{2}} = i\hbar \frac{\partial \psi_{2}}{\partial t}$$
	- then, any linear combination of $\psi_{1}$ and $\psi_{2}$ is also a solution: 
	$$\psi = \alpha\psi_{1}+\beta\psi_{2}$$ $$- \frac{\hbar^{2}}{2m} \frac{\partial^{2}}{\partial {x}^{2}}(\alpha\psi_{1}+\beta\psi_{2}) = i\hbar \frac{\partial}{\partial t}(\alpha\psi_{1}+\beta\psi_{2})$$
		- $\alpha$ and $\beta$ are constants