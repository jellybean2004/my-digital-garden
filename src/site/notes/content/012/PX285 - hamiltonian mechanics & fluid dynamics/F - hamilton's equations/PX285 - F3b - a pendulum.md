---
{"dg-publish":true,"permalink":"/content/012/px-285-hamiltonian-mechanics-and-fluid-dynamics/f-hamilton-s-equations/px-285-f3b-a-pendulum/","created":"2024-11-25T10:50:32.000+00:00","updated":"2024-11-26T12:59:39.399+00:00"}
---

- considering a simple pendulum of length, $l$, and $\theta$ is the angle between the pendulum and the equilibrium position at a given time
- writing down the lagrangian, $L$, and using it to calculate the hamiltonian, $H$ and identifying the momentum: 
$$\begin{align*}
	T &= \frac{1}{2}I\dot\theta^{2} \\
	\frac{1}{2}mv^{2} &= \frac{1}{2}ml^{2} \dot\theta^{2} \\
	\implies v &= l\dot\theta \\\\
	V &= -mgl\cos\theta \\\\
	\therefore L &= \frac{1}{2}ml^{2} \dot\theta^{2} + mgl\cos\theta \\\\
	p &= \frac{\partial L}{\partial \dot\theta} = ml^{2}\dot\theta \tag{1}
\end{align*}$$
- **note:** here, $p \neq mv$ because this is the angular momentum
- the definition of $H$ from first principles: 
$$H = - L + p \dot\theta = - L + ml^{2}\dot\theta^{2}$$
- substituting for $L:$ 
$$H = \frac{1}{2}ml^{2} \dot\theta^{2} - mgl\cos\theta$$
- substituting using $(1):$ 
$$H(\theta, p) = \frac{1}{2}ml^{2}\left(\frac{p}{ml^{2}}\right)^{2} - mgl\cos\theta = \frac{p^{2}}{2ml^{2}} - mgl\cos\theta$$
- using hamilton's equations: 
$$\begin{align*}
	\dot\theta &= \frac{p}{ml^{2}}\tag{2} \\
	\dot p &= -mgl\sin\theta \tag{3}
\end{align*}$$
- if $\theta<<1:$ 
$$\dot p \approx -mgl\theta$$ 
- on phase plane: 
$$\begin{align*}
	d\theta &= \frac{p}{ml^{2}} \,dt \\
	dp &= -mgl\sin\theta\,dt
\end{align*}$$

- deriving the equations of motion: 
$$\ddot\theta = \frac{\dot{p}}{ml^{2}} = \frac{-mgl}{ml^{2}} \sin\theta = - \omega^{2}\sin\theta$$
	where, $\omega = \sqrt{\frac{g}{l}}$
- for $\theta<<1:$ 
$$\ddot \theta \approx - \omega^{2}\theta$$
- this is SHM with solutions: 
$$\theta = A\cos(\omega t + \phi) = A\cos\psi$$
$$\implies p = ml^{2}\dot\theta = - Aml^{2} \omega \sin(\omega t + \phi)$$
- defining $\tilde p$ as: 
$$\tilde p = \frac{p}{ml^{2}\omega} = -A\sin\psi$$
![Pasted image 20241114200847.png](/img/user/pics/Pasted%20image%2020241114200847.png)
- a circular trajectory on the $\tilde p - \theta$ plane with clockwise rotation
- an elliptical trajectory on the $p-\theta$ plane
- the slope: 
$$\frac{dp}{d\theta} = \frac{dp}{dt} \frac{dt}{d\theta} = \frac{\dot p}{\dot\theta} = - \frac{mgl\sin\theta}{\frac{p}{ml^{2}}} = \frac{m^{2}l^{3}g\sin\theta}{p}$$
- the slope is negative
- if pendulum oscillates back and forth: $E<E^{*} = 2mgl$, $-\theta_{max} < \theta < \theta_{max}$, $\theta_{max}<\pi$
- if $\theta = \pm \theta_{max}: p=0$
![Pasted image 20241114201640.png](/img/user/pics/Pasted%20image%2020241114201640.png)
- if ${} E>E^{*} = 2mgl: {}$ no restriction on $\theta$, $\theta=\pm\pi : p>0:$ 
$$\frac{dp}{dt}\propto \frac{\sin\theta}{p} \to 0$$
![Pasted image 20241114201915.png](/img/user/pics/Pasted%20image%2020241114201915.png)
- if $E=E^{*}$, the pendulum can come to rest at $\theta=\pm\pi$
- let, $\theta = \pi - \epsilon:$ 
$$\dot\theta = -\dot\epsilon = \frac{p}{ml^{2}}$$
- in the late stages, $\epsilon<<1:$ 
$$\dot p = -mgl\epsilon$$
$$\ddot \epsilon = - \frac{1}{ml^{2}}\dot p = \frac{mgl}{ml^{2}}\epsilon = \omega^{2}\epsilon$$
- note: this is **not** SHM as there is a $'+'$, not $'-'$
- the solution: 
$$\epsilon = A e^{\omega t} + B e^{-\omega t}$$
- the first term is diverging from upright, while the second is converging to it
- here,  $\epsilon$ is getting smaller: 
$$\epsilon = Be^{-\omega t}$$
![Pasted image 20241114202555.png](/img/user/pics/Pasted%20image%2020241114202555.png)
- seeking a expression for $\frac{dp}{d\theta}:$ 
$$\begin{align*}
	\frac{dp}{dt}&= -mgl\epsilon = -mgl\,Be^{-\omega t} \\
	\frac{d\theta}{dt} &= - \dot\epsilon = B\omega e^{-\omega t}\\
	\therefore \frac{dp}{d\theta} &= - \frac{mgl}{\omega}
\end{align*}$$
- the gradient is a non-zero negative constant
## disconnected trajectories
![Pasted image 20241114204550.png](/img/user/pics/Pasted%20image%2020241114204550.png)
- not all statues of a given energy are necessarily accessible, this is called breaking of **ergodicity**
- **ergodic** systems explore all sates consistent with energy conservation

- considering a rollercoaster in a 'mexican hat' potential, where, $E^{*} = mgh^{*}$
![Pasted image 20241114204837.png](/img/user/pics/Pasted%20image%2020241114204837.png)
- for $E>E^{*}$
![Pasted image 20241114204905.png](/img/user/pics/Pasted%20image%2020241114204905.png)
- this is **ergodic** as it can explore all states consistent with energy, $E$
