---
{"dg-publish":true,"permalink":"/content/012/px-285-hamiltonian-mechanics-and-fluid-dynamics/term-2-fluid-dynamics/i-navier-stokes-equation/px-285-i3b-water-drain/","noteIcon":"1","created":"2025-01-31T12:30:57.597+00:00","updated":"2025-01-31T12:31:06.085+00:00"}
---


- eg: water draining from a tank through a pipe at its base
- the height of the water is $H$
- the rate of drain is $\vec u_{2}$
- the height falls at the rate, $\vec u_{1}$
- $P_{atm}$ applies at the water surface as well as the mouth of the pipe

![PX285 - I3 - bernoulli's principle-2.png](/img/user/pics/PX285%20-%20I3%20-%20bernoulli's%20principle-2.png)

$$\begin{align*}
P_{atm} + \frac{\rho  u_{1}^{2}}{2} + \rho gH &= P_{atm} + \frac{\rho u_{2}^{2}}{2} \\
\rho gH &= \frac{\rho}{2} ( u_{2}^{2}- u_{1}^{2})
\end{align*}$$
- assuming the pipe is narrow, ie: $u_{2} \gg u_{1}:$
$$u_{2} = \sqrt{2gH}$$

- this is the freefall speed
- from conservation of energy:
$$\begin{gather}
mgH = \frac{1}{2}mv^{2} \\
y = \sqrt{2gH}
\end{gather}$$

- assuming the flow to be slow, ie. bernoulli's principle is applicable

- the surface of the tank, $A_t$
- cross section of the pipe, $A_p$
- $A_{t} \gg A_p$
- the initial volume of water: $V (t = 0) = A_{t}H(t=0)$
- when it drains completely, $V(t_{d}) = A_{t} \times o$
- the rate of change of the volume:
$$\frac{dV}{dt} = A_{t} \frac{dH}{dt} = - A_{p}u_{z}(H) = - A_{p}\sqrt{2gH(t)}$$

- solving the ODE by separation of variables:
$$A_{t} \int_{H(0)}^{0} \frac{dH}{H^{1/2}}
= - A_{p}\sqrt{2g} \int_{0}^{t_{d}} dt$$
$$\therefore t_{d}= \frac{A_{t}}{A_{p}} \sqrt{\frac{2H(0)}{g}}$$

- considering a horizontal pipe at varying cross sections
#fig 
- from bernoulli's principle:
$$\begin{gather}
P_{1}+ \rho \frac{u_{1}^{2}}{2} = P_{2} + \rho \frac{u_{2}^{2}}{2}\\
(P_{1} - P_{2}) = \frac{\rho}{2} ( u_{2}^{2} - u_{1}^{2})  \\
= \frac{\rho}{2}u_{1}^{2} \left( \frac{u_{2}^{2}}{u_{1}^{2}} -1\right) 
\end{gather}$$
- from mass conservation:
$$u_{1}A_{1} = u_{2}A_{2} \implies \frac{u_{1}}{u_{2}}= \frac{A_{2}}{A_{1}}$$
$$\therefore P_{2} - P_{2} = \frac{\rho}{2} u_{1}^{2} \left(\frac{A_{1}^{2}}{A_{2}^{2}}- 1\right)$$

- using a monometer - a bent pipe of constant cross section filled with mercury, with density, $\rho_{m}$, such that $\rho_{m} \gg \rho$
#fig 
$$\begin{gather}
P_{1} = P_{2} + \rho_{m} g \Delta z \\
P_{1} - P_{2} = \rho_{m} g \Delta z
\end{gather}$$
$$u_{1}^{2} = \left[2 \left(\frac{\rho_{m}}{\rho}\right) g\right]\Delta z \left(\frac{A_{1}^{2}}{A_{2}^{2}} -1 \right)^{-1}$$
	where, all but $z$ are constants
