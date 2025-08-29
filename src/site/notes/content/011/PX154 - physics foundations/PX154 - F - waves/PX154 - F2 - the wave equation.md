---
{"dg-publish":true,"permalink":"/content/011/px-154-physics-foundations/px-154-f-waves/px-154-f2-the-wave-equation/","noteIcon":"1","created":"2025-08-27T13:14:08.556+01:00","updated":"2024-11-26T23:14:48.000+00:00"}
---

- a fundamental equation, ubiquitous in physics
- the wave function: 
$$u(x,t) = A\cos(kx-\omega t)$$
- differentiating wrt $t$: 
$$\frac{\partial u}{\partial t} = A\omega\sin(kx-\omega t)$$
	- **note**: $\frac{\partial u}{\partial t} \neq v$
- for acceleration: 
$$\begin{align*}
	\frac{\partial^{2} u}{\partial t^{2}} &= -A\omega^{2}\cos(kx-\omega t) \\
	\frac{\partial^{2} u}{\partial t^{2}} &= -\omega^{2} \, u(x,t) \; ...[1]
\end{align*}$$
- differentiating wrt ${} x$: $$\frac{\partial u}{\partial x} = -Ak\sin(kx-\omega t)$$
- again: 
$$\begin{align*}
	\frac{\partial^{2} u}{\partial x^{2}} = -Ak^{2}\sin(kx-\omega t) \\
	\frac{\partial^{2} u}{\partial x^{2}} = -k^{2} \, u(x,t)  \; ...[2]
\end{align*}$$
- from $[1]$ and $[2]$: 
$$\begin{align*}
	\frac{1}{k^{2}} \frac{\partial^{2} u}{\partial x^{2}} &= \frac{1}{\omega^{2}}\frac{\partial^{2} u}{\partial t^{2}} \\
	\frac{\partial^{2} u}{\partial t^{2}} &= \frac{\omega^{2}}{k^{2}}\frac{\partial^{2} u}{\partial x^{2}}
\end{align*}$$
- the wave equation:
$$\frac{\partial^{2} u}{\partial t^{2}} = v^{2} \, \frac{\partial^{2} u}{\partial x^{2}}$$ [YF eqn 15.12]
- ***comments***:
	- applies to right + left travelling waves, and also to standing waves
	- this is in 1D, in 3D: 
$$\frac{\partial^{2} u}{\partial t^{2}} =  v^{2} \, \vec \nabla^{2} u$$
			where: $\vec\nabla^{2}u = (\frac{\partial^{2}}{\partial x^{2}} + \frac{\partial^{2}}{\partial y^{2}} + \frac{\partial^{2}}{\partial z^{2}})u$
- electromagnetic waves: 
$$\frac{\partial^{2} E}{\partial t^{2}} = \frac{1}{\mu_{0}\epsilon_{0}} \, \frac{\partial^{2} E}{\partial x^{2}}$$
		where, $E=$ electric field, $\mu_{0}=$ permeability of free space, $\epsilon_0=$ permittivity of free space
	- we can see here: 
$$c = \frac{1}{\sqrt{\mu_{0}\epsilon_{0}}} = 3\times 10^{8}ms^{-1}$$
	