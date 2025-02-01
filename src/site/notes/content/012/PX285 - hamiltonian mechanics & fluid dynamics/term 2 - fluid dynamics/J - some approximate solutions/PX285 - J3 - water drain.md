---
{"dg-publish":true,"permalink":"/content/012/px-285-hamiltonian-mechanics-and-fluid-dynamics/term-2-fluid-dynamics/j-some-approximate-solutions/px-285-j3-water-drain/","noteIcon":"1","created":"2025-01-31T12:30:57.597+00:00","updated":"2025-02-01T14:11:08.361+00:00"}
---

- considering water draining from a tank through a pipe at its base
- $P_{atm}$ applies at the water surface as well as the mouth of the pipe

![PX285 - I3 - bernoulli's principle-2.png|500](/img/user/pics/PX285%20-%20I3%20-%20bernoulli's%20principle-2.png)

- applying [[content/012/PX285 - hamiltonian mechanics & fluid dynamics/term 2 - fluid dynamics/J - some approximate solutions/PX285 - J1a - bernoulli's principle from conservation of energy\|bernoulli's principle]]:
$$\begin{align*}
P_{atm} + \frac{\rho  u_{1}^{2}}{2} + \rho gH &= P_{atm} + \frac{\rho u_{2}^{2}}{2} \\
\rho gH &= \frac{\rho}{2} ( u_{2}^{2}- u_{1}^{2})
\end{align*}$$
- assuming the pipe is narrow, ie: $u_{2} \gg u_{1}:$
$$u_{2} \approx \sqrt{2gH}$$
- this is the freefall speed

- from conservation of energy:
$$\begin{gather}
mgH = \frac{1}{2}mv^{2} \\
v = \sqrt{2gH}
\end{gather}$$

- assuming the flow to be slow, ie. bernoulli's principle is applicable

- the cross section of the tank, $A_t$, and the cross section of the pipe, $A_p$, such that $A_{t} \gg A_p$
- the initial volume of water: 
$$V (t = 0) = A_{t}H(t=0)$$
- when it drains completely, $H =0:$ 
$$V(t_{d}) = A_{t} \times 0$$
- the rate of change of the volume:
$$\frac{dV}{dt} = A_{t} \frac{dH}{dt} = - A_{p}u_{z}(H) = - A_{p}\sqrt{2gH(t)}$$

- solving the ODE by separation of variables:
$$A_{t} \int_{H(0)}^{0} \frac{dH}{H^{1/2}}
= - A_{p}\sqrt{2g} \int_{0}^{t_{d}} dt$$
$$\therefore t_{d}= \frac{A_{t}}{A_{p}} \sqrt{\frac{2H(0)}{g}}$$

- here, the fluid speed remains constant regardless of the depth
- but, it is known that the speed at the pipe, $u_2$, is faster than at the surface, $u_1$
- this leads to the conclusion that the speed goes from $u_1$ to $u_2$ instantaneously at the outflow entrance
- this arises due to the assumptions that the fluid speed in the rank is zero, and the fluid is incompressible
