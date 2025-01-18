---
{"dg-publish":true,"permalink":"/content/012/px-285-hamiltonian-mechanics-and-fluid-dynamics/term-1-hamiltonian-mechanics/f-hamilton-s-equations/px-285-f4-a-gyroscope/","noteIcon":"1","created":"2024-11-25T10:50:32.000+00:00","updated":"2025-01-03T19:38:31.870+00:00"}
---

- considering a spinning top that can rotate on a fixed point
- it has three rotational degrees of freedom: $\theta$, $\alpha$, and $\phi$; but no translational degrees of freedom 

![spinning gyroscope.png|500](/img/user/pics/spinning%20gyroscope.png)

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
- the potential energy: $$V = mgl\cos\theta$$
### kinetic energy
- the axes of rotation for top are represented by:
	$\hat e_{\theta} \perp$ plane of rotation, due to 'wobble'
	$\hat e_{\phi} \sim \hat z$, due to rotation about $z$-axis
	$\hat e_{\alpha} \sim \hat r$, due to spin
- these are not orthogonal

![rotation axes.png|500](/img/user/pics/rotation%20axes.png)

- defining another unit vector, $\hat e_{\phi}'$, such that $\hat e_{\phi}' \perp \hat e_{\theta}$ and ${} \hat e_\alpha {}$
- therefore, $\phi$ rotation is represented by: $\dot\phi \, \hat e_{\phi}$
- taking its projection in the basis $\hat e_{\phi} : \dot\phi \sin\theta \, \hat e_{\phi}'$  

![PX285 - F4 - a gyroscope3.png|500](/img/user/pics/PX285%20-%20F4%20-%20a%20gyroscope3.png)

- the spin frequency: $\dot\omega = \dot\alpha + \dot\phi\cos\theta$ about $\hat e_{\alpha}$
- the theta rotation is represented by: $\dot \theta  \,\hat e_{\theta}$
- therefore the three rotations are:
$$\begin{gather}
	\dot \phi \sin\theta \, \hat e_{\phi}' \,, & (\dot \alpha + \dot \phi \cos\theta)\, \hat e_\alpha \, & \dot\theta \, \hat e_\theta
\end{gather}$$
- hence, the kinetic energy is given by: 
$$T = \frac{1}{2}I\dot\theta^{2} + \frac{1}{2} I (\dot\phi\sin\theta)^{2} + \frac{1}{2}J(\dot\alpha + \dot\phi\cos\theta)^{2}$$
	where, $J$ is the moment of inertia about the axis of the top, and $I$ is that about the 
### the lagrangian
$$L = T - V  = \frac{1}{2}I\dot\theta^{2} + \frac{1}{2} I (\dot\phi\sin\theta)^{2} + \frac{1}{2}J(\dot\alpha + \dot\phi\cos\theta)^{2} - mgl\cos\theta$$
## the euler-lagrange equation
- the euler-lagrange equation: 
$$\frac{\partial L}{\partial q_{i}} = \frac{d}{dt} \frac{\partial L}{\partial \dot q_{i}}$$
- there will be three equations:
	$q_{1}= \theta$
	$q_{2}= \phi$
	$q_{3} = \alpha$
- there will two rotational symmetries as $L$ does not depend on ${} \phi$ or $\alpha$
- looking at $\phi$ and $\alpha$ equations first, anticipating the emergence of two conserved momenta: 
$$\begin{gather*}
	\frac{\partial L}{\partial \phi} = 0 = \frac{d}{dt}p_{\phi} \\
	p_{\phi} = \frac{\partial L}{\partial \dot\phi} = I \sin^{2}\theta + J \cos\theta (\dot \alpha + \dot \phi \cos\theta) = constant \\
\end{gather*}$$
$$\begin{gather*}
	\frac{\partial L}{\partial \alpha} = 0 = \frac{d}{dt}p_{\alpha} \\
	p_{\alpha} = \frac{\partial L}{\partial \dot\alpha} = J (\dot\alpha + \dot\phi \cos\theta) = constant \\
\end{gather*}$$
$$\implies p_{\phi}= I\sin^{2}\theta \,\dot\phi + \cos\theta\,p_{\alpha}= constant \tag{1}$$
- considering the $\theta$ equation:
$$\frac{\partial L}{\partial \theta} = I\sin\theta\cos\theta\,\dot\phi^{2} - J\dot\phi\sin\theta (\dot\alpha + \dot\phi \cos\theta) + mgl\sin\theta$$
$$\frac{d}{dt} \frac{\partial L}{\partial \dot \theta} = \frac{d}{dt}I\dot \theta = I \ddot \theta$$
$$\begin{align*}
	I\ddot\theta &= I\sin\theta\cos\theta\,\dot\phi^{2} - J\dot\phi\sin\theta (\dot\alpha + \dot\phi \cos\theta) + mgl\sin\theta \\
	&= I\sin\theta\cos\theta\,\dot\phi^{2} - \dot\phi\sin\theta p_\alpha + mgl\sin\theta \\
\end{align*}$$
- from equation ${} (1): {}$
$$\dot \phi = \frac{p_{\phi}-cos\theta p_{\alpha}}{I\sin^{2}\theta}$$
$$\begin{align}	I\ddot\theta &=I\sin\theta\cos\theta\,\left(\frac{p_{\phi}-cos\theta p_{\alpha}}{I\sin^{2}\theta}\right)^{2}  \\ 
&-  p_{\alpha}\sin\theta \left(\frac{p_{\phi}-cos\theta p_{\alpha}}{I\sin^{2}\theta}\right) + mgl\sin\theta \\
&= F(\theta) 
\end{align}$$
- this is a second order ODE that can be solved numerically
