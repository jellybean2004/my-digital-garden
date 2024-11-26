---
{"dg-publish":true,"permalink":"/content/012/px-275-mathematical-methods/c-vector-calculus/px-275-c1e-examples-of-curl/","created":"2024-11-25T10:50:32.000+00:00","updated":"2024-11-26T10:05:20.701+00:00"}
---

## 1
- consider water flowing with a velocity, $\vec v$, in the $\hat i$ direction: $\vec v = x\hat i$
- the curl: 
$$\vec\nabla \times \vec v = \left| \begin{matrix}\hat i & \hat j & \hat k \\ \frac{\partial }{\partial x} & \frac{\partial }{\partial y} & \frac{\partial }{\partial z} \\ x & 0 & 0\end{matrix} \right| = 0$$
- **interpretation:** if there is a raft on the water, it will not rotate
![Pasted image 20241031121420.png](/img/user/pics/Pasted%20image%2020241031121420.png)
## 2
- now, the water is flowing in the $y$-direction, but the velocity increases in the $x$-direction: but $\vec v = x\hat j$
- the curl: 
$$\vec\nabla \times \vec v = \left| \begin{matrix}\hat i & \hat j & \hat k \\ \frac{\partial }{\partial x} & \frac{\partial }{\partial y} & \frac{\partial }{\partial z} \\ 0 & x & 0\end{matrix} \right| = \hat k$$
- **interpretation:** a raft will tend to spin
![Pasted image 20241031121434.png](/img/user/pics/Pasted%20image%2020241031121434.png)
