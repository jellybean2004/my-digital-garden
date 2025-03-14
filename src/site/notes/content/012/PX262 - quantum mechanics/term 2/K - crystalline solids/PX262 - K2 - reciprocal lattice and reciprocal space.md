---
{"dg-publish":true,"permalink":"/content/012/px-262-quantum-mechanics/term-2/k-crystalline-solids/px-262-k2-reciprocal-lattice-and-reciprocal-space/","noteIcon":"1","created":"2025-02-06T10:39:08.237+00:00","updated":"2025-03-13T12:44:07.212+00:00"}
---

- the structure of crystals can be found from x-ray diffraction measurements, which probe the **reciprocal lattice**
- since a crystal has periodicity, the properties (like the potential, the electron density) are also expected to be periodic functions
- [[content/011/PX153 - mathematics for physicists/term 2/PX153 - J - fourier series/PX153 - J1 - introduction\|fourier series]]:
$$f(x) = a_{0} + \sum\limits_{n\neq0} \left(a_{n} \cos\left(\frac{2\pi n x}{a}\right) + b_{n} \sin\left(\frac{2\pi n x}{a}\right) \right)$$
- periodicity:
$$f(x ) = f(x+a)  = f(x+2a) = \dots$$
- complex representation:
$$F(x) = \sum\limits_{n}F_{n}\exp\left(i \frac{2\pi nx}{a}\right) = \sum\limits_{n}F_{n} e^{iG_{n}x}$$
	where, $F_{n} = a_{n}+ ib_{n}$, and $G_{n} = 2\pi n/a$
$$F_{n} = \frac{1}{a} \int_{0}^{a} F(x) \, \exp\left(i \frac{2\pi nx}{a}\right) \,dx$$
- clearly, $\exp(iG_{n}a) = 1 = \exp(i2\pi n)$
- the points sit on a lattice with a spacing of $2\pi/a$
- for a 3D lattice, were each point is located by three integers: $n_{1},\,n_2,\,n_3:$
$$\vec R_{n_{1}n_{2}n_{3}} = n_{1}\vec a + n_{2}\vec b + n_{3}\vec c$$
- looking for: $\exp(iG_{h,k,l} - \vec R_{n_{1}n_{2}n_{3}}) = 1$
- choosing ${} \vec G_{h,k,l} = h \vec A + k \vec B + l \vec C$
$$\begin{align*}
\vec A &= \frac{2\pi (\vec b \times \vec c)}{\vec a \cdot (\vec b \times \vec c)} \\
\vec B &= \frac{2\pi (\vec c \times \vec a)}{\vec a \cdot (\vec b \times \vec c)} \\
\vec C &= \frac{2\pi (\vec a \times \vec b)}{\vec a \cdot (\vec b \times \vec c)}
\end{align*}$$

- eg: a simple tetragonal lattice with primitive vectors:

$$\begin{gather*}
\vec a = a (1,0,0) = a \hat x \\
\vec b = a (0,1,0) = a \hat y \\
\vec c = c (0,0,1) = c \hat z \\
c>a
\end{gather*}$$
- the position vectors for the points on the lattice are:
$$\vec R_{n_{1},n_{2},n_{3}} = n_{1}\vec a + n_{2}\vec b + n_{3}\vec c$$

- the number of nearest neighbours that any/each point has is given by the shortest distance between any two points, which is $a$ since $c > a$
- each point on the lattice has four nearest neighbours, ie: $\vec R_{1,0,0} , \; \vec R_{-1,0,0}, \; \vec R_{0,1,0}, \; \vec R_{0,-1,0}$

- finding the position vectors of the reciprocal lattice, $\vec G_{h,k,l}:$
$$\vec G_{h,k,l} = h \vec A +  k \vec B + l \vec C$$
$$\begin{gather}
\exp(i\vec G_{h,k,l}\cdot \vec R_{n_{1},n_{2},n_{3}}) = 1 \\\\
\vec A = \frac{2\pi a c }{a^{2}c} \hat x = \frac{2\pi}{a}(1,0,0) \\
\vec B = \frac{2\pi a c }{a^{2}c} \hat y = \frac{2\pi}{a}(0,1,0) \\
\vec C = \frac{2\pi a^{2}}{a^{2}c} \hat z = \frac{2\pi}{c}(0,0,1)
\end{gather}$$
- this is another tetragonal lattice with lattice constant ${} 2\pi/a {}$ and $2\pi/c$
$$\vec G_{0,0,1} = \frac{2\pi}{c} \hat z$$
- this is a vector which specifies the normal vector of a plane perpendicular to the $z$-axis

