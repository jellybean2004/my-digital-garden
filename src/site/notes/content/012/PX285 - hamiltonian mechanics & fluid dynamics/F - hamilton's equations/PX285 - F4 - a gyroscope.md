---
{"dg-publish":true,"permalink":"/content/012/px-285-hamiltonian-mechanics-and-fluid-dynamics/f-hamilton-s-equations/px-285-f4-a-gyroscope/","created":"2024-11-25T10:50:32.000+00:00","updated":"2024-11-26T12:59:40.749+00:00"}
---

- considering a spinning top that can rotate on a fixed point
- it has three rotational degrees of freedom: $\theta$, $\alpha$, and $\phi$; but no translational degrees of freedom 
![Pasted image 20241115190518.png](/img/user/pics/Pasted%20image%2020241115190518.png)
- **reminder:** for a uniform rod of length, $l$, spinning about its centre of mass with an angular frequency, $\omega$, the kinetic energy is given by: 
$$T = \frac{1}{2}I\omega^{2}$$
	where, $I=ml^{2}$ is the moment of inertia

- the gyroscope has two moments of inertia, $I$ and $J$
- the normal is the top symmetry axis
- if the top is spinning at at angle to the normal, the moment of inertia is $I$
- if it is spinning about the normal, then it is $J$
## determining the lagrangian
### potential energy
- suppose $l$ is the distance from the base to the centre of mass of the top, and $\theta$ is the angle with the normal
![Pasted image 20241115195808.png](/img/user/pics/Pasted%20image%2020241115195808.png)
- the potential energy: $$V = mgl\cos\theta$$
### kinetic energy
![Pasted image 20241115200711.png](/img/user/pics/Pasted%20image%2020241115200711.png)
- axes of rotation for top are represented by:
	$\hat e_{\theta} \perp x-y$ plane
	$\hat e_{\phi} \sim \hat z$
	$\hat e_{\alpha} \sim \hat r$
- these are not orthogonal
- suppose $\hat e_{\phi}' \perp \hat e_{\theta}$
- $\phi$ rotation is represented by: ${} \dot\phi \hat e_{\phi}' {}$
- the spin frequency: $\dot\omega = \dot\alpha + \dot\beta\cos\theta$
- $\dot\phi\sin\theta \hat e_{\phi}'$ 
- hence, the kinetic energy is given by: 
$$T = \frac{1}{2}I\dot\theta^{2} + \frac{1}{2} I (\dot\phi\sin\theta)^{2} + \frac{1}{2}J(\dot\alpha + \dot\phi\cos\theta)^{2}$$
## the lagrangian
$$\begin{align*}
	L &= T - V \\
	&= \frac{1}{2}I\dot\theta^{2} + \frac{1}{2} I (\dot\phi\sin\theta)^{2} + \frac{1}{2}J(\dot\alpha + \dot\phi\cos\theta)^{2} - mgl\cos\theta \\
	&= 
\end{align*}$$
- the euler-lagrange equation: 
$$\frac{\partial L}{\partial q_{i}} = \frac{d}{dt} \frac{\partial L}{\partial \dot q_{i}}$$
- $\frac{d}{dt}\frac{\partial L}{\partial \dot q_{i}}$ is the generalized momentum
- there will be three equations
- there are two rotational symmetries as $L$ does not depend on ${} \phi$ or $\alpha$
- looking at $\phi$ and $\alpha$ equations first, anticipating the emergence of two conserved momenta: 
$$\begin{align*}
	\frac{\partial L}{\partial \phi} = 0 &= \frac{d}{dt}p_{\phi} \\
	p_{\phi} = \frac{\partial L}{\partial \dot\phi} &= I \sin^{2}\theta + J \cos\theta (\dot \alpha + \dot \phi \cos\theta) \\
\end{align*}$$
- #incomplete 