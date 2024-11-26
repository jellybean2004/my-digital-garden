---
dg-publish: true
---

- suppose, $E(x) = \alpha x^{2}$, where $\alpha$ is a constant, in the **classical limit**, and $x \in [-\infty, + \infty]$
- in this case, the boltzmann distribution is written as: 
$$P(x) =  \frac{e^{-\beta \alpha x^{2}}}{\int_{-\infty}^{+\infty} e^{-\beta \alpha x^{2}}\,dx}$$
- the average energy: 
$$\langle{E}\rangle = \int_{-\infty}^{+\infty} E(x) P(x) \,dx = \frac{\int_{-\infty}^{+\infty}\alpha x^{2} e^{-\beta \alpha x^{2}}\,dx}{{\int_{-\infty}^{+\infty} e^{-\beta \alpha x^{2}}\,dx}} = \frac{1}{2\beta} = \frac{1}{2}k_{B}T$$
- in general, if the system has $n$ independent quadratic modes or degrees of freedom, ie: $E= \alpha_{1}x_{1}^{2} + \alpha_{2}x_{2}^{2} \dots + \alpha_{n}x_{n}^{2}$, then, $\langle{E}\rangle = \frac{n}{2}k_{B}T$
- this is the **equipartition theorem**
- for a system in contact with a reservoir at a temperature, $T$, each independent quadratic energy mode contributes $\frac{1}{2}k_{B}T$ to the average energy
- the internal energy $(U)$ will be associated with the average energy $(\langle{E}\rangle)$
- so here, 
$$C_{V} = \left(\frac{\partial U}{\partial T}\right)_{V}= \frac{n}{2} k_{B}$$
