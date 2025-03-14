---
{"dg-publish":true,"permalink":"/content/012/px-284-smeto/part-2-electromagnetic-theory/s-em-waves-at-boundaries/px-284-s2b-brewster-s-angle/","noteIcon":"1","created":"2025-03-14T06:27:43.843+00:00","updated":"2025-03-14T06:32:57.077+00:00"}
---

- considering a boundary with $n_{2}>n_{1}$
- by [[content/012/PX284 - SMETO/part 2 - electromagnetic theory/S - EM waves at boundaries/PX284 - S1 - snell's law\|snell's law]]:
$$\sin t = \frac{n_{1}}{n_{2}}\sin i \implies t \leq i$$
- for normal incidence, ie. $i = t = 0:$
$$r_{s} = \frac{n_{1}-n_{2}}{n_{1}+n_{2}} = r_{p} <0$$
- for oblique incidence $(i = 90\degree):$
$$\begin{gather}
r_{s} = - \frac{n_{2}\cos{t}}{n_{2}\cos t} = -1 \\
r_{p} = \frac{n_{1}\cos{t}}{n_{1}\cos t} = +1
\end{gather}$$

- the **brewster angle** is the value of $i$ at which $r_{p} = 0$
$$\begin{gather}
n_{1} \cos t_{B} = n_{2} \cos i_{B} \; \text{(fresnel)} \\
n_{1}\sin i_{B} = n_{2} \sin t_{B} \;\text{(snell)} \\\\
n_{1}^{2}\cos^{2}t_{B} = n_{2}^{2} \cos^{2} i_{B} \\
n_{1}^{2}\sin^{2}i_{B} = n_{2}^{2}\sin^{2} t_{B}  \\\\
\implies n_{1}^{2}n_{2}^{2} = n_{1}^{4} \sin^{2}i_{B} + n_{2}^{4} \cos^{2}i_{B} \\
n_{1}^{2}n_{2}^{2}( 1+ \tan^{2} i_{B}) = n_{1}^{4} \tan^{2}i_{B} + n_{2}^{4} \\
n_{1}^{2}\tan^{2}i_{B} ( n_{2}^{2} - n_{1}^{2}) = (-n_{1}^{2} + n_{2}^{2}) n_{2}^{2} \\\\
\therefore \tan i_{B} = \frac{n_{2}}{n_{1}}
\end{gather}$$
- at $i_B$, $r_{p} =0$
- therefore, any reflected light must be s-polarized

- for air-to-glass: $n_{1}/n_{2} \approx 1/1.5 \implies i_{B} \approx 56.3\degree$
- for air-to-water: $n_{1}/n_{2} \approx 1/1.33 \implies i_{B} \approx 53.1\degree$
- the applications:
	- polarized sunglasses: road glare, mostly s-polarized, filter to allow only p-polarization to pass through
	- polarized filters on cameras