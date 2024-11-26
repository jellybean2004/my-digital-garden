---
dg-publish: true
---

- considering a particle moving freely in $d=1$ dimension
- the hamiltonian: 
$$H = T + V = \frac{1}{2m}p^{2} + V(x)$$
- using hamilton's equations: 
$$\begin{align*}
	\dot x = \frac{\partial H}{\partial p} &= \frac{p}{m} \\
	\implies  dx &= \frac{p}{m}\,dt \\\\
	\dot p  = - \frac{\partial H}{\partial x} &= - \frac{\partial V}{\partial x} =F \\
	\implies dp &= F\,dt
\end{align*}$$
## example 1
- for a constant $V$, ${} \frac{dp}{dt} = F = -\frac{\partial V}{\partial x} {}$, so $p$ is constant
![Pasted image 20241114193531.png](/img/user/pics/Pasted%20image%2020241114193531.png)

## example 2
- considering a particle attached to a string with a spring constant, $k$, so the potential, $V = \frac{1}{2}kx^{2}:$ 
- from hamilton's equations: 
$$\begin{align*}
	\dot x &= \frac{p}{m}  \implies dx = \frac{p}{m}dt\\
	\dot p &= -\frac{\partial V}{\partial x} \implies dp = -kx\,dt
\end{align*}$$
![Pasted image 20241108154139.png](/img/user/pics/Pasted%20image%2020241108154139.png)
### flow on the phase plane
- more mathematically: 
$$\frac{d}{dt}\dot x = \frac{d}{dt} \left(\frac{p}{m}\right) \implies \ddot x = \frac{1}{m}\dot p = -\frac{k}{m}x$$
- this is the equation of a simple harmonic motion with $\omega^{2} = \frac{k}{m}$, and solutions: 
$$x(t) = A \cos(\omega t + \phi)$$
- similarly, 
$$\ddot p = -k\dot x = - \frac{k}{m}p \implies p (t) = B\sin(\omega t + \phi)$$
