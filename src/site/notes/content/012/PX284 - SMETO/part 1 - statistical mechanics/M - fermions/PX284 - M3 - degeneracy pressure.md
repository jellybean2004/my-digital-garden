---
{"dg-publish":true,"permalink":"/content/012/px-284-smeto/part-1-statistical-mechanics/m-fermions/px-284-m3-degeneracy-pressure/","noteIcon":"1","created":"2025-08-27T13:15:24.875+01:00","updated":"2025-02-03T19:37:16.000+00:00"}
---

- pressure due to the electron gas at $T=0$
$$\begin{align*}
\langle{E}\rangle &= \frac{U}{N} = \frac{\int_{0}^{\infty} Eg(E)f_{FD}(E)\,dE}{\int_{0}^{\infty} g(E)f_{FD}(E)\,dE} \\
&= \frac{\int_{0}^{E_{F}} Eg(E)\,dE}{\int_{0}^{E_{F}} g(E)\,dE} \\
&\approx \frac{\int_{0}^{E_{F}} E\,E^{1/2}\,dE}{\int_{0}^{E_{F}} E^{1/2}\,\,dE} \\
&\approx \frac{E_{F}^{5/2}/(5/2)}{E_{F}^{3/2}/(3/2)}\\
\therefore \langle{E}\rangle&\approx \frac{3}{5}E_{F}
\end{align*}$$
	where, $g(E) \sim E^{1/2}$

- the internal energy:
$$U = \frac{3N}{5}E_{F}$$
- from equation $(1)$ in [[content/012/PX284 - SMETO/part 1 - statistical mechanics/M - fermions/PX284 - M2 - fermi energy\|fermi energy]]:
$$\begin{gather}
U \propto V^{-2/3} \\
\ln U = - \frac{2}{3} \ln V + \text{constant}\\
\frac{dU}{U} = - \frac{2}{3} \frac{dV}{V}
\end{gather}$$
- using the [[content/011/PX154 - physics foundations/PX154 - D - the first law of thermodynamic/PX154 - D2 - the first law\|first law of thermodynamics]]:
$$p = - \left(\frac{\partial U}{\partial V}\right)_{S} = \frac{2}{3} \frac{U}{V} = \frac{2}{5} nE_{F}$$
- this is the **degeneracy pressure**
