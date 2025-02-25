---
{"dg-publish":true,"permalink":"/content/012/px-275-mathematical-methods/term-2/i-optics/px-275-i5-different-path-lengths/","noteIcon":"1","created":"2025-02-25T12:42:07.893+00:00","updated":"2025-02-25T12:55:39.517+00:00"}
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
