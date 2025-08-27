---
{"dg-publish":true,"permalink":"/content/012/px-262-quantum-mechanics/term-2/j-atoms-and-molecules/px-262-j4-interacting-electrons-and-nuclei-in-matter/","noteIcon":"1","created":"2025-08-27T13:15:23.312+01:00","updated":"2025-03-13T12:30:36.000+00:00"}
---

- the total energy is the sum of the kinetic energies of electrons and nuclei, and the interactions between electrons and nuclei, all pairs of electrons, and all pairs of nuclei
- even for simple approximations, [[content/012/PX262 - quantum mechanics/term 1/B - introduction/PX262 - B2 - time-independent schrödinger equation\|TISE]] needs approximations and computational methods
- TISE for electrons (neglecting the KE of the protons:)
$$\hat H_{w} \phi_{\lambda} = E_{\lambda}\phi_{\lambda}$$
- anti-symmetry from the [[content/012/PX284 - SMETO/part 1 - statistical mechanics/L - exchange symmetry/PX284 - L2 - pauli exclusion principle\|pauli exclusion principle]]:
$$\phi_{\lambda}(\vec r_{1}, \sigma_{1}, \vec r_{2}, \sigma_{2}) = - \phi_{\lambda}(\vec r_{2}, \sigma_{2}, \vec r_{1}, \sigma_{1})$$
- a helium atom has 2 electrons, 1 nucleus:
$$\begin{align*}
\hat H &= \left(- \frac{\hbar^{2}\nabla_{1}^{2}}{2m_{e}} - \frac{2e^{2}}{4\pi\varepsilon_{0}r_{1}}\right) + \left(- \frac{\hbar^{2}\nabla_{2}^{2}}{2m_{e}} - \frac{2e^{2}}{4\pi\varepsilon_{0}r_{2}}\right) + \frac{e^{2}}{4\pi\varepsilon_{0}|\vec r_{1}-r_{2}|} \\
\hat H &= \hat H_{1}(\vec r_{1}) + \hat H_{2}(\vec r_{2}) + \hat V_{ee}(|\vec r_{1}- \vec r_{2}|)
\end{align*}$$
- if $\vec V_{ee}$ is ignored, the ground state wave function is:
$$\phi_{gs}(\vec r_{1}, \sigma_{1}, \vec r_{2}, \sigma_{2}) = \phi_{100}(\vec r_{1}) \phi_{100}(\vec r_{2}) \times (\uparrow\downarrow)$$
- the spin states:
$$(\uparrow \downarrow) = u_{1\uparrow} u_{2\downarrow} - u_{2\uparrow}u_{1\downarrow}$$

$$\begin{gather}
\hat H_{1}(\vec r_{1}) \phi_{100}(\vec r_{1}) = - \frac{13.6}{1^{2}}2^{2} \phi_{100}(\vec r_{1}) \\\\
\therefore \bigg[\hat H_{1}(\vec r_{1}) + \hat H_{2}(\vec r_{2}) \bigg]\phi_{100}(\vec r_{1}) \phi_{100}(\vec r_{2}) = - \frac{13.6}{1^{2}}2^{2}\times 2 \phi_{100}(\vec r_{1})\phi_{100}(\vec r_{2}) \\\\
E_{gs}= -108.8\,\text{eV}
\end{gather}$$

- when $\hat V_{ee}$ is included, $E_{gs}= -79.9$ eV
- one electron screens the nuclear charge from the other
