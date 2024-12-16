---
{"dg-publish":true,"permalink":"/content/011/px-157-electricity-and-magnetism/px-157-b-electric-fields/i-field/px-157-b4b-electric-flux-from-an-arbitrary-surface/","noteIcon":"1","created":"2024-10-01T18:27:10.065+01:00","updated":"2024-11-26T20:07:19.824+00:00"}
---

![Pasted image 20240116233410.png](/img/user/pics/Pasted%20image%2020240116233410.png)
$$
d\phi_{E,ij} = \vec E_{ij} \cdot d\vec S_{ij}
$$
$$\begin{align}
\phi_{E} &= \sum\limits_{i} \sum\limits_{j} d \phi_{E,ij} \\
&= \sum\limits_{i} \sum\limits_{j} \vec E_{ij} \cdot d\vec S_{ij} \\
\therefore \phi_{E}&= \iint_{S} \vec E \cdot d\vec S
\end{align}$$
- if the surface is closed:
$$
  \newcommand{\oiint}{\subset\!\supset \!\!\!\!\!\!\!\!\!\!\iint} \phi_{E} = \oiint_{S} \vec E \cdot d\vec S$$
- $d\vec S$ is always chosen pointing *outwards*

- eg: a point charge, $+q$, at the origin. 
	![Pasted image 20240116233519.png](/img/user/pics/Pasted%20image%2020240116233519.png)
	- choosing a spherical surface with radius, $r$, concentric with the charge:
$$\begin{align*}
	\vec E &= \frac{q}{4\pi\epsilon_{0}r^{2}} \hat r\\
	d\vec S &= dS \, \hat r
	\end{align*}$$
	$$\begin{align}
	\phi_{E} &= \oiint_{S}  \frac{q}{4\pi\epsilon_{0}r^{2}} \hat r \cdot \hat r \, dS \\
	&= \frac{q}{4\pi\epsilon_{0} r^{2}} \oiint_{S} dS
	\end{align}$$
	- the sphere has a surface area, $S= 4\pi r^{2}$:
$$
\therefore \phi_{E} = \frac{q}{\epsilon_{0}}
$$
- eg: the electric flux though a sphere concentric with an ideal electric dipole with dipole moment, $\vec p = p \hat z$
	![Pasted image 20240116233918.png](/img/user/pics/Pasted%20image%2020240116233918.png)
	- coordinates to describe any point on the sphere, $\theta$ and $\phi$, gives position vector:
$$
\vec r' = r' \cos\phi' \sin\theta' \hat x + r' \sin\phi' \sin\theta' \hat y + \hat r \cos\theta' \hat z
$$
	- the surface vector for a small section at $(\theta',\phi')$ is given by:
$$
d\vec S = \frac{\partial \vec r'}{\partial \theta'} \times \frac{\partial \vec r'}{\partial \phi'} \, d\theta \, d\phi = r'^{2} \sin\theta' \hat r \, d\theta \, d\phi
$$
	$$\vec E \approx  \frac{1}{4\pi\epsilon_{0}r^{3}}[3(\vec p \cdot \hat r)\hat r -\vec p]$$ 
	$$d\vec S = dS \hat r = r^{2} \sin\theta \, d\theta \, d\psi \, \hat r$$
	$$\vec E \cdot d\vec S =  \frac{1}{4\pi\epsilon_{0}r^{3}} r^{2} \sin\theta \, d\theta \, d\phi \, \hat r \, [3(\vec p \cdot \hat r)\hat r -\vec p] \cdot \hat r$$
	- use $\vec p \cdot \hat r = p(\hat z \cdot \hat r) = p\cos\theta$ :
$$
\vec E \cdot d\vec S =  \frac{1}{4\pi\epsilon_{0}r^{3}} r^{2} \sin\theta \, 2p\cos\theta \, d\theta \, d\phi \, \hat r
$$
	$$\phi_{E} = \int_{0}^{2\pi} \int_{0}^{\pi}  \frac{1}{4\pi\epsilon_{0}r^{3}} r^{2} \sin\theta \, 2p\cos\theta \, d\theta \, d\psi \, \hat r$$
	- in this:
$$
\int_{0}^{\pi}  2\sin\theta\cos\theta d\theta = \int_{0}^{\pi}\sin2\theta = 0
\1\n\2\n