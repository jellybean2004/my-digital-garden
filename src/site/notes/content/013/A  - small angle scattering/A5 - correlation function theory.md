---
{"dg-publish":true,"permalink":"/content/013/a-small-angle-scattering/a5-correlation-function-theory/","noteIcon":"1","created":"2025-08-15T10:07:34.278+01:00","updated":"2025-08-15T10:47:31.387+01:00"}
---

## introduction
- SAS is assumed to be elastic, so the momentum transfer can be directly related to the wavelength, ie, spatial distance
- the **correlation function** $\Gamma(\vec r)$ relates the **scattering intensity** in terms this spatial distance
- $\Gamma(\vec r)$ is proportional to the pairwise product of **scattering length densities** (SLDs) for all points separated by $\vec r$ summed over all orientations and locations
- it can be thought og as SLD without the phase information
- correlation function take a 3D vector input, but the measurements from SAS are limited to 1/2D

- $\Gamma_{1}$ looks at changes in a single direction perpendicular to the beam, averaging the other directions
- $\Gamma_{3}$ is described by the Debye equation

- lorentz correction is made
$$I(q) = q^{2} I_{measured}(q)$$

## mathematical destription
- the correlation function arises from calculating the square magnitude of the 3D fourier transform:
$$\frac{d\sigma}{d\Omega} \propto F(\vec q) F^{*}(\vec q) = \int \left[ \int \rho(\vec s) \rho(\vec s+\vec r)\,ds^{3}\right] \exp(i \vec r \cdot \vec q) \, dr^{3}$$
	where, $F(q) = \int \rho(r) \exp(i\vec r\cdot\vec q) \, dr^{3}$ 
- the bracketed term is the correlation function: 
$$\gamma(\vec r) = \int \rho(\vec s) \rho(\vec s+\vec r)\,ds^{3}$$

- they contain no phase information, ie. its fourier transform is purely real and it is an even function that can be written solely in terms of cosines
	- this is as $Z = a \cos \theta  + ib \sin \theta$, with $b = 0$ for real values
$$\gamma (\vec r)  = \int \rho(\vec s) \rho(\vec s + \vec r) \, ds^{3} = \int(\vec u - \vec r) \rho(\vec u)\,du^{3} = \gamma(-\vec r)$$

$$\begin{align*}
\int_{-\infty}^{\infty} f(x) e^{ix\xi}\,dx &= \int_{-\infty}^{0} f(x) e^{ix\xi}\,dx + \int_{-0}^{\infty} f(x) e^{ix\xi}\,dx  \\
&= \int_{0}^{\infty} f(u) e^{-iu\xi}\,du + \int_{-0}^{\infty} f(x) e^{ix\xi}\,dx  \\
&= 2 \int_{0}^{\infty}f(x) \, \frac{e^{ix\xi})+e^{-ix\xi}}{2}\,dx \\
 &= \int_{-\infty}^{\infty} f(x) \cos(x\xi)\,dx
\end{align*}$$

## $\Gamma_{1}$ projection
$$\iiint \gamma(\vec r) e^{i\vec r\cdot q} \,dx\,dy\,dz$$
- for SAS, $q_{z} \simeq 0$
- measuring in one direction of $q_{x}q_{y}$ plane, where $q_{y} = 0$
$$I(q) = \int \gamma(\vec r) e^{ixq_{x}} \,dx\,dy\,dz = \int \left(\iint \gamma(\vec r)\,dy\,dz \right) e^{ixq_{x}}\,dx$$
- the bracketed term is $\Gamma_{1}$
- since $\gamma$ is even:
$$I(q) = \int \Gamma_{1}(x)\cos(qx \,dx)$$
- the Corfunc inverts this:
$$\Gamma_{1}(x) = \int I(q)\cos(qx)\,dx$$
## $\Gamma_3$ projection
- based on spherical symmetry
$$I(q) = \int_{\mathbb R^{3}} \gamma(\vec) \exp(i \vec r \cdot\vec q) \,dr^{3}$$
- averaging over all solid angles:
$$I(\vec q) = \frac{1}{4\pi} \int_{\phi=0}^{2\pi} \int_{\theta=0}^{\pi} \int_{\vec r \in \mathbb R^{3}} \gamma(\vec r) \exp(i qr\cos\theta)\,d\vec r^{3} \sin\theta \, d\theta \, d\phi$$
- this will lead to:
$$I(q) = \int_{\vec r \in \mathbb R^{3}} \gamma(\vec r) \frac{\sin(qr)}{qr} \,dr$$
- the object is independent of the angular components:
$$I(q) = \int_{0}^{\infty} \int_{\Omega}\gamma(\vec r) \, d\Omega \, \text{sinc}(qr) \,dr$$
$$\Gamma_{3} = \int_{\Omega} \gamma(\vec r) \, d\Omega$$

## relationship
$$\begin{align*}
x \Gamma_{3}&= \int I(q) \, \frac{\sin(qx)}{q}\,dq \\
\frac{d}{dx}(x \Gamma_{3}) &= \frac{d}{dx} \int I(q) \frac{\sin(qx)}{q} \,dq = \int I(q) \cos(qx)\,dq \\
\therefore \Gamma_{3}(x) &= \int_{0}^{x} \frac{\Gamma_{1}(r)}{r} \,dr
\end{align*}$$

