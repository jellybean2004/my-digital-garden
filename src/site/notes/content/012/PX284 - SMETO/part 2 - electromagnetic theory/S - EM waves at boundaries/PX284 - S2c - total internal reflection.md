---
{"dg-publish":true,"permalink":"/content/012/px-284-smeto/part-2-electromagnetic-theory/s-em-waves-at-boundaries/px-284-s2c-total-internal-reflection/","noteIcon":"1","created":"2025-08-27T13:15:28.787+01:00","updated":"2025-03-14T06:56:36.000+00:00"}
---

- considering $n_{1} > n_{2}$
- using snell's law:
$$n_{1} \sin i = n_{2} \sin t$$
- if $\sin i > n_{2}/n_{1} \implies \sin t>1:$ there is no solution for $t$
- there is no transmitted light, and there is **total internal reflection** for $i \geq i_{c}$, where, $\sin i_{c} = n_{2}/n_{1}$
- eg: for glass-to-air, $i_{c} \approx 41.8\degree$
- the transmitted wave:
$$\vec E_{t} \propto \exp(\vec k_{t} \cdot \vec r - \omega t)$$
- considering the components of the wavevector:
$$\vec k_{t} = k_{tx}\hat x + k_{tz} \hat z$$
- $\omega$ fixes $|\vec k|$ via:
$$k = \frac{\omega n}{c}$$
- $k_\parallel$ must be equal on both sides of the boundary:
$$k_{tx} = k_{ix} = k_{i} \sin i$$
$$\begin{gather}
|\vec k_{t}|^{2} = k_{tx}^{2} + k_{tz}^{2} \\
k_{tz}^{2} = |\vec k_{t}|^{2} - k_{i}^{2} \sin^{2}i
\end{gather}$$
- this is less than $0$ if $k_{i} \sin i > |\vec k_{t}|$
$$k_{tz} = \pm i \sqrt{k_{i}^{2}\sin^{2}i - |\vec k_{t}|^{2}}$$
- **note:** $i$ represents both $\sqrt{-1}$ and the incidence angle, but incidence angle is always an argument of $\sin$, or a subscript
- to avoid confusion, defining $\kappa:$
$$\begin{align*}
\kappa^{2} &= k_{i}^{2} \sin^{2} i - |\vec k_{t}|^{2} \\
&= \frac{\omega^{2}}{c^{2}} (n_{1}^{2} \sin^{2} i - n_{2}^{2})
\end{align*}$$
$$\therefore \vec E_{t} \propto \exp(-\kappa z) \exp(i(k_{tx} x - \omega t))$$
- this is called an **'evanescent'** wave, which means it is decaying, $\exp(-\kappa z)$

- eg: for glass/air, $n_{1} = 1.5$ and $n_{2} = 1$
- the critical angle, $i_{c} \approx 41.8\degree$
- considering a $45\degree$ reflector:
$$\kappa  = \frac{2\pi}{\lambda_{0}} \sqrt{1.5^{2} \sin^{2} 45\degree - 1^{2}} \approx \frac{2.2}{\lambda_{0}}$$
- the z-dependence:
$$\exp(-\kappa z) \approx \exp\left(\frac{-z}{10.45\,\lambda_{0}}\right)$$
