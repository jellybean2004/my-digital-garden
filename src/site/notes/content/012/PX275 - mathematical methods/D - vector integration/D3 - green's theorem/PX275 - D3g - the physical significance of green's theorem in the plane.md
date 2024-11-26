---
dg-publish: true
---

- [[content/012/PX275 - mathematical methods/D - vector integration/D3 - green's theorem/PX275 - D3a - green's theorem in the plane\|green's theorem in the plane]]: 
$$\oint \vec F \cdot d \vec r =  \iint_{R} (\vec\nabla \times \vec F) \cdot d\vec A = \iint_{R} (\vec\nabla \times \vec F)_{z}dA$$
- considering a field, $\vec F$, describing the laminar flow of water
![Pasted image 20241114124910.png](/img/user/pics/Pasted%20image%2020241114124910.png)
- at $A$ and $B$, $\vec F \cdot d\vec r$ do not cancel, but they do at diametrically opposite points, ie: $A$ and $B$, or $B$ and $C$, therefore: 
$$\oint_{C}\vec F \cdot d\vec r = 0$$
![Pasted image 20241114125051.png](/img/user/pics/Pasted%20image%2020241114125051.png)
- comparing to the whirlpool
- $\vec F$ and $d\vec r$ are always parallel to each other, so: 
$$\oint_{C}\vec F \cdot d\vec r >0$$
- considering the magnetic field around a current carrying wire: 
$$\vec B = \frac{\mu_{0}I}{2\pi r} \hat\phi$$
![Pasted image 20241114125243.png](/img/user/pics/Pasted%20image%2020241114125243.png)
![Pasted image 20241114125251.png](/img/user/pics/Pasted%20image%2020241114125251.png)
- in the radial direction: $\vec B \perp d\vec r$, so, $\vec B \cdot d\vec r = 0$
- for the loop: 
$$\oint_{C}\vec B \cdot d\vec r = \int_{line}\vec B_{r1} \cdot d\vec r \int_{line}\vec B_{r2} \cdot d\vec r$$
- using the relation for the length of arc, $l = \theta\,r$, along the arc, $\int dr = \theta r_{n}:$ 
$$\begin{align*}
	\int_{line}\vec B_{r1} \cdot d\vec r = \frac{\mu_{0}I}{2\pi r_{1}} = \frac{\mu_{0}I\theta}{2\pi} \\
	\int_{line}\vec B_{r2} \cdot d\vec r = \frac{\mu_{0}I}{2\pi r_{2}} = - \frac{\mu_{0}I\theta}{2\pi}
\end{align*}$$
- therefore the integral around the loop becomes: 
$$\oint_{C}\vec B \cdot d\vec r = 0$$
