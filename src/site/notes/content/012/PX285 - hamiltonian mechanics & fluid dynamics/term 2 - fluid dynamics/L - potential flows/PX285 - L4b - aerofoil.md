---
{"dg-publish":true,"permalink":"/content/012/px-285-hamiltonian-mechanics-and-fluid-dynamics/term-2-fluid-dynamics/l-potential-flows/px-285-l4b-aerofoil/","noteIcon":"1","created":"2025-08-27T13:15:24.485+01:00","updated":"2025-03-07T13:28:30.000+00:00"}
---

![PX285 - L6 - airfoils.png](/img/user/pics/PX285%20-%20L6%20-%20airfoils.png)

- applying [[content/012/PX285 - hamiltonian mechanics & fluid dynamics/term 2 - fluid dynamics/J - some approximate solutions/PX285 - J1a - bernoulli's principle from conservation of energy\|bernoulli's principle]] above and below the aerofoil:
$$\begin{gather}
P_{0} + \frac{\rho U_{0}^{2}}{2} = P_{T} + \frac{\rho u_{T}^{2}}{2} \\
P_{0} + \frac{\rho U_{0}^{2}}{2} = P_{B} + \frac{\rho u_{B}^{2}}{2} \\
P_{B} - P_{T} = \frac{\rho}{2} (u_{T}^{2} - u_{B}^{2}) = \frac{\rho}{2} (u_{T} + u_{B}) (u_{T} - u_{B}) \simeq  \frac{\rho}{2} 2U_{0} (u_{T} - u_{B})
\end{gather}$$
-  the total lift:
$$L = \int_{0}^{d} (P_{B} - P_{T})\, dx = \rho U_{0} \left[\int_{0}^{d} u_{T}\, dx + \int_{d}^{0} u_{B} dx \right] = \rho U_{B} \oint \vec u \cdot d\vec l$$
- the closed integral is clockwise around the aerofoil
- if $K = \oint \vec u \cdot d\vec l > 0$, the lift is upwards:
$$\vec L = \rho  \vec u \times \vec K$$

