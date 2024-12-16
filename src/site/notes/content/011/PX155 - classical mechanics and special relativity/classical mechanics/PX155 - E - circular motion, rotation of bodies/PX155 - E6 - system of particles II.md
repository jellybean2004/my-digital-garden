---
{"dg-publish":true,"permalink":"/content/011/px-155-classical-mechanics-and-special-relativity/classical-mechanics/px-155-e-circular-motion-rotation-of-bodies/px-155-e6-system-of-particles-ii/","noteIcon":"1","created":"2024-10-01T18:27:09.715+01:00","updated":"2024-11-26T19:56:28.611+00:00"}
---

- as *[[content/011/PX155 - classical mechanics and special relativity/classical mechanics/PX155 - B - systems of particles, accelerations/PX155 - B1 - systems of particles I\|before]]*, consider a body as a system of particles subject to internal and external forces
- total force on the particle :
$$\vec F= \vec F_{i} + \sum\limits_{j\neq i} \vec F_{ji} = \frac{d\vec p_{i}}{dt}$$
- if positions $\vec r_{i}$ are measured from $O$, then the torque about $O$:
$$\vec\tau_{i} = \vec r_{i} \times (\vec F_{i} + \sum_{j\neq i} \vec F_{ji}) = \frac{d\vec L_{i}}{dt}$$
- total torque
$$\vec\tau =\sum\limits_{i}\vec r_{i}\times (\vec F_{i}+\sum\limits_{j\neq i} \vec F_{ji})= \sum\limits_{i}\vec r_{i}\times \vec F_{i} + \sum\limits_{i}\sum\limits_{j\neq i} \vec r_{i} \times F_{ji} = \sum\limits_{i}\frac{d\vec L_{i}}{dt}$$
- $\sum\limits_{i}\sum\limits_{j\neq i} \vec r_{i} \times F_{ji}=0$ as for central forces, acting along the line between particles, [[content/011/PX155 - classical mechanics and special relativity/classical mechanics/PX155 - A - foundations of classical mechanics/PX155 - A3 - newton's third law\|PX155 - A3 - newton's third law]]: internal force term cancels out
- ![Pasted image 20231104150825.png](/img/user/pics/Pasted%20image%2020231104150825.png)
	- both $F_{21}$ and $F_{12}$ have some perpendicular distance from the pivot, so, generate equal and opposite torques
$$\vec \tau  = \sum\limits_{i}(\vec r_{i}\times \vec F_{i})= \frac{d}{dt}\sum\limits_{i}\vec L_{i} = \frac{d\vec L}{dt}$$
- *total torque from external forces on a composite body equals the rate of change of its total angular momentum*:
$$\vec\tau = \frac{d\vec L}{dt}$$
