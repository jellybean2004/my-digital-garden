---
{"dg-publish":true,"permalink":"/content/012/px-275-mathematical-methods/term-2/i-optics/px-275-i6c-multiple-slits/","noteIcon":"1","created":"2025-03-04T12:34:01.017+00:00","updated":"2025-03-06T12:06:41.167+00:00"}
---

- considering the **young's double slit interference pattern**
- two rectangular slits, $2w\times 2H$, centred at $y_{1}=\pm l$  from the origin
- shifted versions of the single slit function can be combined to describe the two slits
- reminder: convolution of a function with a $\delta$ function shifts the function to $\delta f_{n}$
- the aperture function:
$$\begin{align*}
a(\vec y) &= \int a_{slit}(\vec y') \bigg[ \delta(\vec y' - (\vec y + l \, \hat y_{1})) + \delta(\vec y' - (\vec y - l\, \hat y_{1})) \bigg] \, dy' \\
&= a_{slit} * g(\vec y) \\\\
a_{slit}* g(x') &= \int a_{slit}(x') \, g(x-x')\,dx'
\end{align*}$$
$$\tilde a(\vec k) = \mathcal{F}(a(\vec y)) = \tilde a_{slit}(\vec k) \, \tilde g(\vec k)$$
- it is known that:
$$\tilde a_{slit}\propto \text{sinc}\,\left(\frac{kx_{1}w}{D}\right) \text{sinc}\,\left(\frac{kx_{2}H}{D}\right)$$
$$\begin{align*}
\tilde g(k) &= \int \exp(-i\vec k \cdot \vec y (\delta(\vec y + l \, \hat y_{1})+ \delta(\vec y - l \, \hat y_{1})))\,d\vec y \\ 
&= \exp(i\vec k \cdot l\,\hat y_{1}) + \exp(-i\vec k \cdot l\,\hat y_{2}) \\ 
&= \exp(ik_{1}l) + \exp(-ik_{1}l) \\
&= 2\cos(k_{1}l)
\end{align*}$$
- the intensity:
$$I(\vec x) \propto \text{sinc}^{2}(k_{1}w)\,\text{sinc}^{2}(k_{2}H) \, 2\cos(k_{1}l)$$
	where, $k_{1} = kx_{1}/D$ and $k_{2} = kx_{2}/D$

- the fringe spacing:
	- large rectangular pattern:
$$\begin{gather}
\Delta x_{1} = \frac{\pi D}{kw} \\
\Delta x_{1} = \frac{\pi D}{kH}
\end{gather}$$
	- smaller fringes:
$$\Delta x_{1} = \frac{\pi D}{kl}$$
