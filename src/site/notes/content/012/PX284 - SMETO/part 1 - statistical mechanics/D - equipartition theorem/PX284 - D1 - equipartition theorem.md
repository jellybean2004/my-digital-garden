---
{"dg-publish":true,"permalink":"/content/012/px-284-smeto/part-1-statistical-mechanics/d-equipartition-theorem/px-284-d1-equipartition-theorem/","noteIcon":"1","created":"2024-11-25T10:50:32.000+00:00","updated":"2024-12-23T21:41:53.457+00:00"}
---

- suppose, $E(x) = \alpha x^{2}$, where $\alpha$ is a constant, $E$ is in the **classical limit**, and $x \in [-\infty, + \infty]$
- in this case, the [[content/012/PX284 - SMETO/part 1 - statistical mechanics/C - entropy and temperature/PX284 - C3 - boltzmann distribution\|boltzmann distribution]] can be written as: 
$$P(x) =  \frac{e^{-\beta \alpha x^{2}}}{\int_{-\infty}^{+\infty} e^{-\beta \alpha x^{2}}\,dx}$$
- the average energy is: 
$$\langle{E}\rangle = \int_{-\infty}^{+\infty} E(x) P(x) \,dx = \frac{\int_{-\infty}^{+\infty}\alpha x^{2} e^{-\beta \alpha x^{2}}\,dx}{{\int_{-\infty}^{+\infty} e^{-\beta \alpha x^{2}}\,dx}} = \frac{1}{2\beta} = \frac{1}{2}k_{B}T$$
- standard gaussian integrals:
$$\begin{align*}
\int_{-\infty}^{+\infty} e^{-\beta \alpha x^{2}}\,dx &= \sqrt{\frac{\pi}{2a}} \\
\int_{-\infty}^{+\infty} x^2e^{-\beta \alpha x^{2}}\,dx &= \frac{1}{2}\sqrt{\frac{\pi}{2a^{3}}}
\end{align*}$$

- in general, for a system with $n$ independent quadratic modes or degrees of freedom, ie: $E= \alpha_{1}x_{1}^{2} + \alpha_{2}x_{2}^{2} \dots + \alpha_{n}x_{n}^{2}$, the expected energy is given by:
$$\langle{E}\rangle = \frac{n}{2}k_{B}T$$
- this called is the **equipartition theorem**

>[!info] equipartition theorem
>for a system in contact with a reservoir at temperature $T$, each independent quadratic energy term in the energy (mode) contributes $\frac{1}{2}k_{B}T$ to the average energy

- eg:
	- for the energy of a [[content/012/PX262 - quantum mechanics/term 1/B - introduction/PX262 - B6 - 1D harmonic oscillator\|1D harmonic oscillator]], there are two quadratic terms:
$$ E = kx^{2} + \frac{1}{2}mv^{2}$$
	- therefore there are two modes of freedom, and the average energy:
$$\langle{E }\rangle =k_{B}T$$

- the internal energy $(U)$ is associated with the average energy $(\langle{E}\rangle)$, so: 
$$C_{V} = \left(\frac{\partial U}{\partial T}\right)_{V}= \frac{n}{2} k_{B}$$
