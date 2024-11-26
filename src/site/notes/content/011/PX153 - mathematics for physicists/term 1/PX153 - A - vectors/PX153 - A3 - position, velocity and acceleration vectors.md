---
{"dg-publish":true,"permalink":"/content/011/px-153-mathematics-for-physicists/term-1/px-153-a-vectors/px-153-a3-position-velocity-and-acceleration-vectors/","created":"2024-11-25T10:50:32.000+00:00","updated":"2024-11-26T19:34:29.680+00:00"}
---

![Pasted image 20231003172648.png](/img/user/pics/Pasted%20image%2020231003172648.png)
- position vector, usually $\vec r$, describes the position of point P relative to the origin 
- eg: for trajectory of a particle, $\underline r(t) = x(t)\underline{\hat i} + y(t) \underline{\hat ij} + z(t) \underline{\hat k}$
$$\underline v(t) = \frac{d \underline r}{dt} = \frac{d x(t)}{dt}\underline{\hat i} + \frac{d y(t)}{dt}\underline{\hat j} + \frac{d z(t)}{dt}\underline{\hat k}$$
$$\underline a(t) = \frac{d^2 \underline r}{dt^2} = \frac{d^2 x(t)}{dt}\underline{\hat i} + \frac{d^2 y(t)}{dt^2}\underline{\hat j} + \frac{d^2 z(t)}{dt^2}\underline{\hat k}$$
	- cartesian coordinates, initial position $\underline r_{o}= h_{o}\underline{\hat j}$
	- gravity is in the negative y direction $\underline g = -g\underline{\hat j}$
	- initial velocity ($v_{0})= (v_{0x}  ,v_{0y} )=v_{0x} \underline{\hat i}+v_{0y} \underline{\hat j}$
## equations of motion in vector notation
$$\vec F = m \vec a = m \vec g$$
$$ \vec a=\frac{d^2r}{dt^{2}}=-g\underline{\hat j}=\frac{d \vec v}{dt}$$
- integrate to find velocity:
$$\vec v(t) = \vec v_{0}+ \int^t_{0}\frac{d \vec v}{dt}dt= \vec v_{0}+\int^t_{0}-g\underline{\hat j}.dt$$
$$\vec v= \vec v_{0} - gt \underline{\hat j}$$
- integrating again:
$$\vec r(t) = \vec r_0+\int_0^t\vec v(t).dt = \vec r_0 +\vec v_0 t - \frac{1}{2}gt^2\underline{\hat j}$$
- the components:
	- $x(t)=v_{0x}t$
	- $y(t)=h_0+v_{0y}t-\frac{1}{2}gt^2$
(check that $\vec r(0)$ and $\vec v(0)$ are correct)
we can solve for $y(x)$ using $t=\frac{x}{v_{0x}}$
$$y(x) = h_{0}+ (\frac{v_{0y}}{v_{0x}})x-\frac{1}{2}g\frac{x^2}{v_{0x}^2}$$
a parabola as expected