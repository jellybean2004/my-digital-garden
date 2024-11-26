---
dg-publish: true
---

## interlude
- often, the [[content/011/PX154 - physics foundations/PX154 - D - the first law of thermodynamic/PX154 - D2 - the first law\|the first law]] is written as: 
$$dU=dQ-dW$$
- eg: have used $dW =pdV$

- from *[[content/011/PX154 - physics foundations/PX154 - C - thermal physics 2/PX154 - C9 - heat capacity of the ideal gas\|the heat capacity of the ideal gas]]*: 
$$C_{V}=\frac{1}{n} \frac{dQ}{dT}\Bigg|_{V}$$
- if $V$ is constant, then it is an isochore, and 
$$W=0$$
- ie: $dU = dQ - dW$, with $dW = 0$, so: 
$$dU = dQ$$
- hence: 
$$C_{V} = \frac{1}{n} \frac{dU}{dT}\bigg |_{V}$$
- for constant pressure: 
$$C_{P} = \frac{1}{n} \frac{dQ}{dT} \bigg\vert_p$$
- here, volume can change, so, $dW\neq 0$

- $C_{P}$ and $C_{V}$ can be related for the ideal gas: 
$$\begin{align*}
	dU &= dQ - dW \\\\
	dQ &= dU + dW \\\\
	dQ &= dU + pdV \\\\
	n \, C_{p} \, dT &=  n \, C_{V} \, dT + n \, R \, dT \\\\
	\therefore C_{P} &= C_{V} + R
\end{align*}$$ [YF eqn 19.7]
- it is also useful to define: 
$$\gamma = \frac{C_{{P}}}{C_{V}}$$
	- eg: for a monatomic gas
		- $C_{V}= \frac{3}{2}R$, so, $C_{P}= \frac{5}{2}R$, and $\gamma = \frac{5}{3}$
	- eg: for a diatomic gas
		- $C_{V}= \frac{5}{2}R$, so, $C_{P}= \frac{7}{2}R$, and $\gamma = \frac{7}{5}$
