---
{"dg-publish":true,"permalink":"/content/012/px-284-statistical-mechanics/c-entropy-and-temperature/px-284-c2-temperature/","noteIcon":"1","created":"2024-11-25T10:50:32.000+00:00","updated":"2024-11-27T17:56:46.594+00:00"}
---

- considering two systems that can exchange energy, and the combined system is isolated
- **equilibrium** is reached when $\Omega_{tot}$ is maximized: 
$$\begin{gather*}
	\frac{d\Omega_{1}\Omega_{2}}{dE_{1}} = 0 \\
	\Omega_{2} \frac{d\Omega_{1}}{dE_{1}} + \Omega_{1}\frac{d\Omega_{2}}{dE_{2}} \frac{dE_{2}}{dE_{1}} = 0 \\
\end{gather*}$$
- $E = E_{1}+E_{2}$ is fixed, so, $dE_{1} = - dE_{2} \implies \frac{dE_{2}}{dE_{1}} = -1:$ 
$$\begin{gather*}
	\frac{1}{\Omega_{1}} \frac{d\Omega_{1}}{dE_{1}} - \frac{1}{\Omega_{2}} \frac{d\Omega_{2}}{dE_{2}} = 0 \\
\frac{	d\ln\Omega_{1}}{dE_{1}} = \frac{d\ln\Omega_{2}}{dE_{2}}
\end{gather*}$$

- statistically defining the temperature using the expression: 
$$\frac{1}{k_{B}T} = \frac{d\ln\Omega}{dE}$$
- it is found that $T_{1} = T_{2}$ at equilibrium

- in **thermodynamics**, for an isolated system, [[content/011/PX154 - physics foundations/PX154 - D - the first law of thermodynamic/PX154 - D2 - the first law\|the first law]] states: 
$$dU = T\,dS - p\,dV \implies \frac{1}{T} = \left(\frac{\partial S}{\partial V}\right)_{V}$$
- in **statistical mechanics**, for an isolated system: 
$$\frac{1}{T} = \frac{d}{dE} (k_{B}\ln\Omega) = \frac{dS}{dE}$$

- **note:** 
	- $k_{B}T$ has the same units as energy
	- defining $\beta = \frac{1}{k_{B}T}$
