---
{"dg-publish":true,"permalink":"/content/012/px-285-hamiltonian-mechanics-and-fluid-dynamics/c-calculus-of-variations/px-285-c4-simple-pendulum/","created":"2024-11-25T10:50:32.000+00:00","updated":"2024-11-26T13:00:18.343+00:00"}
---

- consider a simple pendulum bearing a mass, $m$, at the end of a string of length, $l$, inclined at an angle, $\theta$, to the vertical
- the kinetic energy: 
$$T = \frac{1}{2}I\dot \theta^{2}= \frac{1}{2}ml^{2}\dot\theta^{2}$$
	where, $I$ is the moment of inertia of the pendulum about the pivot
- the potential energy: 
$$V = -mgl\cos\theta$$
- applying the euler-lagrange equation: 
$$\begin{align*}
	-(mgl\sin\theta+ ml^{2}\ddot\theta) &= 0 \\
	-\frac{g}{l}\sin\theta &= \ddot\theta
\end{align*}$$
- let, $\omega^{2}= \frac{-g}{l}$, and using the small angle approximation: 
$$\ddot\theta \approx -\omega^{2}\theta$$
- this is a simple harmonic relation, where $\omega= \sqrt {\frac{g}{l}}$ is the angular frequency
- the solution is in the form: 
$$\theta(t) = A\sin(\omega t+\phi)$$
	where, $A$ and $\phi$ are arbitrary amplitude and phase difference respectively, which can be determined given two boundary conditions
