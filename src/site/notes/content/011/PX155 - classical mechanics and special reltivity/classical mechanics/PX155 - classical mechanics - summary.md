---
{"dg-publish":true,"permalink":"/content/011/px-155-classical-mechanics-and-special-reltivity/classical-mechanics/px-155-classical-mechanics-summary/","created":"2024-10-01T18:50:56.711+01:00","updated":"2024-11-26T19:57:38.897+00:00"}
---

# [[content/011/PX155 - classical mechanics and special reltivity/classical mechanics/PX155 - A - foundations of classical mechanics/A - foundations of classical mechanics\|A - foundations of classical mechanics]]
## newton's laws
### first law
- law of inertia
- "every body continues in its state of rest or uniform motion unless acted on by an external force"
### second law
- "the rate of change of momentum of a body is equal to the total external force acting upon it"
$$F = \frac{dp}{dt}$$
- if mass is constant:
$$F = ma$$
### third law
- "to every action there is an equal and opposite reaction"
## friction
### static friction
$$F_{s,\,max} = \mu_{s}N$$
### kinetic friction
$$F_{k} = \mu_{k}N$$
## gravitation
### newton's law of gravity
$$\vec F_{12} = - \frac{Gm_{1}m_{2}}{r^{2}}\hat r$$
### newton's shell theorem
- force on a mass outside the shell due to the shell is as if it is due to a point mass at the shell's centre
- force on a mass inside the shell is zero as the net force is zero
# [[content/011/PX155 - classical mechanics and special reltivity/classical mechanics/PX155 - B - systems of particles, accelerations/B - systems of particles and acceleration\|B - systems of particles and acceleration]]
## centre of mass
$$\vec r_{cm}= \frac{\int\vec r\,dm}{\int dm} \;;\; \int\vec r\,dm = \left(\int x\,dm,\int y\,dm,\int z\,dm\right)$$
## equations of motion
### constant acceleration
$$a= \frac{dv'}{dt'} : a
\int_{0}^{t}dt' = \int_{u}^{v}dv'  \implies at = v-u$$
$$v = \frac{dx'}{dt'}: \int_{0}^{t} (u+at) dt' = \int_{0}^{s}dx'  \implies s=ut+ \frac{1}{2}at^{2}$$
$$v^{2}-u^{2}= 2as$$
### time-dependent acceleration
$$\int_{0}^{t} a(t)\,dt' = \int_{u}^{v}dv'$$
### position-dependent acceleration
$$\begin{align*}
	a(x) = \frac{dv'}{dt'} &= \frac{dv'}{dx'} \frac{dx'}{dt'} \\
	\int_{0}^{s} a(x)\,dx' &= \int_{u}^{v}v\,dv' \\
	&= \frac{1}{2}(v^{2}-u^{2}) 
\end{align*}$$
## velocity-dependent acceleration
$$a(v) = \frac{dv'}{dt'} \implies \int_{u}^{v} \frac{1}{a(v)} \,dv' = t$$
# [[content/011/PX155 - classical mechanics and special reltivity/classical mechanics/PX155 - C - work and energy/C - work and energy\|C - work and energy]]
## kinetic energy
$$KE = \frac{1}{2}mv^{2}$$
$$W = \int_{a}^{b} \vec F\,d\vec x$$
## conservative forces
- conservative if work done is independent of the path
$$\oint \vec F\,d\vec r = 0$$
$$W = -\Delta U \implies \Delta KE + \Delta U = 0$$
$$\vec F = -\vec\nabla U$$
## gravitational potential energy
$$W_{a\to b} = -GMm \left(\frac{1}{b} - \frac{1}{a}\right)$$
$$\Delta U = - W$$
- considering ${} U_{\infty} = 0,\; a=\infty,\; b=r: {}$
$$U(r) = - \frac{GMm}{r}$$
- gravitational potential:
$$\phi = \frac{U}{m} = \frac{GM}{r}$$
## power
$$P = \frac{dW}{dt} = \vec F\cdot \frac{d\vec r}{dt} = \vec F\cdot \vec v$$
# D - simple harmonic moton
## general equation
$$\begin{align*}
	F = ma &= -kx \\
	\ddot x + \omega^{2}x &= 0 \;;\; \omega = \sqrt{\frac{k}{m}}
\end{align*}$$
$$\therefore x = A\cos\omega t + B\sin\omega t$$
- angular velocity:
$$\omega = \frac{\theta}{t}$$
$$\therefore x = A\cos\theta + B\sin\theta$$
$$x = A' \cos(\omega t + \phi)$$
	where, $A'=$ amplitude, $\phi=$phase angle
