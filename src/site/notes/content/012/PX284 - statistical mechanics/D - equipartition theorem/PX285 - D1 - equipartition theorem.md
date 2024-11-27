---
{"dg-publish":true,"permalink":"/content/012/px-284-statistical-mechanics/d-equipartition-theorem/px-285-d1-equipartition-theorem/","created":"2024-11-25T10:50:32.000+00:00","updated":"2024-11-27T18:01:11.997+00:00"}
---

- suppose, $E(x) = \alpha x^{2}$, where $\alpha$ is a constant, $E$ is in the **classical limit**, and $x \in [-\infty, + \infty]$
- in this case, the [[content/012/PX284 - statistical mechanics/C - entropy and temperature/PX285 - C3 - boltzmann distribution\|boltzmann distribution]] is written as: 
$$P(x) =  \frac{e^{-\beta \alpha x^{2}}}{\int_{-\infty}^{+\infty} e^{-\beta \alpha x^{2}}\,dx}$$
- the average energy is: 
$$\langle{E}\rangle = \int_{-\infty}^{+\infty} E(x) P(x) \,dx = \frac{\int_{-\infty}^{+\infty}\alpha x^{2} e^{-\beta \alpha x^{2}}\,dx}{{\int_{-\infty}^{+\infty} e^{-\beta \alpha x^{2}}\,dx}} = \frac{1}{2\beta} = \frac{1}{2}k_{B}T$$

- in general, for a system with $n$ independent quadratic modes or degrees of freedom, ie: $E= \alpha_{1}x_{1}^{2} + \alpha_{2}x_{2}^{2} \dots + \alpha_{n}x_{n}^{2}$, then the expected energy is given by:
$$\langle{E}\rangle = \frac{n}{2}k_{B}T$$
- this is the **equipartition theorem**

- for a system in contact with a reservoir at a temperature, $T$, each independent quadratic energy mode contributes $\frac{1}{2}k_{B}T$ to the average energy
- the internal energy $(U)$ will be associated with the average energy $(\langle{E}\rangle)$
- so here, 
$$C_{V} = \left(\frac{\partial U}{\partial T}\right)_{V}= \frac{n}{2} k_{B}$$
