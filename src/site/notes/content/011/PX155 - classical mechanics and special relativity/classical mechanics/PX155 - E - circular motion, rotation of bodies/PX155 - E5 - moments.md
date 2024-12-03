---
{"dg-publish":true,"permalink":"/content/011/px-155-classical-mechanics-and-special-relativity/classical-mechanics/px-155-e-circular-motion-rotation-of-bodies/px-155-e5-moments/","created":"2024-10-01T18:27:09.711+01:00","updated":"2024-11-26T19:56:25.850+00:00"}
---

## introduction
- familiar eg: ![Pasted image 20231104143042.png](/img/user/pics/Pasted%20image%2020231104143042.png)
	- *archimedes' lever rule*: moments must balance if the lever doesn't rotate
	
$$moment = F \times d_{perp}$$
	- take moments about $P$: $r_{1}W_{1}=r_{2}W_{2}$ for balance
## torque
-  define torque:
$$\vec \tau = \vec r \times \vec F$$with dimensions $Nm$	
- generalisation of turning moment to 3D

![Pasted image 20231104143249.png](/img/user/pics/Pasted%20image%2020231104143249.png)
- perpendicular distance of line of action of $\vec F$ to point $O$ is $r\sin\theta$
- from the *right-hand rule*: $\vec\tau$ out of the page generating an anti-clockwise rotation of particle
- like a moment, $\vec \tau$ must always be defined with respect to a point (of reference), not necessarily the centre of rotation

### derivation
- what does a torque do?
	- from [[content/011/PX155 - classical mechanics and special relativity/classical mechanics/PX155 - A - foundations of classical mechanics/PX155 - A2 - newton's second law\|newton's second law]]: $\vec F = m \frac{d\vec v}{dt}$
	$$\vec r \times \vec F = m (\vec r\times\frac{d\vec v}{dt})$$
	- consider $\frac{d}{dt}(\vec r \times \vec v) = \frac{d\vec r}{dt}\times \vec v + \vec r \times \frac{d\vec v}{dt}$
		- $\frac{d\vec r}{dt}= \vec v, \; \therefore \frac{d\vec r}{dt}\times\vec v=0$
	$$\frac{d}{dt} (\vec r \times \vec v) = \vec r \times \frac{d\vec v}{dt}$$
	- so,
$$\vec r \times \vec F = m \frac{d}{dt}(\vec r \times \vec v) = \frac{d}{dt}(\vec r \times \vec p)$$
	- looks a lot like [[content/011/PX155 - classical mechanics and special relativity/classical mechanics/PX155 - A - foundations of classical mechanics/PX155 - A2 - newton's second law\|newton's second law]] , so, define $\vec L = \vec r \times \vec p$ ($kgm^{2}s^{-1}$), which is the *angular momentum* (moment of momentum)
	$$\vec \tau = \vec r \times \vec F = \frac{d}{dt}\vec L$$
- *torque is the rate of change of angular momentum* (both $\vec\tau$ and $\vec L$ must be around some point)
- ***note***: a particle moving in a straight line will have a non-zero $\vec L$ along any point not along that straight line