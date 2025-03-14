---
{"dg-publish":true,"permalink":"/content/012/px-284-smeto/part-2-electromagnetic-theory/s-em-waves-at-boundaries/px-284-s3b-reflections-on-boundaries-with-metals/","noteIcon":"1","created":"2025-03-13T17:46:18.090+00:00","updated":"2025-03-13T17:55:34.022+00:00"}
---

- considering normal incidence, ie: $i = r= t = 0$, and p-polarization:
$$\begin{gather}
H_{i} - H_{r} = H_{t} \\ 
E_{i} + E_{r} = E_{t}
\end{gather}$$
- in the limit of perfect conductor, $g \to \infty:$
$$\begin{gather}
E_{t} = 0 \\
E_{r} = - E_{i} \\
r = \frac{E_{r}}{E_{i}} = -1 \\
t = \frac{E_{t}}{E_{i}}= 0
\end{gather}$$
- for good conductors:
$$\begin{gather}
\frac{E_{i}}{Z_{1}}- \frac{E_{r}}{Z_{1}} = \frac{E_{t}}{Z_{2}} \\
E_{i} + E_{r} = E_{t} = \frac{Z_{2}}{Z_{1}}(E_{i}- E_{r}) \\
\left(1- \frac{Z_{2}}{Z_{1}}\right) E_{i} = \left(1 +\frac{ Z_{2}}{Z_{1}}\right)E_{r} \\
r = \frac{E_{r}}{E_{i}}= \frac{Z_{2}-Z_{1}}{Z_{2}+Z_{1}}
\end{gather}$$
- for air-metal boundary: $Z_{1} \approx Z_{0} \approx 377\,\omega$
$$Z_{2} = Z_{c} = \frac{\mu\omega\delta}{2} (1-i) = \sqrt{\frac{\mu\omega}{2g}} (1-i)$$
- considering $\omega = 2\pi \times 2\times10^{6}$ rad s$^{-1}$
$$|Z_{c}| \simeq 7.3\times10^{4}\,\Omega$$
$$\frac{Z_{C}}{Z_{0}} \simeq 10^{-6} $$
$$r = - \frac{1- \frac{Z_C}{Z_{0}}}{1+ \frac{Z_{C}}{Z_{0}}} \simeq \left(1 - \frac{2Z_{c}}{Z_{0}}\right)$$
	where, $1$ is the perfect conductor limit, and the additional term is the small correction
