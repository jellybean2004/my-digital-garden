---
dg-publish: true
---

## spherical coordinates
![Pasted image 20240116121526.png](/img/user/pics/Pasted%20image%2020240116121526.png)
- coordinate transformations: 
$$\begin{align}
x &= r \sin\theta \cos\phi \\
y &= r \sin\theta \sin\phi \\
z &= r \cos\theta
\end{align}$$
- what is $dV$?
	$dV = r^{2} \sin\theta \, d\theta \, d\phi \, dr$
 $$I = \iiint_{V} f(\vec r) \, dV = \iiint f(r, \theta, \phi)  r^{2} \sin\theta \, d\theta \, d\phi \, dr$$
 - eg: what is the volume of the sphere with radius, $a$?
	 $$I = \int_{0}^{a} \int_{0}^{2\pi} \int_{0}^{\pi} [f(\vec r)=1]  r^{2} \sin\theta \, d\theta \, d\phi \, dr = \frac{4\pi}{3}a^{3}$$
- *aside* : surface area of a sphere
	- if the radius is increased from $a$ to $a + \delta a$, the volume of the sphere increases by the volume of the spherical shell with thickness $\delta a$, and area of the surface of a sphere: $\Delta V = S.A. \times \Delta a$ : 
	$$S.A. = \frac{\Delta V}{\Delta a} = \frac{d}{da}\left(\frac{4\pi}{3}a^{3}\right)= 4\pi a^{2}$$
## cylindrical coordinates
![Pasted image 20240116122754.png](/img/user/pics/Pasted%20image%2020240116122754.png)
- coordinate transformations: $$\begin{align}
x &= r \cos\theta \\
y &= r \sin\theta\\
z &= z
\end{align}$$
- what is $dV$?
	$dV = r \, dr \, d\theta \, dz$
	
- eg: what is the volume of a cylinder with height, $L$, and radius, $a$?
	$$I = \int_{0}^{L} \int_{0}^{a} \int_{0}^{2\pi} r \, dr \, d\theta \, dz = \pi a^{2}L$$
## 2D polar coordinates
![Pasted image 20240116123420.png](/img/user/pics/Pasted%20image%2020240116123420.png)
- coordinate transformations: 
$$\begin{align}
x &= r \cos\theta \\
y &= r \sin\theta
\end{align}$$
- eg: integrate the gaussian function over all space.
	- gaussian function: $$f(x) = e^{-x^{2}}$$
	$$I = \int_{-\infty}^{+\infty} e^{-x^{2}} \, dx$$
	- trick: $$\begin{align}
	I^{2} &= \int_{-\infty}^{+\infty} e^{-x^{2}} \, dx \int_{-\infty}^{+\infty} e^{-y^{2}} \, dy \\
	&= \int_{-\infty}^{+\infty} \int_{-\infty}^{+\infty} e^{-y^{2}} \, dy \, dx \\
	\end{align}$$
	- switching to polar coordinates: $$\begin{align}
	I^{2} &= \int_{0}^{\infty} \int_{0}^{2\pi} r e^{-r^{2}} \, d\theta \, dr \\
	&= 2\pi  \int_{0}^{\infty} r e^{-r^{2}} \, dr \\
	&= 2\pi \left[ - \frac{1}{2} e^{-r^{2}} \right]_{0}^{\infty}\\
	&= \pi \\
	\therefore I &= \sqrt{\pi}
	\end{align}$$
