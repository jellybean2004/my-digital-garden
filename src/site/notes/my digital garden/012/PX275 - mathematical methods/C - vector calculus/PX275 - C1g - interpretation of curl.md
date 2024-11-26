---
{"dg-publish":true,"permalink":"/my-digital-garden/012/px-275-mathematical-methods/c-vector-calculus/px-275-c1g-interpretation-of-curl/","created":"2024-11-25T10:50:32.000+00:00","updated":"2024-11-26T10:05:24.132+00:00"}
---

![Pasted image 20241031122818.png](/img/user/pics/Pasted%20image%2020241031122818.png)
- assuming that angular momentum is conserved
		$L = mvr$
		$|\omega| = \frac{v}{r}$
		$L = m|\omega|r^{2}$
	$|\omega| \propto \frac{1}{r^{2}}$ and $v \propto \frac{1}{r}$
- the velocity: 
$$\vec v = \frac{k}{\rho} \, \hat e_\phi$$
	where, $k$ is a constant
- the curl: 
$$\vec\nabla \times \vec v = \frac{1}{\rho} \left|\begin{matrix}\hat e_\rho & \rho\hat e_{\phi} & \hat e_{z} \\ \frac{\partial }{\partial \rho} & \frac{\partial }{\partial \phi} & \frac{\partial }{\partial z} \\ 0 & \rho\frac{k}{\rho} & 0 \end{matrix} \right| = 0$$
- previously, something spinning was thought of as having a curl
- but here, it is the curl of a velocity field, ie: the potential for that field to 'curl' something around

- basically, every point of a raft on the field experiences the same force, so it does not turn

- consider two red buoys and a paddle wheel in a whirlpool
- the paddle wheel will go around the centre of the whirlpool, but it won’t rotate on it’s own axis 
- this happens because the angular velocity of the liquid changes with radial distance out from the centre
- locally the curl is always zero, in the neighbourhood of the point of interest

- when the curl, $\vec\nabla\cdot\vec v =0$, the velocity field, $\vec v$ is said to be '*irrotational*' in that region
![Pasted image 20241031132145.png](/img/user/pics/Pasted%20image%2020241031132145.png)
![Pasted image 20241031132220.png](/img/user/pics/Pasted%20image%2020241031132220.png)
![Pasted image 20241031132259.png](/img/user/pics/Pasted%20image%2020241031132259.png)