## energy
$$W = \frac{1}{2}kx^{2} \;:\; U = \frac{1}{2}kA^{2}\cos(\omega t)$$
$$KE = \frac{1}{2}m\dot x^{2} = \frac{1}{2}kA^{2}\sin^{2}(\omega t)$$
$$E_{tot} = \frac{1}{2}kA^{2}$$
## complex form
$$x = \mathbb Re (A'e^{i\theta} e^{i\phi}) = \mathbb Re(a e^{i\omega t})$$
	where, $a=A'e^{i\phi}=$ complex amplitude
	$$\ddot z + \omega^{2} z = 0$$
## damped oscillations
$$\begin{align*}
	m\ddot x + b\dot x + kx &= 0 \\
	\ddot x + \gamma\dot x + \omega^{2}x &= 0
\end{align*}$$
	where, $b=$ damping coefficient, $\gamma=\frac{b}{m}$
	$$\ddot z + \gamma \dot z + \omega^{2}z =0$$
	$$\lambda = - \frac{\gamma}{2}\pm \sqrt{\left(\frac{\gamma}{2}\right)^{2}-\omega^{2}}$$
![Pasted image 20231113085521.png](/img/user/pics/Pasted%20image%2020231113085521.png)
### light daming
$$\gamma< 2\omega: \lambda = - \frac{\gamma}{2}\pm i\omega'\;,\; \omega' = \sqrt{\omega^{2}-\left(\frac{\gamma}{2}\right)^{2}}$$
### heavy damping
$$\gamma> 2\omega: \lambda = - \frac{\gamma}{2}\pm \omega'\;,\; \omega' = \sqrt{\omega^{2}-\left(\frac{\gamma}{2}\right)^{2}}$$
### critical damping
$$\gamma= 2\omega: \lambda = - \frac{\gamma}{2}$$
## driven damped oscillations
$$\begin{align*}
	m\ddot x + b\dot x + kx &= F_{0}\cos(\omega t) \\
	\ddot z + \gamma\dot z + \omega_{0}^{2}z &= \frac{F_{0}}{m}e^{i\omega t}
\end{align*}$$
- trying $z = ae^{i\omega t}:$
$$a = \frac{F}{m ((\omega_{0}^{2}-\omega^{2})+i\omega\gamma)} = |a|e^{i\phi}$$
$$|a| = \frac{F}{m \sqrt{(\omega_{0}^{2}-\omega^{2})^{2}- (\omega\gamma)^{2}}} \;;\; \tan \phi = - \frac{\gamma\omega}{\omega^{2}_{0}-\omega^{2}}$$
# E - circular motion, rotation of bodies
## circular motion
### angular velocity ($\omega$)
$$\omega = \dot \theta = \frac{2\pi}{T}$$
$$\vec v = \vec\omega \times \vec r$$
### centripetal acceleration
$$a = \omega v = \omega^{2}r = v^{2}r$$
$$\vec a = a\,\hat r$$
### moments
$$moment = F\,d_{\perp}$$
- for a system in equilibrium, sum of moments about a point is zero
### torque (${} \tau {}$)
$$\vec\tau = \vec r \times \vec F$$
### angular momentum
$$\vec\tau = \frac{d\vec{L}}{dt}$$
- for a particle moving in a straight line, $\vec L$ along any point not along the straight line $=0$
- for a lever to balance, about the fulcrum, $\vec\tau = \frac{d\vec L}{dt} =0$

- for a moving particle:
$$\begin{gather*}
	\vec L = \vec r \times \vec p = r \times m\vec v \\
	|\vec L| = mr^{2}\omega
\end{gather*}$$
#### orbital angular momentum
- for a satellite of mass, $m$, orbiting earth at a distance, $R$, from the centre of earth:
$$\begin{align*}
	L = mR^{2}\omega \\
\frac{	GMm}{R^{2}} = \frac{mv^{2}}{R} \\
\therefore v = \sqrt{\frac{GM}{R}}
\end{align*}$$
$$\begin{align*}
	\vec \tau = \vec R \times \vec F &= 0 \;[\because \vec R \parallel \vec F] \\
	\therefore  \frac{d\vec L}{dt} &= 0
\end{align*}$$
- *angular momentum is conserved*
### moment of inertia (I)
$$I = mr^{2}\omega$$
$$\vec  L = I\vec\omega$$
- which is not true if:
	- plane of rotation does not contain the origin of $\vec r$
	- the origin is not the centre of rotation
$$KE = \frac{1}{2} mr^{2}\omega^{2} = \frac{1}{2}I\omega^{2}$$
#### for continuous rigid bodies
$$I = \int r^{2}\,dm$$
- for a thin ring with radius, $R$, and mass $M$, about an axis perpendicular though its centre, let the mass per unit length along the circumference be $\sigma:$ 
$$I = R^{2}\int_{0}^{2\pi} R\sigma\,d\theta = 2\pi R^{3}\sigma = MR^{2}$$
- for a uniform disc with radius, $R$, and mass $M$, about an axis perpendicular though its centre:
	- dividing the disc into concentric rings of radius, $r$, and thickness, $dr$, $\sigma$ is the mass per unit area such that the mass of the ring, $dm=2\pi r\sigma\,dr:$ 
$$I = \int_{0}^{R} 2\pi r^{3}\sigma\,dr = \frac{1}{2} \pi\sigma R^{4} = \frac{1}{2}MR^{2}$$
- for a hollow sphere about an axis through its centre:
$$I = \frac{2}{3}MR^{2}$$
- for a solid sphere about an axis through its centre:
$$I = \frac{2}{5}MR^{2}$$
- for a thin uniform rod about an axis perpendicular though its centre:
$$I = \frac{1}{12}ML^{2}$$
- for a thin uniform rod about an axis perpendicular thought one end:
$$I = \frac{1}{3}ML^{2}$$
#### parallel axis theorem
$$I = I_{COM}+md^{2}$$
- axes about which $I$ and $I_{COM}$ are taken must be parallel