---
{"dg-publish":true,"permalink":"/content/012/px-275-mathematical-methods/term-2/i-optics/px-275-i3-point-sources-in-3-d/","noteIcon":"1","created":"2025-02-20T12:29:12.826+00:00","updated":"2025-03-09T11:32:31.072+00:00"}
---

- the 3D wave equation:
$$\frac{\partial^{2} {u}}{\partial {t}^{2}} = c^{2}\,\nabla^{2}u$$
- in spherical coordinates:
$$\begin{gather}
x = r\sin\theta \cos\phi \\
y = r \sin\theta \sin\phi \\
z = r \cos\theta \\
\nabla^{2} = \frac{1}{r^{2}}\frac{\partial }{\partial r}\left(r^{2}\frac{\partial }{\partial r}\right) + \frac{1}{r^{2}\sin\theta} \frac{\partial }{\partial \theta} \left(\sin\theta \frac{\partial }{\partial \theta}\right) + \frac{1}{r^{2}\sin\theta} \frac{\partial^{2} {}}{\partial {\phi}^{2}}
\end{gather}$$
- since the point sources are spherically symmetric, there is no $\theta$ or $\phi$ dependence, only $r$, ie:$u(\vec r, t) = u(r,t)$
- this simplifies $\nabla^{2}$ and the radial wave equation is obtained:
$$\begin{gather}
\left(\frac{1}{r^{2}}\frac{\partial }{\partial r}\left(r^{2} \frac{\partial }{\partial r} \right) - \frac{1}{c^{2}}\frac{\partial^{2} {}}{\partial {t}^{2}}\right) u(r,t) = 0 \\
\frac{2}{r}\frac{\partial u}{\partial r}+ \frac{\partial^{2} {u}}{\partial {r}^{2}} - \frac{1}{c^{2}}\frac{\partial^{2} {u}}{\partial {t}^{2}} = 0
\end{gather}$$
- this is the 1D wave equation with an additional term in the beginning

$$\begin{gather}
\frac{2}{r} \frac{\partial }{\partial r}\left(\frac{v}{r}\right) + \frac{\partial }{\partial r} \frac{\partial }{\partial r}\frac{v}{r} - \frac{1}{c^{2}} \frac{\partial }{\partial t} \frac{\partial }{\partial t} \left(\frac{v}{r}\right) = 0 \\
= \dots = \frac{1}{r} \frac{\partial^{2} {v}}{\partial {r}^{2}} - \frac{1}{c^{2}r} \frac{\partial^{2} {v}}{\partial {r}^{2}} = 0 \\
\implies \frac{\partial^{2} {v}}{\partial {r}^{2}} = \frac{1}{c^{2}}\frac{\partial^{2} {v}}{\partial {t}^{2}}
\end{gather}$$
- this is the 1D wave equation, but for $v$, the solutions for which is:
$$v(r,t) = A\exp(ik(r-ct)) + B\exp(ik(r+ct)) = A'\exp(-ik(r-ct)) + B' \exp(-ik(r+ct))$$
- for sources of light, outward propagating solutions are needed
- so, without loss of generality:
$$ u(r,t) = \frac{A}{r} \exp(ik(r-ct ))$$
- this is the solution for a point source

- separating it into radial and temporal components:
$$u(r,t) = R(r) T(t) = \frac{A}{r} \exp(ikr) \exp(-ikct)$$
- for a stationary source, the time dependence is uniform
- so the intensity patterns have a common time dependence
- it is not possible to calculate the intensity patterns at given locations and for different shape apertures
