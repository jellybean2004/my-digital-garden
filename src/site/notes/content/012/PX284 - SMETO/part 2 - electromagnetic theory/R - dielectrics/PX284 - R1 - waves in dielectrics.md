---
{"dg-publish":true,"permalink":"/content/012/px-284-smeto/part-2-electromagnetic-theory/r-dielectrics/px-284-r1-waves-in-dielectrics/","noteIcon":"1","created":"2025-02-27T15:51:36.287+00:00","updated":"2025-03-10T08:13:16.634+00:00"}
---

- [[content/012/PX284 - SMETO/part 2 - electromagnetic theory/Q - maxwell's equations in matter/PX284 - Q3 - maxwell's equations in matter\|maxwell's equations in matter]] with no sources, ie: $\rho_{f} - \vec J_{f} = 0$, for linear, isotropic materials

$$\begin{gather}
\vec\nabla\times\vec  E = - \frac{\partial \vec B}{\partial t} \\\\
\vec\nabla \times (\vec\nabla \times \vec E) = \vec\nabla (\vec\nabla\cdot\vec  E) - \nabla^{2}\vec E= -\frac{\partial }{\partial t} (\vec\nabla \times \vec B) \\
- \nabla^{2} \vec E = - \mu_{0} \mu_{r} \frac{\partial^{2} {}}{\partial {t}^{2}}\vec D= - \mu_{0}\varepsilon_{0} \mu_{r}\varepsilon_r \frac{\partial^{2} {}}{\partial {t}^{2}}\vec E
\end{gather}$$


- this is a wave equation:
$$\nabla^{2} \vec E = \frac{1}{v^{2}} \frac{\partial^{2} {\vec E}}{\partial {t}^{2}}$$
- the wave speed:
$$v = \frac{1}{\sqrt{\mu_{0}\varepsilon_{0}\mu_{r}\varepsilon_{r}}} = \frac{c}{\sqrt{\mu_{r}\varepsilon_{r}}}= \frac{c}{n}$$
- $n = \sqrt{\mu_{r}\varepsilon_{r}}$ is called the **refractive index**
- for most transparent matter (allowing propagation of EM waves), $\mu_{r} \simeq 1$, so $n \simeq \sqrt{\varepsilon_{r}}$
- $\epsilon_r$ is frequency dependent

- plane waves in matter (linear, isotropic response)
$$\begin{gather}
\vec E = E_{0} \exp(i (\vec k \cdot \vec x - \omega t))\, \hat E \\
\vec H = H_{0} \exp(i (\vec k \cdot \vec x - \omega t))\, \hat H\\\\
\vec\nabla  \implies i\vec k \\
\partial_{t} \implies - i\omega
\end{gather}$$
- maxwell's equations with no free charges or currents :
$$\begin{gather}
\vec k \cdot \vec D = 0 \\
\vec k \cdot \vec B = 0 \\
\vec k \times \vec E = \omega \vec B \\
\vec k \times \vec H = - \omega \vec D
\end{gather}$$
- as in free space: $\vec k \perp \vec E, \vec H$ and $\vec E \perp \vec H$
$$E_{0} = \frac{\omega B_{0}}{|\vec k|} = vB_{0} = v \mu_{0}\mu_{r} H_{0}$$
- defining the **impedance**:
$$Z = \frac{E_{0}}{H_{0}} = v\mu_{0}\mu_{r} = \sqrt{\frac{\mu_{0}\mu_{r}}{ \varepsilon_{0}\varepsilon_{r}}} = Z_{0} \sqrt\frac{\mu_{r}}{\varepsilon_{r}}$$
	where, $Z_{0} \simeq 376.73\,\Omega$ is the impedance of free space

- in materials with $\mu_{r}\simeq 1:$
$$ Z \simeq \frac{Z_{0}}{\sqrt{\varepsilon_{r}}} \simeq \frac{Z_{0}}{n}$$
- 