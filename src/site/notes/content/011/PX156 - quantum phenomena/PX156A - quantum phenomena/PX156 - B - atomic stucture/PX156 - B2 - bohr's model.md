---
{"dg-publish":true,"permalink":"/content/011/px-156-quantum-phenomena/px-156-a-quantum-phenomena/px-156-b-atomic-stucture/px-156-b2-bohr-s-model/","noteIcon":"1","created":"2025-08-27T13:14:00.841+01:00","updated":"2024-12-03T17:09:22.000+00:00"}
---

- electrons orbit around the nucleus
## quantized angular momentum
- orbiting electrons are standing waves, the orbits must be whole number multiples of the wavelength: 
$$\begin{align*}
		2\pi r &= n\lambda \\
		&= \frac{nh}{p} \\
		&= \frac{nh}{m_{e}v} \\
		m_{e}vr = L &= \frac{nh}{2\pi} = n\hbar 
	\end{align*}$$
## bohr radius
$$v_{n} = \frac{nh}{2\pi m_{e}r_{n}}$$
- acceleration is caused due to electrostatic interaction, so from [[content/011/PX157 - electricity and magnetism/PX157 - A - coulomb's law/PX157 - A2 - coulomb's law\|coulomb's law]] : 
$$\begin{align*}
	F_{E} &= F_{c} \\
	\frac{e^{2}}{4\pi\epsilon_{0}r_{n}^{2}} &=  \frac{m_{e} v_{n}^{2}}{r_{n}} \\
	&= \frac{n^{2}h^{2}}{4\pi^{2} m_{e}r_{n}^{3}} \\
	\therefore r_{n}&= \frac{\epsilon_{0}n^{2}h^{2}}{\pi m_{e}e^{2}}
\end{align*}$$
- bohr's radius $(a_{0}):$ 
$$\begin{align*}
	a_{0} &= \frac{\epsilon_{0}h^{2}}{\pi m_{e}e^{2}} \\
	r_{n} &= a_{0}n^{2} \\
	v_{n} &= \frac{e^{2}}{2n\epsilon_{0}h}
\end{align*}$$
$$\begin{align*}
	E_{n} &= KE + PE \\
	&= \frac{1}{2}m_{e}v_{n}^{2} - \frac{e^{2}}{4\pi\epsilon_{0} r_{n}} \\
	&= \frac{m_{e}}{2} \frac{e^{4}}{4n^{2}\epsilon_{0}h^{2}} - \frac{e^{2}}{4\pi\epsilon_{0}} \frac{\pi m_{e}e^{2}}{\epsilon_{0}n^{2}h^{2}}\\
	&= - \frac{m_{e}e^{4}}{8\epsilon_{0}^{2}n^{2}h^{2}}
\end{align*}$$
- comparing it with the *rydberg formula*: 
$$E = \frac{hc}{\lambda} = hc R\left(\frac{1}{m^{2}}- \frac{1}{n^{2}}\right)$$
$$R = 1.097\times10^{7} \,m^{-1} = \frac{m_{e}e^{4}}{8\epsilon_{0}^{2}h^{3}c}$$
- rydberg units of energy: 
	- ${} Rhc \approx 13.6\,eV {}$
	- $E_{n}\approx -\frac{13.6}{n^{2}}\,eV$