---
{"dg-publish":true,"permalink":"/content/012/px-285-hamiltonian-mechanics-and-fluid-dynamics/term-2-fluid-dynamics/k-circulation-and-vorticity/px-285-k2-kelvin-s-circulation-theorem/","noteIcon":"1","created":"2025-08-27T13:15:24.366+01:00","updated":"2025-02-14T15:06:47.000+00:00"}
---

>[!info] kelvin's circulation theorem
>the circulation, $K$, around a closed loop, $\Gamma$, is moving with the fluid is constant for an inviscid flow
## proof

$$\begin{align*}
\frac{dK}{dt} &= \frac{d}{dt} \left[ \oint_{\Gamma} \vec u \cdot d\vec l \right] \\
&= \underbrace{\oint_{\Gamma} \frac{d\vec u}{dt} \cdot d\vec l }_{I_{1}} + \underbrace{\oint_{\Gamma} \vec u \cdot \frac{d}{dt}(d\vec l)}_{I_{2}}
\end{align*}$$
- considering two nearby points on $\Gamma$

![PX285 - K2 - kelvin's circulation theorem-1.png|500](/img/user/pics/PX285%20-%20K2%20-%20kelvin's%20circulation%20theorem-1.png)

$$\begin{gather}
d\vec l = \vec r_{2} - \vec r_{1} \\
\frac{d}{dt} d\vec l = \frac{d\vec{r_{2}}}{dt} - \frac{d\vec{r_{2}}}{dt} = \vec u_{2} - \vec u_{1} = d\vec u \\\\
\therefore I_{2} = \oint_{\Gamma} \vec u \frac{d}{dt}(\vec l) = \oint_{\Gamma} \vec u \cdot d\vec u \\
= \oint_{\Gamma} d\left(\frac{u^{2}}{2}\right) = 0 \\\\
\therefore I_{2} =0
\end{gather}$$
- the integral vanishes because it is the integral of a perfect differential along a closed path (ie. starting point = end point)

- for $I_{1}$, using the [[content/012/PX285 - hamiltonian mechanics & fluid dynamics/term 2 - fluid dynamics/I - navier-stokes equation/PX285 - I2a - conservation of momentum\|navier-stokes equation]]:
$$\begin{gather}
\frac{d\vec{u}}{dt} = - \frac{1}{\rho} \vec\nabla p + g \vec\nabla z\\
\therefore \frac{dK}{dt} = \oint_{\Gamma} \left( - \frac{\vec\nabla{p}}{\rho} + g\vec\nabla z\right)\cdot d\vec l
\end{gather}$$

- $\vec\nabla z = \vec k$ and:
$$\oint g (\vec\nabla z)\cdot d\vec l = 0$$
- the integral around a closed loop for conservative fields is zero
$$\therefore \frac{dK}{dt} = \oint - \frac{1}{\rho}\vec\nabla p \cdot d\vec l$$
## incompressible
- considering the incompressible limit: $\vec\nabla\cdot\vec u = 0$
$$\frac{dK}{dt} = \frac{1}{\rho} \oint_{\Gamma} (- \vec\nabla p) \cdot d\vec l = - \frac{1}{\rho} \oint_{\Gamma} dp= 0$$
- therefore, $K$ is a constant, or, an **invariant of fluid motion**, and this proves the theorem
## barotropic
- for a barotropic fluid, $\rho = \rho(p)$ only
- eg: adiabatic processes:
$$\frac{p}{\rho^{\gamma}} = \text{ constant} \implies p \propto \rho^{\gamma}$$

- eg: isothermal process: $\gamma = 1$
- applying [[content/012/PX275 - mathematical methods/term 1/E - stoke's theorem and the divergence theorem/PX275 - E1a - stokes' theorem\|stokes' theorem]] and some vector identities:
$$\oint_{\Gamma} - \frac{1}{\rho} (\vec\nabla p)\cdot d\vec l = \iint_{S} \left[\vec\nabla  \times \left(- \frac{\vec\nabla{p}}{\rho}\right)\right] \cdot d\vec S = \iint_{S} \frac{1}{\rho^{2}} [ \vec\nabla \rho \times \vec\nabla p]\cdot d\vec S$$
- for a barotropic fluid, the density gradient is parallel to the pressure gradient:
$$\vec\nabla \rho = \frac{\partial  \rho}{\partial p} \cdot \vec\nabla p$$
$$\therefore \frac{dK}{dt} = \iint_{S} \frac{1}{\rho^{2}} \frac{\partial  \rho}{\partial p}[\vec\nabla p \times \vec\nabla p]\cdot d\vec S = 0$$

- therefore, the theorem is true for an inviscid fluid if it is either incompressible or barotropic
