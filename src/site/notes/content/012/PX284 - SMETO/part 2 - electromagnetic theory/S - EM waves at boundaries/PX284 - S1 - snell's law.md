---
{"dg-publish":true,"permalink":"/content/012/px-284-smeto/part-2-electromagnetic-theory/s-em-waves-at-boundaries/px-284-s1-snell-s-law/","noteIcon":"1","created":"2025-03-06T17:39:05.793+00:00","updated":"2025-03-13T19:30:33.516+00:00"}
---

![PX284 - S1 -.png|500](/img/user/pics/PX284%20-%20S1%20-.png)

- the electric field:
$$\vec E = \vec E_{a} \exp(i(\vec k_{a}\cdot \vec x - \omega_{a}t))$$
	where, $a = \{i,r,t\}$

- boundary conditions: 
	- matching phases: $\omega_{i} = \omega_{r}= \omega_t$
	- for all vectors, $\vec x_b$ in the boundary: $\vec k_{i} \cdot \vec x_{b} = \vec k_{r}\cdot \vec x_{b} = \vec k_{t} \cdot \vec x_{b}$ $\implies (\vec k_{r}- \vec k_{i})\cdot \vec x_{b} = 0 = (\vec k_{t}- \vec k_{i})\cdot \vec x_{b}$
	- components of $\vec k_{a}$ in the phase boundary must be equal, therefore the differences must be perpendicular in the boundary, ie: $\hat n \times \vec k_{i} = \hat n \times \vec k_{r} = \hat n \times \vec k_{t} \implies k_{i}\sin i = k_{r} \sin r = k_{t} \sin t$

- the speed:
$$v = \frac{\omega}{k} = \frac{c}{n}$$
	where, $n$ is the refractive index 
- since $\omega$ is same for $i,\;r$ and $t$, $k \propto n \implies k_{i} = k_{r}$, as they are both in $n_{1}$, and therefore, $i = r$ (angles)
- **snell's law:**
$$n_{1} \sin{i} = n_{2} \sin t$$
- if $n_{1} > n_{2}$, when $\sin i > n_{2}/n_{1}$, **total internal reflection** is obtained
