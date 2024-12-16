---
{"dg-publish":true,"permalink":"/content/011/px-157-electricity-and-magnetism/px-157-d-induction/px-157-dx1-displacement-current/","noteIcon":"1","created":"2024-10-01T18:27:10.260+01:00","updated":"2024-11-26T20:11:05.082+00:00"}
---

![Pasted image 20240322164551.png](/img/user/pics/Pasted%20image%2020240322164551.png)
$$
\int_{C}\vec B\cdot d\vec l = \mu_{0}I = \mu_{0}\iint \vec J \cdot d\vec S
$$
- surface $A_{2}$ goes between the capacitor plates, but is still bounded by the curve $C:$
$$
\oint_{C}\vec B \cdot d\vec l = 0
$$
- both results **cannot** be true at the same time
- there is an electric field between the plates, from [[content/011/PX157 - electricity and magnetism/PX157 - B - electric fields/I - field/PX157 - B5a - gauss's law\|PX157 - B5a - gauss's law]]:
$$
\phi_{E}= \iint_{A_{2}} \vec E\,d\vec S = \frac{Q}{\epsilon_{0}}
$$
- a current is defined as $I= \frac{dQ}{dt}:$
$$
I_{D}= \epsilon_{0} \frac{d\phi_{E}}{dt}
$$
	- compable with $\epsilon = - \frac{d\phi_{B}}{dt}$ 
$$
I_{D}= \epsilon_{0} \frac{d\phi_{E}}{dt} = \epsilon_{0} \frac{d}{dt}\iint_{S}\vec E\cdot d\vec S
$$
- adding $I_{D}$ to [[content/011/PX157 - electricity and magnetism/PX157 - C - magnetic fields/PX157 - C4a - ampere's law\|PX157 - C4a - ampere's law]]:
$$
\oint_{C}\vec B\cdot d\vec l = \mu_{0}I + \mu_{0}I_{D} = \mu_{0}I + \mu_{0} \epsilon_{0} \frac{d\phi_{E}}{dt}
$$
- for surface $A_{1}:$
$$
\oint \vec B \cdot d\vec l = \mu_{0}I
$$
- for surface $A_{2}:$
$$
\oint \vec B \cdot d\vec l = \mu_{0}I_D
$$
- between the capacitor plates: magnetic field is induced in the azimuthal direction
## how important is the displacement current?
- consider a solenoid with an oscillating current:
$$
I_{s}(t) = I_{0}\cos(\omega t)
$$
$$
\vec B = \mu_{0}nI_{s}(t)\hat z
$$
- solenoid has a cross-section, $\pi a^{2}$
- [[content/011/PX157 - electricity and magnetism/PX157 - D - induction/PX157 - D1a - faraday's law\|faraday's law]] (static) over a circular path with radius, $R$:
$$\begin{align*}
	\oint \vec E \cdot d\vec l &= - \frac{d\phi_{B}}{dt} \\
	E_{\phi}2\pi R &= -\mu_{0}n \frac{dI_{S}}{dt}\pi a^{2} \\
	E_{\phi}(t) &= - \frac{1}{2}\mu_{0}n \frac{a^{2}}{R} \frac{dI_{S}}{dt}
\end{align*}$$
- [[content/011/PX157 - electricity and magnetism/PX157 - B - electric fields/I - field/PX157 - B4a - electric flux\|PX157 - B4a - electric flux]]:
$$
\phi_{E}= \int_{0}^{L}dz \int_{R_{1}}^{R_{2}}dR\, E_{\phi} = - \frac{1}{2}\mu_{0}n a^{2}L \ln\left(\frac{R_{2}}{R_{1}}\right) \frac{dI_{S}}{dt}
$$
- displacement current:
$$
I_{D}(t) = \epsilon_{0} \frac{d\phi_{E}}{dt} = -\frac{1}{2}\mu_{0}\epsilon_{0}na^{2}L \ln\left(\frac{R_{2}}{R_{1}}\right)\omega^{2}I_{S}
$$
$$
\frac{|I_{D}|}{|I_{S}|} = \frac{1}{2}na^{2}L\ln\left(\frac{R_{2}}{R_{1}}\right) \cdot \mu_{0}\epsilon_{0} \cdot\omega^{2}= \left(\frac{\lambda\omega}{c}\right)^{2}
$$
- $I_{D}$ is important if $\lambda$ is large, or $\omega$ is large

- eg: of large $\lambda:$ jupiter-io
