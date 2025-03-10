---
{"dg-publish":true,"permalink":"/content/012/px-275-mathematical-methods/term-2/i-optics/px-275-i6a-square-aperture/","noteIcon":"1","created":"2025-03-04T10:43:26.100+00:00","updated":"2025-03-09T12:38:32.937+00:00"}
---

- considering a square hole with sides, $2w$, centred at the origin
- the aperture function:
$$a(y_{1}, y_{2}) = \begin{cases} 1 & \text{for } |y_{1}| < w, |y_{2}| < w ,\\
0 & \text{otherwise}
\end{cases}$$
- the fourier transform:
$$\begin{align*}
\tilde a(\vec k) &= \iint_{-\infty}^{\infty} a(\vec y) \exp(-i \vec k \cdot \vec y) \, dy_{1}\, dy_{2} \\
 &= \int_{-w}^{w}\int_{-w}^{w} \exp(-i \vec k \cdot \vec y) \, dy_{1}\, dy_{2} \\
 &= \int_{-w}^{w}\int_{-w}^{w} \exp\left(-\frac{ik (x_{1}y_{1} + x_{2}y_{2})}{D}\right) \, dy_{1}\, dy_{2} \\
 &= \left[- \frac{D}{ikx_{1}} \exp\left(- \frac{ikx_{1}y_{1}}{D}\right) \right]_{-w}^{w} \left[- \frac{D}{ikx_{2}} \exp\left(- \frac{ikx_{2}y_{2}}{D}\right) \right]_{-w}^{w} \\
 &= - \frac{D}{ikx_{1}}\left[\exp\left(- \frac{ikx_{1}w}{D}\right)- \exp\left(\frac{ikx_{1}w}{D}\right) \right]  \left(- \frac{D}{ikx_{2}}\right) \left[\exp\left(- \frac{ikx_{2}w}{D}\right) - \exp\left(\frac{ikx_{2}w}{D}\right) \right]  \\
 &= \frac{2D}{kx_{1}} \sin\left(\frac{kx_{1}w}{D}\right) \frac{2D}{kx_{2}} \sin\left(\frac{kx_{2}w}{D}\right)  \\
 &= 2w \,\text{sinc}\left(\frac{kx_{1}w}{D}\right) 2w \,\text{sinc}\left(\frac{kx_{2}w}{D}\right)
\end{align*}$$
	where, $\text{sinc }\theta = \cfrac{\sin\theta}{\theta}$
- the observed intensity:
$$\begin{gather}
I \propto |u|^{2} \propto |\tilde a(\vec k)|^{2} \\\
\therefore I(x_{1}, x_{2}) \propto \text{sinc}^{2}\left(\frac{kx_{1}w}{D}\right) \, \text{sinc}^{2}\left(\frac{kx_{2}w}
{D}\right)
\end{gather}$$
- zeroes when $kwx_{1}/D$ or $kwx_{2}/D = n\pi$
- separation of fringes: $\Delta x_{1} = \Delta x_{2} = \pi D/kw$
