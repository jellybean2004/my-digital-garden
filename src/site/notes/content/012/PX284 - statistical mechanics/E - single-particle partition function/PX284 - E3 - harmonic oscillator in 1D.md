---
{"dg-publish":true,"permalink":"/content/012/px-284-statistical-mechanics/e-single-particle-partition-function/px-284-e3-harmonic-oscillator-in-1-d/","noteIcon":"1","created":"2024-11-29T17:03:05.459+00:00","updated":"2024-12-23T22:49:56.088+00:00"}
---

- considering a [[content/012/PX284 - statistical mechanics/E - single-particle partition function/PX284 - E3 - harmonic oscillator in 1D\|harmonic oscillator in 1D]], the energy of states is:
$$E_{n} = \left(n + \frac{1}{2}\right)\hbar \omega$$
- the partition function:
$$\begin{align*}
	Z &= \sum\limits_{n} \exp\left(-\beta\left(n + \frac{1}{2}\right)\hbar \omega\right) \\
	&= \exp\left(- \frac{\beta\hbar\omega}{2}\right) \sum\limits_{n} \exp(- \beta\hbar\omega n)
\end{align*}$$
- the above sum looks like a geometric series:
$$a \sum\limits_{n}^{\infty} r^{n} = \frac{a}{1-r}$$
	with $a = \exp(-\beta\hbar\omega/2)$ , and $r - \exp(-\beta\hbar\omega)$
- therefore, it can be rewritten as:
$$\begin{align*}
	Z &= \frac{\exp\left(-{\beta\hbar\omega/2}\right)}{1-\exp\left(-\beta\hbar\omega\right)} \\
	\ln Z &= - \frac{\beta\hbar\omega}{2}-\ln(1-\exp(-\beta\hbar\omega))
\end{align*}$$

- thus, the internal energy:
$$U = - \frac{d\ln{Z}}{d\beta} = \hbar\omega \left[\frac{1}{2} + \frac{1}{\exp(\beta\hbar\omega)-1} \right]$$

- the heat capacity: 
$$C_{V} = \left(\frac{\partial U}{\partial T}\right)_{V} = k_{B} (\beta\hbar\omega)^{2} \frac{\exp({\beta\hbar\omega})}{(\exp(\beta\hbar\omega)-1)^{2}}$$
- at very high temperatures, ${} \beta\hbar\omega \ll 1: {}$
$$\implies \exp(\beta\hbar\omega) = 1+ \beta\hbar\omega$$
$$C_{V} = k_{B} \left(\frac{\beta\hbar\omega}{\beta\hbar\omega}\right)^{2} = k_{B}$$
- this is in keeping with the [[content/012/PX284 - statistical mechanics/D - equipartition theorem/D - equipartition theorem\|equipartition theorem]]

![PX284 - E3 - harmonic oscillator in 1D.png|100%](/img/user/pics/PX284%20-%20E3%20-%20harmonic%20oscillator%20in%201D.png)
*image: P. Goddard, lecture notes*