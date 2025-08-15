---
{"dg-publish":true,"permalink":"/content/012/px-285-hamiltonian-mechanics-and-fluid-dynamics/term-2-fluid-dynamics/l-potential-flows/px-285-l2-potential-dipole/","noteIcon":"1","created":"2025-02-20T14:09:20.894+00:00","updated":"2025-06-09T10:31:20.962+01:00"}
---

- let $\phi = a\cos\theta/r$ in cylindrical coordinates
- the components of u:
$$\begin{gather}
u_{r} = \frac{\partial \phi}{\partial r} = - \frac{a\cos\theta}{r^{2}} \\
u_{\theta} = \frac{\partial \phi}{\partial \theta} = - \frac{a\sin\theta}{r} \\
u_{z} = \frac{\partial \phi}{\partial z} = 0
\end{gather}$$
$$\vec\nabla\cdot\vec u = \frac{a\cos\theta}{r^{2}}- \frac{a\cos\theta}{r^{3}}= 0$$
- this means it is incompressible

![PX285 - K4 - potential dipole.png|500](/img/user/pics/PX285%20-%20K4%20-%20potential%20dipole.png)

- for time dependent irrotational flows: $\vec\nabla \times \vec u = 0$
- the vector identity:
$$(\vec u \cdot \vec\nabla ) \vec u = \frac{1}{2} \vec\nabla u^{2} - \vec u (\vec\nabla \times \vec u) = \frac{1}{2} \vec\nabla u^{2}$$
- the euler equation becomes:
$$\frac{\partial \vec u}{\partial t} + \frac{1}{2} \vec\nabla u^{2} = \vec\nabla \left(\dot\phi + \frac{u^{2}}{2}\right) = -g\hat z - \frac{1}{\rho} \vec\nabla p$$
$$\vec\nabla \left(\dot\phi + \frac{u^{2}}{2} + gz + \frac{p}{\rho}\right) =0 \implies \dot\phi + \frac{u^{2}}{2} + gz + \frac{p}{\rho} = \text{constant}$$

- this is generalized bernoulli's principle
- here, $\vec u$ is incompressible, irrotational and inviscid

 - eg: gravity waves (different from gravitational waves)

 ![PX285 - K4 - potential dipole-1.png|500](/img/user/pics/PX285%20-%20K4%20-%20potential%20dipole-1.png)

  - considering flows that satisfy laplace's equation: $\nabla^{2}\phi = 0$
  - also, the boundary conditions: $u_{z}(z=0)=0$
  - collision on free surface ($z \simeq d$)
  - let $\phi(x,z) = f(x)g(z)$
  $$\nabla^{2} \phi =\frac{f''_{xx}}{f} + \frac{g''_{zz}}{g} = 0 \implies \frac{f''_{xx}}{f} = \frac{-g''_{xx}}{g} = -k^{2} $$
  $$\begin{gather}
  f''_{xx} + k^{2}f  = 0 \implies  f = A_{1}\cos kx + B_{1}\sin kx \\
  g''_{zz} - k^{2}g  = 0 \implies  g = A_{2}e^{-kz} + B_{2} e^{kz}\\
\end{gather}$$

- considering a propagating wave:
$$\phi = \phi_{0} \cos(kx - \omega t)(e^{kz} + Be^{-kz})$$
$$\begin{gather}
u_{x} = \frac{\partial \phi}{\partial x} = -k \phi_{0} \sin(kx-\omega t) (e^{kz} + Be^{-kz}) \\
u_{z} = \frac{\partial \phi}{\partial z} = k \phi_{0} \cos(kx - \omega t) (e^{kz} - Be^{-kz}) \\
u_{z}(z = 0) = 0 \implies 1-B = 0 \implies B = 1
\end{gather}$$
- considering waves of small amplitude (amplitude of displacement $\ll 2\pi/k$, the wavelength)
- the displacement of the fluid element by wave
$$\begin{gather}
X(t) = \int u_{x}\, dt = - \frac{k\phi_{0}}{\omega} \cos(kx - \omega t) (e^{kz}+ e^{-kz})+ X_{0} \\ 
Z(t) = \int u_{z}\, dt = - \frac{k\phi_{0}}{\omega} \sin(kx - \omega t) (e^{kz} - e^{-kz})+ Z_{0} \\
\implies \frac{(X(t)-X_{0})^{2}}{a(z)} + \frac{(Z(t)-Z_{0})^{2}}{b(z)} = 1
\end{gather}$$
- $(X(t), Z(t))$ gives the coordinates of fluid elements which was $(X_{0}, Z_{0})$

