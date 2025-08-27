---
{"dg-publish":true,"permalink":"/content/012/px-285-hamiltonian-mechanics-and-fluid-dynamics/term-2-fluid-dynamics/i-navier-stokes-equation/px-285-i2b-advective-derivative/","noteIcon":"1","created":"2025-08-27T13:15:24.228+01:00","updated":"2025-01-31T14:02:26.000+00:00"}
---

- in fluid mechanics, capital $D$ is used to denote total derivatives:
$$\frac{D\vec u}{Dt} = \frac{d\vec u}{dt}  = \lim_{\Delta t \to 0} \left[ \frac{\vec u (\vec r(t + \Delta t), t+\Delta t) - \vec u (\vec r(t), t)}{\Delta t}\right]$$

- using the taylor expansion for $\vec u (\vec r(t + \Delta t), t+\Delta t);$
$$\begin{gather}
\frac{D \vec{u}}{D t} \approx \lim_{\Delta t \to 0} \left\{. \frac{1}{\Delta t} \left[ \vec{u}(\vec{r}, t) + \frac{\partial \vec{u}}{\partial x} \Delta x + \frac{\partial \vec{u}}{\partial y} \Delta y + \frac{\partial \vec{u}}{\partial z} \Delta z + \frac{\partial \vec{u}}{\partial t} \Delta t - \vec{u}(\vec{r}, t) \right] \right\} \\
= \frac{\partial \vec{u}}{\partial t} + u_x \frac{\partial \vec{u}}{\partial x} + u_y \frac{\partial \vec{u}}{\partial y} + u_z \frac{\partial \vec{u}}{\partial z} \\
= \frac{\partial \vec u}{\partial t} + (\vec u \cdot \vec\nabla) \vec u
\end{gather}$$
	where, $\lim_{\Delta\to0} [\Delta x(t)/\Delta t] =u_{x}$
- therefore, the **advective derivative**:
$$\frac{d}{dt} = \frac{D}{Dt} = \frac{\partial }{\partial t} + \vec u \cdot \vec\nabla$$
- the first term emphasises the rate of change of fluid property at a fixed point in space
- the second term is for the additional rate of change due to the movement of the fluid element
