---
{"dg-publish":true,"permalink":"/content/012/px-262-quantum-mechanics/g-measurement-of-angular-momentum/px-262-g6a-spin-orbit-coupling/","noteIcon":"1","created":"2024-11-26T11:07:58.725+00:00","updated":"2024-11-26T11:22:40.494+00:00"}
---

- classically orbiting electrons around nucleus generates magnetic field, and electron spin can interact with this internal magnetic field
- classically generated magnetic field will be:
$$B = \frac{\mu_{0}Ze\omega}{4\pi r} = \frac{\mu_{0}Ze}{4\pi mr^{3}}l$$
	where, $\frac{Ze\omega}{2\pi}$ corresponds to the current 
- the spin magnetic moment:
$$ \vec \mu_{s} = - \frac{e}{m}\vec s$$
- and the energy of the interaction:
$$W = - \frac{1}{2} \vec \mu_{s} \cdot \vec B = \frac{\mu_{0}Ze^{2}}{8\pi m^{2}r^{3}} \vec l \cdot \vec s$$
	where, the factor of $1/2$ comes from a relativistic effect known as **thomas precession**
- $\vec l \cdot \vec s$ can be expressed through the total angular momentum: 
$$\begin{align*}
 \vec j &= \vec l + \vec s \\
 \implies j^{2} &= l^{2}+ s^{2} + 2 \,\vec l \cdot \vec s \\
 \therefore \vec l \cdot \vec s &= \frac{1}{2} (j^{2} - l^{2} - s^{2})
\end{align*}$$
- the energy is: 
$$W = \frac{\mu_{0}Ze^{2}}{16\pi m^{2}r^{3}} (j^{2}-l^{2}- s^{2})$$
- in analogy: 

$$\hat H_{LS} = f(r) (\hat J^{2} - \hat L^{2} - \hat S^{2})$$
	where, $f(r) = \frac{\mu_{0}Ze^{2}}{4\pi m^{2}r^{3}}$
- this is called **spin-orbit (LS) coupling**

- adding the part for the interaction with external magnetic field: $$\hat H_{B} = - \frac{eB_{0}}{2m} (\hat L_{z}+ 2\hat S_{z})$$
- aligned the external magnetic field with the $z$-axis

- two corrections to the energies of the individual states in the hydrogen atom, which breaks some degeneracy
