---
{"dg-publish":true,"permalink":"/content/012/px-284-smeto/part-1-statistical-mechanics/c-entropy-and-temperature/px-284-c3-boltzmann-distribution/","noteIcon":"1","created":"2025-08-27T13:14:15.566+01:00","updated":"2024-12-23T21:22:58.000+00:00"}
---

- considering a system with an energy, $E_{i}$
- it is connected to an extremely large heat bath (reservoir) with: $E_{bath} = E - E_{i}$ , $\Omega_{bath}(E-E{i})$ , and $T$

- for the system, temperature $T$, number of particles $N$, and volume $V$ are fixed

- assuming that the probability of the system being in a particular state, $E_{i}$, is proportional to the number of microstates available to the bath in the state: 
$$P(E_{i}) \propto \Omega(E-E_{i})$$
- [[content/011/PX153 - mathematics for physicists/term 1/PX153 - F - series/PX153 - F1 - taylor series\|taylor series]] expansion of $\ln\Omega(E-E_{i})$ around $E_{i}=0$ 
$$\ln\Omega(E-E_{i}) = \ln\Omega(E) - \frac{d}{dE }\bigg[\ln\Omega(E)\bigg] \, E_{i}+ \dots \approx \ln\Omega(E) - \frac{E_{i}}{k_{B}T}$$
	where, $\frac{d\ln\Omega}{dE} = \frac{1}{k_{B}T}$ from [[content/012/PX284 - SMETO/part 1 - statistical mechanics/C - entropy and temperature/PX284 - C2 - temperature\|PX284 - C2 - temperature]]

- the additional terms are not relevant as $E\gg E_{i}$
$$\therefore \Omega(E-E_{i}) \approx \Omega(E) \exp\left(-\frac{{E_{i}}}{k_{B}T}\right)$$
- therefore, the probability: 
$$P(E_{i}) \propto \exp\left(- \frac{E_{i}}{k_{B}T}\right)$$
- for normalization: 
$$\sum\limits_{i} P(E_{i}) = \frac{1}{Z}\sum\limits_{i} {e^{-\beta E_{i}}} = 1$$
- the **boltzmann distribution**: 
$$\boxed{P(E_{i}) = \frac{e^{-\beta E_{i}}}{Z}}$$
- $Z$ is the **partition function** such that:  
$$\boxed{ Z = \sum\limits_{i}e^{-\beta E_{i}}}$$
## example
- a two state system with energies: $0$ or $E$
- the expected energy: 
$$\begin{align*}
	\langle{E}\rangle &= \sum\limits_{i} E_{i}P_{i} \\
	&= 0 \times P(0) + E \times P(E) \\
	&= E \times \frac{e^{-\beta E}}{Z}
\end{align*}$$
	where, $Z = e^{-\beta\cdot0} + e^{-\beta E}$
$$\therefore \langle{E}\rangle = \frac{Ee^{-\beta E}}{1+e^{-\beta E}} = \frac{E}{e^{\beta E}+1}$$
