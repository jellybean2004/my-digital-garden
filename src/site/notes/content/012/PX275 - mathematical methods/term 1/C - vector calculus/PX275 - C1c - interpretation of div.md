---
{"dg-publish":true,"permalink":"/content/012/px-275-mathematical-methods/term-1/c-vector-calculus/px-275-c1c-interpretation-of-div/","noteIcon":"1","created":"2025-08-27T13:14:15.934+01:00","updated":"2024-11-26T10:05:16.000+00:00"}
---

- consider the electric field due to a charge
![Pasted image 20241028123835.png](/img/user/pics/Pasted%20image%2020241028123835.png)
$$\vec E = \frac{Q}{4\pi\epsilon_{0} r^{2}} (\sin\theta\cos\phi \hat i + \sin\theta\sin\phi\hat j + \cos\theta\hat k) = \frac{Q}{4\pi\epsilon_{0}r^{2}} \hat e_{r}$$
$$\vec\nabla\cdot \vec E = \frac{1}{r^{2}}\frac{\partial }{\partial r} \left(r^{2} \frac{Q}{4\pi\epsilon_{0}r^{2}}\right) = 0$$

![Pasted image 20241028123900.png](/img/user/pics/Pasted%20image%2020241028123900.png)
- a 2D cross section of the scenario:
	- the blue circle is from a sphere
	- the green shape is from a bent disc

- for the sphere, the total flux is not equal to zero, but for the disc, the flux is equal to zero as the flux coming in and going out cancel out
$$\vec\nabla\cdot \vec E = \frac{\sigma}{\epsilon_{0}}$$
	where, $\sigma =$  charge density, $\epsilon_{0}=$ permittivity of free space
- if there is no enclosed charge: 
$$\vec\nabla\cdot\vec E =0$$
 - for a magnetic field, there are no magnetic monopoles: 
 $$\vec\nabla\cdot\vec B =0$$
