---
dg-publish: true
---

- normally, in physics, line integral needs to be performed with some field present
- eg: integral of a spatially varying force along a path to give the change in energy
## for a scalar field
$$I = \int_{A}^{B} \phi\,d\vec r$$

## vector field with a dot product
$$I = \int_{A}^{B} \vec a\cdot d\vec r$$
- eg: $W = \int \vec F \cdot d\vec r$
## a vector field with a cross product
$$I = \int_{A}^{B} \vec a\times d\vec r$$
- eg: $\vec F = \int q \vec v \times B$, $\vec F = I \oint d\vec r \times \vec B$

## example
- a scalar function, $\phi(x,y,z) = ax$, where $a$ is a constant
![Pasted image 20241104123356.png](/img/user/pics/Pasted%20image%2020241104123356.png)
- consider the two paths from $O$ to $B:$ $OAB$ and $OCB$
### path $OAB$
$$\begin{align*}
	I &= \int_{OAB} \phi \, d\vec r \\
	&= \hat i \int_{0}^{1} ax\,dx + \hat j \int_{0}^{1} a\,dy \\
	&= \hat i \left[\frac{ax^{2}}{2}\right]_{x=0}^{1} + \hat j [ ay]_{y=1}^{1} \\
	&= \frac{a}{2}\hat i + a \hat j
\end{align*}$$
### path $OCB$
- for $OC: x=0$ and $\phi = 0 \implies \int_{OC} \phi\,d\vec r = 0$
$$I = \hat i \int_{0}^{1} ax\,dx = \frac{a}{2}\hat i$$
- **note:** integral is path dependent
