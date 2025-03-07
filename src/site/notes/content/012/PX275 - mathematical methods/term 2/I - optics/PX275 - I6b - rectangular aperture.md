---
{"dg-publish":true,"permalink":"/content/012/px-275-mathematical-methods/term-2/i-optics/px-275-i6b-rectangular-aperture/","noteIcon":"1","created":"2025-03-04T12:24:14.269+00:00","updated":"2025-03-04T12:33:04.419+00:00"}
---

- considering a rectangular hole of width, $2w$, and height, $2H$, centered at the origin
- the aperture function:
$$a(y_{1}, y_{2}) = \begin{cases}
1 & \text{if } - w <y_{1}<w\; \text{and } -H<y_{2}<H, \\
0 & \text{otherwise}.
\end{cases}$$
- the fourier transform:
$$\begin{align*}
\tilde a(\vec k) &= \int_{-w}^{w} \int_{-H}^{H} \exp\left(-\frac{ik (x_{1}y_{1} + x_{2}y_{2})}{D}\right) \, dy_{1}\, dy_{2} \\
&= \left[ - \frac{D}{ikx_{1}}\exp\left(- \frac{ikx_{1}y_{1}}{D}\right) \right]_{-w}^{w} \left[ - \frac{D}{ikx_{2}}\exp\left(- \frac{ikx_{2}y_{2}}{D}\right) \right]_{-H}^{H} \\
&= \dots \\
&= 2w \, \text{sinc }\left(\frac{kx_{1}w}{D}\right) \, 2H \, \text{sinc }\left(\frac{kx_{2}H}{D}\right)
\end{align*}$$
- the intensity:
$$I(\vec x) \propto \text{sinc}^{2} \left(\frac{kx_{1}w}{D}\right) \text{sinc}^{2} \left(\frac{kx_{2}H}{D}\right) $$

- the spacing of fringes:
$$\begin{gather}
\frac{kx_{1}w}{D} = n\pi  \implies \Delta x_{1} = \frac{\pi D}{kw} = \frac{D\lambda}{2w} \\
\frac{kx_{2}H}{D} = n\pi  \implies \Delta x_{2} = \frac{\pi D}{kH} = \frac{D\lambda}{2H} 
\end{gather}$$
