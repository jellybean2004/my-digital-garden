---
{"dg-publish":true,"permalink":"/content/011/px-155-classical-mechanics-and-special-relativity/classical-mechanics/px-155-e-circular-motion-rotation-of-bodies/px-155-e16-using-conservation-of-momentum/","created":"2024-10-01T18:27:09.700+01:00","updated":"2024-11-26T19:57:24.358+00:00"}
---

- if no torques act about a point then the angular momentum is conserved about that point
- ball striking a bat: no torque(or force) external to bat + ball $\implies L$ is conserved
![Pasted image 20231112152143.png](/img/user/pics/Pasted%20image%2020231112152143.png)
- 2 key points:
- ball is in contact with the bat for a small time, $\Delta T$, during which, we ignore the movement of the bat
	- ie: ball imports an *impulse*: $\Delta p = \int F.dt$
- after the impulse, no forces on the bat, so, $a_{cm}=0$ for the bat. this means, the centre of rotation after the ball hits must be the centre of mass
- conserve linear momentum:
$$mv_{cm} = \Delta p$$
- conserve angular momentum about the bat's centre of mass:
$$I_{cm}\omega = (x-x_{cm})\Delta p$$
- where is the sweet spot, $x$, such that $v_{H}=0$?
$$v_{H}= v_{cm}-\omega x_{cm}= \frac{\Delta p}{m} - \frac{(x-x_{cm})\Delta pc_{cm}}{I_{cm}}$$
- solve for $x$ so that the velocity of the handle, $v_{H}=0:$
$$x = x_{cm}+ \frac{I_{cm}}{mx_{cm}}$$
- uniform bat length, $L$, $x_{cm}= \frac{L}{2}$, $I_{cm}=\frac{1}{12}ML^{2}:$
$$x=\frac{2}{3}L$$

