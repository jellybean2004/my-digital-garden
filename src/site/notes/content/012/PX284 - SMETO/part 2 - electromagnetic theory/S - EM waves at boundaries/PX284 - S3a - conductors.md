---
{"dg-publish":true,"permalink":"/content/012/px-284-smeto/part-2-electromagnetic-theory/s-em-waves-at-boundaries/px-284-s3a-conductors/","noteIcon":"1","created":"2025-08-27T13:15:28.797+01:00","updated":"2025-03-14T07:05:19.000+00:00"}
---

- no free charge, but there may be free current:
$$\begin{gather}
\rho_{f} = 0 \\
\vec J_{f} \neq 0
\end{gather}$$
- assuming linear and isotropic medium:
$$\begin{gather}
\vec D = \varepsilon \vec E  \\
\vec D = \mu \vec H \\
\vec J_{f} = g \vec E
\end{gather}$$
	where, $g$ is conductivity
- assuming that $\varepsilon$, $\mu$ and $g$ are scalars, ie. they don't depend on the field strength, but may depend on $\omega$
$$\begin{align*}
\vec\nabla\times (\vec\nabla\times\vec  E) &= \vec\nabla (\vec\nabla\cdot\vec  E) - \nabla^{2} \vec E \\
&= - \frac{\partial }{\partial t} (\vec\nabla\times \mu \vec H) \\
&= - \mu \frac{\partial }{\partial t} (g\vec E) - \mu \varepsilon_{0} \frac{\partial^{2} {\vec E}}{\partial {t}^{2}} \\
\nabla^{2} \vec E &= \mu g \frac{\partial \vec E}{\partial t} + \mu \varepsilon \frac{\partial^{2} {\vec E}}{\partial {t}^{2}}
\end{align*}$$
- looking for plane wave solutions:
$$\vec E = \vec E_{0} \exp(i(\vec k \cdot \vec r - \omega t))$$
$$\begin{gather}
\vec\nabla \to i \vec k \\
\frac{\partial }{\partial t} \to -i\omega
\end{gather}$$
$$\implies k^{2} = i\mu\omega g + \mu \varepsilon\omega^{2}$$
- this is the dispersion relation

- considering good conductors, at frequencies, $\omega \ll g/\varepsilon$, can neglect the second term
$$\begin{gather}
k^{2} \simeq i\mu g\omega \\
	k = \pm \frac{1+i}{\sqrt{2}} \sqrt{\mu g \omega} = \pm \frac{1+i}{\delta}
\end{gather}$$
	where, $\delta= \sqrt{2/\mu g\omega}$, is called the 'skin depth'
- for a wave propagating in $\vec x$-direction:
$$\vec E = \vec E_{0} \exp(i(kx - \omega t)) = \vec E_{0} \exp\left(-\frac{x}{\delta}\right) \exp\left(i\left( \frac{x}{\delta} - \omega t\right)\right)$$
- this is a decaying solution

$$\begin{gather}
\vec k \cdot \vec E = 0 \\
\vec k \times \vec E = \omega\mu \vec H
\end{gather}$$
- $\vec k$, $\vec E$ and $\vec H$ are all perpendicular to each other
- the impedance: 
$$Z_{c} = \frac{E}{H} = \frac{\omega\mu}{k} =\frac{\omega\mu\delta}{i+1} = \frac{\omega\mu\delta}{\sqrt{2}} \exp\left(- \frac{i\pi}{4}\right)$$
- $\vec H$ is out of phase with $\vec E$ by $\pi/4$
$$\begin{gather}
\vec E = E_{0} \hat z \exp(i(-kr - \omega t)) \\
\vec H = H_{0}  \hat \theta  \exp(i(-kr - \omega t))
\end{gather}$$
- $\vec k$ is the direction of $- \hat r$, ie. into the wire
$$\begin{gather} 
k = \frac{1+i}{\delta} \\
\vec E = E_{0} \hat z \exp\left(\frac{e}{\delta}\right) \exp\left(i\left(- \frac{r}{\delta} - \omega t\right)\right)
\end{gather}$$
- growing with $r$ up to $r = r_{0}$
- current flows in a cylindrical shell of thickness $\delta$ of edge of the wire
- this is called the **skin effect**
