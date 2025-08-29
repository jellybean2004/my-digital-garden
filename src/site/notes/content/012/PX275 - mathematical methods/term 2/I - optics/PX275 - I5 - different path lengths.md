---
{"dg-publish":true,"permalink":"/content/012/px-275-mathematical-methods/term-2/i-optics/px-275-i5-different-path-lengths/","noteIcon":"1","created":"2025-08-27T13:15:24.010+01:00","updated":"2025-04-29T17:42:18.000+01:00"}
---

- different path lengths lead to phase differences
- considering two pinholes, hole 1 at the origin, and hole 2 at position, $\vec y$
- at a point $\vec x$ on the detector:
$$\begin{gather}
l_{1}  = |\vec x - \vec y^{1}| = |\vec x| \\
l_{2} = |\vec x - \vec y^{2}| = |\vec x - \vec y| \\\\
\Delta \phi = (l_{2}- l_{1}) k = k(|\vec x - \vec y| - |\vec x|)
\end{gather}$$
	where, $\Delta \phi$ is the phase difference

$$\begin{align*}
|\vec x - \vec y | &= \sqrt{(\vec x - \vec y) (\vec x - \vec y)} \\
&= \sqrt{|\vec x^{2}| - 2\vec x \cdot \vec y + |\vec y|^{2}} \\
&= |\vec x| \sqrt{1 - \frac{2\vec x \cdot \vec y}{|\vec x|^{2}} +\frac{ |\vec y|^{2}}{|\vec x|^{2}}}
\end{align*}$$
- considering for **far field regime**: the detector distance, $D \gg$ size of the aperture/detector screen
- this is also called **fraunhofer diffraction**, as opposed to the **near field regime** - **fresnel diffraction**
$$\therefore |\vec x| \gg |\vec y| \implies |\vec x - \vec y | \simeq |\vec x| \sqrt{1 - \epsilon}$$
	where, $\epsilon ={2\vec x \cdot \vec y}/{|\vec x|^{2}}$
- using taylor expansion:
$$\begin{gather}
\sqrt{1 - \epsilon} \simeq 1 - \frac{1}{2}\epsilon + 0 (\epsilon^{2})+ \dots  \\
\therefore |\vec x - \vec y| \simeq |\vec x| \left(1 - \frac{\vec x \cdot \vec y}{|\vec x|^{2}}\right)
\end{gather}$$
$$\therefore \Delta \phi = k \left(|\vec x| \left(1 - \frac{\vec x \cdot \vec y}{|\vec x|^{2}}\right) - |x| \right) = - k \frac{\vec x \cdot \vec y}{|\vec x|^{2}}$$
- defining a wavevector:
$$\vec  k = k\,\hat x = k \frac{\vec x}{|\vec x|}$$
- this is also known as the '**scattering wavevector**', and points towards the observation point
$$\therefore \Delta \phi = - \vec k \cdot \vec y$$

- for a single point source: 
$$u(\vec x, t) = \frac{A}{|\vec x - \vec y|} \exp(ik (|\vec x - \vec y| - ct))$$
$$k|\vec x - \vec y| = k |\vec x | + \Delta \phi = k|\vec x | - \vec k \cdot \vec y$$

- for a superposition of $N$ point sources:
$$\begin{align*}
u(\vec x, t) &= \sum\limits_{j=1}^{N} \frac{A^{j}}{|\vec x - \vec y^{j}|} \exp(ik(|\vec x - \vec y^{j}| - ct)) \\
&= \sum\limits_{j=1}^{N} \frac{A^{j}}{|\vec x - \vec y^{j}|} \exp(ik|\vec x | - i\vec k \cdot \vec y^{j} - ikct) \\
&= \sum\limits_{j=1}^{N} \frac{A^{j}}{|\vec x - \vec y^{j}|} \exp(ik(|\vec x | - ct) - i\vec k \cdot \vec y^{j})
\end{align*}$$
- in far-field regime: $|\vec x - \vec y^{j}| \simeq D$, so, $\exp(ik(|\vec x | - ct))$ is the same for all sources
$$\therefore u(\vec x , t) = \frac{1}{D} \exp(ik(|\vec x | - ct) ) \sum\limits_{j=1}^{N} A^{j} \exp(- i\vec k \cdot \vec y^{j})$$
- this can be used to model various apertures
- considering an aperture function, $a(\vec y)$, that describes the location of the pinholes, such that $a(\vec y) = 0$ except at the location with holes
- eg: a set of pinholes, each described by a $\delta$ function:
$$a(\vec y) = \sum\limits_{j=1}^{N} A^{j} \delta (\vec y - \vec y^{j})$$
- on a centred circular aperture with radius, $d$:
$$a(\vec y) = \begin{cases} 1 & \text{if } |\vec y| < d, \\
0 & \text{if } |\vec y| \geq d.
\end{cases}$$
- the combined source contribution is an integral over $a(\vec y)$
$$u(\vec x, t) = \frac{1}{D} \exp(ik(|\vec x| - ct )) \iint \exp(- i \vec k \cdot \vec y) \, a(\vec y) \, dy_{1}\,dy_{2}$$
- the above integral is a 2D fourier transform of $a(\vec y)$
- thus, the spatial interference pattern for a given aperture function, $a(\vec y)$, is given by the fourier transform of the aperture function:
$$u(\vec x, t) \propto \tilde a(\vec k)$$
- the corresponding light intensity, $I(x_{1}, x_{2}) \propto |u|^{2} \propto |\tilde a(k)|^{2}$