$$\begin{gather}
a(z) =  \left[- \frac{k\phi}{\omega} (e^{kz}+ e^{-kz})\right]^{2} \\
b(z) =  \left[- \frac{k\phi}{\omega} (e^{kz}-  e^{-kz})\right]^{2} 
\end{gather}$$
- the path of a fluid element in the wave is an ellipse
- the 'aspect ratios' of the ellipse depends upon $a$ via $a(z)$ and $b(z)$

- considering the trajectory of fluid element near the surface, $z \simeq d$
- let $kd \gg 1 \implies d \gg \lambda$, ie. 'deep water approximation'
$$\begin{gather}
e^{kd} + e^{-kd} \simeq e^{kd} \\
e^{kd} -  e^{-kd} \simeq e^{kd} \\
\implies a(z) \simeq b(z)
\end{gather}$$
- so, the trajectory is a circle

- at $z = 0:$
$$\begin{gather}
e^{k0}+ e^{-k0} = 2 \\
e^{k0} - e^{-k0} = 0 \\
\implies a(0) \gg b(0)
\end{gather}$$
- this is a piece of straight line

![PX285 - K4 - potential dipole-3.png|500](/img/user/pics/PX285%20-%20K4%20-%20potential%20dipole-3.png)

- to determine the boundary condition at the free surface, $z \simeq d$, using the generalized bernoulli's principle:
$$\dot \phi + \frac{P_{atm}}{\rho} + gz + \frac{u^{2}}{z} = \text{constant}$$
- considering waves of very low amplitude the governing equations can be linearized
- $u^{2}/2$ can be neglected with respect to $\dot \phi$, as $u^{2}/2 \sim \phi_{0}^{2}$, and $\dot \phi \sim \phi_{0}$
$$\dot \phi(t)+ gz(t)  + \frac{P_{atm}}{\rho}  = \text{constant} \implies \dot \phi(t)+ gz(t) = \text{constant}$$
- let the constant be zero
$$\begin{gather}
\omega\phi_{0} \sin (kx -\omega t) (e^{kd}+e^{-kd}) + g\left[- \frac{k\phi_{0}}{\omega} \sin(kx - \omega t) (e^{kd} - e^{-kd})\right]= 0 \\
\omega^{2} = gk  \frac{e^{kd}-e^{-kd}}{e^{kd}+e^{-kd}} = gk\tanh(kd)
\end{gather}$$
- this is the dispersion relation for surface waves
- $\omega(k)$ is independent of the amplitude, $\phi_0$, because of linear approximation

- considering two limiting cases:
- firstly, let $kd \ll 1 \implies d\ll \lambda$, ie. 'shallow water limit', eg: tsunami waves
$$\begin{gather}
\lim_{kd\to0} \tanh(kd) \to kd \implies \omega \to \sqrt{gh}k \\
v_{p} = \frac{\omega}{k} = \sqrt{gh} \\
v_{g} = \frac{d\omega}{dk} = \sqrt{gk}
\end{gather}$$
- this is called a **'dispersion-less wave'**

- secondly, $kd\gg 1 \implies d \gg \lambda$, ie. 'deep water limit'
$$\begin{gather}
\lim_{kd} \tanh(kd) = 1 \\
\omega = \sqrt{gk} \\
v_{p} = \frac{\omega}{k} = \sqrt{\frac{g}{k}} \sim \lambda^{1/2}\\
v_{g} = \frac{d\omega}{dk} = \frac{1}{2}\sqrt{\frac{g}{k}}
\end{gather}$$
- this is a **dispersive wave** 
 