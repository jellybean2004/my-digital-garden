---
{"dg-publish":true,"permalink":"/content/012/px-262-quantum-mechanics/term-2/l-relativity-and-quantum-mechanics/px-262-l1-klein-gordon-equation/","noteIcon":"1","created":"2025-03-06T10:10:11.529+00:00","updated":"2025-03-10T11:46:51.163+00:00"}
---

- looking at the schrodinger equation for a free particle:
$$i \hbar \frac{\partial \psi}{\partial t} = - \frac{\hbar^{2}}{2m} \nabla^{2}\psi$$
- the plane wave solution:
$$\begin{gather}
\psi = A\exp\left(i \left(\frac{\vec p \cdot \vec r - Et}{\hbar}\right)\right) \\
\vec p = \hbar \vec k \text{ if } E = \frac{p^{2}}{2m}
\end{gather}$$
- this is a classical result

- trying to get a wave equation where $E^{2} = p^{2}c^{2} + m^{2}c^{4}$ comes out, ie. the relativistic mechanics result
$$\begin{gather}
E \to i\hbar \frac{\partial }{\partial t} \\
\vec p \to -i \hbar \vec\nabla 
\end{gather}$$

$$- \hbar^{2} \frac{\partial^{2} { \psi}}{\partial {t}^{2}} = - \hbar c^{2} \nabla^{2} \psi + m^{2}c^{4} \psi $$
- this is called the **klein-gordon equation**
$$\begin{gather}
\psi = A \exp\left(i\left(\frac{\vec p \cdot \vec r - Et}{\hbar}\right)\right) \\
 E^{2} = p^{2}c^{2}+ m^{2}c^{4} \\
 E = \pm \sqrt{p^{2}c^{2} + m^{2}c^{4}}
\end{gather}$$
- in classical mechanics, the negative energy solutions can be discarded
- in quantum mechanics, all the solutions are needed to form a complete set of states
- the probability density, $\rho(\vec r, t) = \psi^{*}\psi$, is found to be proportional to the energy, which is unphysical for the negative energy solutions
