---
dg-publish: true
---

- consider a cylinder rotating about the $z$-axis, so the angular velocity: $\vec \omega = \omega_{z}\hat k$
![Pasted image 20241031121453.png](/img/user/pics/Pasted%20image%2020241031121453.png)
- looking down the $z$-axis, the linear velocity, $\vec v$, of a point on the cylinder will be perpendicular to its position vector, and direction of $\vec v$ will be $-y\hat i + x\hat j$
- the angular velocity: 
$$|\omega| = \frac{|\vec v|}{r} \implies |\vec v| = |\omega|r$$
$$\vec v = - \omega y\hat i + \omega x\hat j$$
- considering the curl of $\vec v:$ 
$$\vec\nabla \times \vec v = \left|\begin{matrix}\hat i & \hat j & \hat k \\ \frac{\partial }{\partial x} & \frac{\partial }{\partial y} & \frac{\partial }{\partial z} \\ -\omega_{z}y & \omega_{z}x & 0\end{matrix} \right| = 2\omega_{z}\hat k$$