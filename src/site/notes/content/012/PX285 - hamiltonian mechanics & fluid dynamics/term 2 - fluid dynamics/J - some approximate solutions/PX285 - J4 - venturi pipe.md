---
{"dg-publish":true,"permalink":"/content/012/px-285-hamiltonian-mechanics-and-fluid-dynamics/term-2-fluid-dynamics/j-some-approximate-solutions/px-285-j4-venturi-pipe/","noteIcon":"1","created":"2025-02-01T14:15:44.585+00:00","updated":"2025-02-01T14:27:55.964+00:00"}
---

- considering a horizontal pipe of varying cross section

![PX285 - I3b - water drain.png|500](/img/user/pics/PX285%20-%20I3b%20-%20water%20drain.png)

- from bernoulli's principle:
$$\begin{gather}
P_{1}+ \rho \frac{u_{1}^{2}}{2} = P_{2} + \rho \frac{u_{2}^{2}}{2}\\
(P_{1} - P_{2}) = \frac{\rho}{2} ( u_{2}^{2} - u_{1}^{2})  \\
= \frac{\rho}{2}u_{1}^{2} \left( \frac{u_{2}^{2}}{u_{1}^{2}} -1\right) 
\end{gather}$$
- from mass conservation:
$$u_{1}A_{1} = u_{2}A_{2} \implies \frac{u_{1}}{u_{2}}= \frac{A_{2}}{A_{1}}$$
$$\therefore P_{2} - P_{2} = \frac{\rho}{2} u_{1}^{2} \left(\frac{A_{1}^{2}}{A_{2}^{2}}- 1\right) \tag{1}$$

- using a monometer - a bent pipe of constant cross section filled with mercury, with density, $\rho_{m}$, such that $\rho_{m} \gg \rho$

![PX285 - I3c - pitot pipe.png|500](/img/user/pics/PX285%20-%20I3c%20-%20pitot%20pipe.png)

$$\begin{gather}
P_{1} = P_{2} + \rho_{m} g \Delta z \\
P_{1} - P_{2} = \rho_{m} g \Delta z
\end{gather}$$
- substituting this into equation $(1):$
$$u_{1}^{2} = \left[2 \left(\frac{\rho_{m}}{\rho}\right) g\right]\Delta z \left(\frac{A_{1}^{2}}{A_{2}^{2}} -1 \right)^{-1}$$
	where, all but $z$ are constants