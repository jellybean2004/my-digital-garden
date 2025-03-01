---
{"dg-publish":true,"permalink":"/content/012/px-285-hamiltonian-mechanics-and-fluid-dynamics/term-2-fluid-dynamics/l-potential-flows/px-285-l1-potential-flows/","noteIcon":"1","created":"2025-02-14T12:06:40.234+00:00","updated":"2025-03-01T12:17:27.642+00:00"}
---

- considering a flow that is irrotational, ie: $\vec\nabla \times \vec u = 0$, and incompressible, ie: $\vec\nabla\cdot\vec u = 0$
- $\vec u=\vec\nabla \phi$, where $\phi$ is the scalar potential 
$$\begin{gather}
\vec\nabla \times (\vec\nabla \phi) = 0 \\\\
\vec\nabla\cdot( \vec\nabla\cdot\phi) = \nabla^{2} \phi = 0 \\
\end{gather}$$
- the flow is described by a scalar, and the solutions to the laplacian can be added to give a more complex solution
## uniform flow
- considering $\vec u = v \hat i$
- by symmetry:
$$\begin{gather}
\vec u = \vec\nabla \phi = \frac{\partial \phi}{\partial x} \\
\implies \phi = ux +c
\end{gather}$$

- equipotential lines are lines of constant $\phi$, which are locally perpendicular to the stream lines
- in 3D, equipotential surfaces

![PX285 - K3 - potential flows.png|500](/img/user/pics/PX285%20-%20K3%20-%20potential%20flows.png)

## 2D point source
- considering a 2D point source velocity in cylindrical coordinates:
$$\vec u = \frac{q}{2\pi r} \hat r$$
- checking for rotation:
$$\vec\nabla \times \vec u = \frac{1}{r} \begin{vmatrix}\hat r & r\hat\theta & \hat z \\ \frac{\partial}{\partial r} & \frac{\partial }{\partial \theta} & \frac{\partial }{\partial z} \\ u_{r} & ru_{\theta} & u_{z} \end{vmatrix} = 0$$
- checking for incompressibility:
$$\vec\nabla\cdot\vec u = \frac{1}{r} \frac{\partial ru_{r}}{\partial r} + 0 = \frac{1}{r} \left(\frac{q}{2\pi r} - r \frac{\partial }{\partial r}\left(\frac{q}{2\pi r^{2}}\right)\right)  = 0$$
- since the flow is incompressible and irrotational, $\vec u = \vec\nabla \phi:$
$$\begin{gather}
\vec\nabla \phi = \frac{q}{2\pi r}\hat r = \frac{\partial \phi}{\partial r} \hat r = \frac{q}{2\pi r}\\
\implies \phi = \frac{1}{2\pi} \ln(r) + c = \frac{1}{4\pi} \ln(r^{2}) +c \\
\therefore \phi= \frac{1}{4\pi}\ln(x^{2}+y^{2})+c
\end{gather}$$

![PX285 - K3 - potential flows-1.png|500](/img/user/pics/PX285%20-%20K3%20-%20potential%20flows-1.png)

## tornado/free vortex
- this is a flow with circular paths around an axis
- considering $\vec u = u_{\theta}(r) \hat \theta$
- it is irrotational as $\vec\nabla\times \vec u = 0$
$$\implies \frac{1}{r} \frac{\partial (ru_{\theta})}{\partial r} = 0$$
- this means that $ru_\theta$ must be constant
- it is only possible for:
$$u_{\theta} = \frac{K}{2\pi} \frac{1}{r}$$
- for $r\to0$, $u_\theta\to\infty$, which would be impossible
- therefore, near $r=0$, viscosity must be accounted for
- therefore the potential flow model works for $r > \delta$

![PX285 - K3 - potential flows-2.png|500](/img/user/pics/PX285%20-%20K3%20-%20potential%20flows-2.png)

- calculating the circulation around the axis:
$$\oint_{\Gamma} \vec u \cdot d\vec l = \int_{0}^{2\pi} u_{\theta} r\,d\theta = \frac{K}{2\pi} \int_{0}^{2\pi} \frac{r}{r}d\rho  = K$$
- therefore, ${} K$ is the circulation around the axis
- generally, ${} K \neq 0$ if $\Gamma$ is around $r=0$, ie. the axis
- from [[content/012/PX285 - hamiltonian mechanics & fluid dynamics/term 2 - fluid dynamics/K - circulation and vorticity/PX285 - K2 - kelvin's circulation theorem\|kelvin's circulation theorem]], $K = 0$ if $\Gamma$ is not around the axis

- the potential:
$$u_{\theta}(r) = \frac{1}{r} \frac{\partial \phi}{\partial \theta} \implies \frac{K}{2\pi r} = \frac{1}{r} \frac{d\phi}{d\theta} \implies \phi = \frac{K}{2\pi} \theta +c$$

![PX285 - K3 - potential flows-3.png|500](/img/user/pics/PX285%20-%20K3%20-%20potential%20flows-3.png)

- the density is constant as it is incompressible
- the pressure: at $r\to\infty$, $\vec u \to 0$, $p = p_{atm}$

- using the [[content/012/PX285 - hamiltonian mechanics & fluid dynamics/term 2 - fluid dynamics/I - navier-stokes equation/I - navier-stokes equation\|navier-stokes equation]] in euler form as it is inviscid, considering a stationary case, ie: $\partial_{t} = 0$
- $g$ is also neglected
$$\begin{gather}
\rho[(\vec u \cdot \vec\nabla)\vec u]_{r} = - \frac{\partial p}{\partial r} \\
-\rho \frac{u_{\theta}^{2}}{r} = - \frac{dp}{dr} \\
- \frac{\rho K^{2}}{4\pi^{2}} \int \frac{1}{r^{3}}\, dr = - \int dp \\
\therefore p = - \frac{K^{2}\rho^{2}}{8\pi r^{2}} 
\end{gather}$$
- as $p(r = \infty) = p_{atm}:$
$$p = p_{atm}- \frac{K^{2}\rho^{2}}{8\pi r^{2}}$$
- ie. $p$ decreases towards the tornado
