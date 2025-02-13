---
{"dg-publish":true,"permalink":"/content/012/px-285-hamiltonian-mechanics-and-fluid-dynamics/px-285-k2-kelvin-s-circulation-theorem/","noteIcon":"1","created":"2025-02-13T14:28:19.073+00:00","updated":"2025-02-13T15:04:37.300+00:00"}
---

- the circulation, $K$, around a closed loop, $\Gamma$, is moving with the fluid is constant for an inviscid flow
## proof

$$\begin{align*}
\frac{dK}{dt} &= \frac{d}{dt} \left[ \oint_{\Gamma} \vec u \cdot d\vec l \right] \\
&= \oint_{\Gamma} \frac{d\vec u}{dt} \cdot d\vec l + \oint_{\Gamma} \vec u \cdot \frac{d}{dt}(d\vec l) \\
&= I_{1} + I_{2}
\end{align*}$$

- considering two nearby points on $\Gamma$

![PX285 - K2 - kelvin's circulation theorem.png](/img/user/pics/PX285%20-%20K2%20-%20kelvin's%20circulation%20theorem.png)
#fig 

$$\begin{gather}
d\vec l = \vec r_{2}= \vec r_{1} \\
\frac{d}{dt} d\vec l = \frac{d\vec{r_{2}}}{dt} - \frac{d\vec{r_{2}}}{dt} = \vec u_{2} - \vec u_{1} = d\vec u \\\\
I_{2} = \oint_{\Gamma} \vec u \frac{d}{dt}(\vec l) = \oint_{\Gamma} \vec u \cdot d\vec u \\
= \oint_{\Gamma} d\left(\frac{u^{2}}{2}\right) = 0
\end{gather}$$
- because it is the integral of a perfect differential along a closed path

- using the [[content/012/PX285 - hamiltonian mechanics & fluid dynamics/term 2 - fluid dynamics/I - navier-stokes equation/PX285 - I2a - conservation of momentum\|navier-stokes equation]]:
$$\frac{dK}{dt} = \oint_{\Gamma} \left( - \frac{\vec\nabla{p}}{\rho} + g\vec\nabla z\right)\cdot d\vec l + 0$$

## incompressible
- considering the incompressible limit: $\vec\nabla\cdot\vec u = 0$
$$\frac{dK}{dt} = \frac{1}{\rho} \oint_{\Gamma} (- \vec\nabla p) \cdot d\vec l + g \oint_{\Gamma} \vec\nabla z \cdot d\vec l = 0$$

- therefore, $K$ is a constant, or, an **invariant of fluid motion**

## barotropic
- $\rho = \rho(p)$ only
- eg: adiabatic flow
$$\frac{p}{\rho^{\gamma}} = \text{ constant} \implies p \propto \rho^{\gamma}$$

#incomplete 
