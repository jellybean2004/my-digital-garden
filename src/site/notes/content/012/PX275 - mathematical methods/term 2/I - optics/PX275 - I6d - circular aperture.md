---
{"dg-publish":true,"permalink":"/content/012/px-275-mathematical-methods/term-2/i-optics/px-275-i6d-circular-aperture/","noteIcon":"1","created":"2025-03-06T12:10:48.117+00:00","updated":"2025-03-09T12:56:29.294+00:00"}
---

- considering a circular hole with radius, $R$
- using polar coordinates:
$$\begin{gather}
y_{1} = r \cos\theta\\
y_{2} = r \cos \theta \\
y_{3} = 0 \\\\

x_{1} = \rho \cos\phi\\
x_{2} = \rho \cos \phi \\
x_{3} = D \\\\
\end{gather}$$
- in the far field regime:
  $$\vec k = k \frac{\vec x}{|\vec x|} = \frac{k}{D} \begin{pmatrix}\rho \cos\phi \\ \rho \sin\phi \\ D\end{pmatrix}$$
- using the [[content/012/PX275 - mathematical methods/term 1/B - coordinate systems and integration/B2-4  - integration/PX275 - B3 - jacobian\|jacobian integrals]]:
$$\begin{gather}
dy_{1} dy_{2} = r\,dr\,d\theta \\
dx_{1}dx_{2} = \rho\,d\rho\,d\phi
\end{gather}$$
- the aperture can be written as:
$$a(r,\theta) = \begin{cases} 1 & \text{if } r<R, \\ 0 & \text{otherwise}\end{cases}$$
- the fourier transform:
$$\begin{align*}
\tilde a (\vec k) &= \int_{0}^{2\pi} \int_{0}^{\infty} a \, e^{-i\vec k \cdot \vec y}\, r\,dr\,d\theta \\
&= \int_{0}^{2\pi} \int_{0}^{R}  e^{-i\vec k \cdot \vec y}\, r\,dr\,d\theta \\
&= \int_{0}^{2\pi} \int_{0}^{R} \exp\left(- \frac{ikr\rho}{D} (\cos\phi\cos\theta + \sin\phi\sin\theta) \right) \, d\rho\,d\theta \\
&= \int_{0}^{2\pi} \int_{0}^{R} \exp\left(- \frac{ikr\rho}{D} (\cos(\theta - \phi)  \right) \, d\rho\,d\theta \\
&= \int_{0}^{2\pi} \int_{0}^{R} \exp\left(- \frac{ikr\rho}{D} \cos\theta  \right) \, d\rho\,d\theta' \\
\end{align*}$$
- here, **bessel functions** come in handy
$$J_{n}(x) = \frac{i^{n}}{2\pi} \int_{0}^{2\pi} \exp(-in\theta - ix \cos\theta) \, d\theta$$
- here, taking ${} n=0$ and $x = k\rho r/D: {}$
$$J_{0}(x) = \frac{1}{2\pi} \int_{0}^{2\pi} \exp(-ix\cos\theta)\, d\theta$$
- the **recurrence relation** is a convenient property of bessel functions:
$$\frac{d}{dx}(x^{n} J_{n}(x)) = x^{n} J_{n-1}(x)$$
- this can be rewritten as:
$$\int_{a}^{b} x^{1} \, J_{0}(x) \, dx = \bigg[ x^{1} J_{1}(x) \bigg]_{a}^{b}$$

- going back to the fourier transform:
$$\begin{align*}
\tilde a(\vec k) &= 2\pi \int_{0}^{R} r \, J_{0} \left(\frac{k\rho r}{D}\right) \, dr  \\
&= 2\pi  \int_{0}^{k\rho R/D}
\frac{D}{k\rho} x \, J_{0}(x) \, \frac{D}{k\rho}\, dx \\
&= 2\pi \left(\frac{D}{k\rho}\right)^{2} \int_{0}^{k\rho R/D}
x\, J_{0}(x) \, dx \\
&= 2\pi \left(\frac{D}{k\rho}\right)^{2} \bigg[ x\, J_{1}(x) \bigg]_{0}^{k\rho R/D} \\
&= 2\pi \left(\frac{D}{k\rho}\right)^{2} \left( \frac{k\rho R}{D} \, J_{1}\left(\frac{k\rho R}{D}\right) \right) - 0 \\
&= 2\pi R \left(\frac{D}{k\rho}\right) \, J_{1}\left(\frac{k\rho R}{D}\right) \\
&= 2\pi R^{2} \frac{J\left(\frac{k\rho R}{D}\right)}{\frac{k\rho R}{D}}
\end{align*}$$
- this is similar to the $\text{sinc}$ function
- therefore, it can be concluded that:
$$I \propto |u|^{2} \propto |\tilde a(\vec k)|^{2} \propto \left(\frac{J\left(\frac{k\rho R}{D}\right)}{\frac{k\rho R}{D}}\right)^{2}$$
- this is known as the **airy pattern**
- 