---
dg-publish: true
---
- considering a system with an energy, $E_{i}$, connected with an extremely large heat bath (reservoir) such that, $E_{bath} = E - E_{i}$, $\Omega_{bath}(E-E{i})$, and $T$
- for the system, temperature $T$, number of particles $N$, and volume $V$ are fixed
- assuming that the probability of the system in a particular state, $E_{i}$, is proportional to the number of microstates available to the bath in the state: 
$$P(E_{i}) \propto \Omega(E-E_{i})$$
- expanding ${} \ln\Omega(E-E_{i}) {}$ around $E_{i}=0:$ 
$$\ln\Omega(E-E_{i}) = \ln\Omega(E) - \frac{d}{dE }\bigg[\ln\Omega(E)\bigg] \, E_{i}+ \dots \approx \ln\Omega(E) - \frac{E_{i}}{k_{B}T}$$
	where, $\frac{d\ln\Omega}{dE} = \frac{1}{k_{B}T}$
- the additional terms are not relevant as $E>>>E_{i}$
$$\therefore \Omega(E-E_{i}) = \Omega(E) \exp\left(-\frac{{E_{i}}}{k_{B}T}\right)$$
- therefore, the probability: 
$$P(E_{i}) \propto \exp\left(- \frac{E_{i}}{k_{B}T}\right)$$
- for normalization: 
$$\sum\limits_{i} P(E_{i}) = \frac{1}{Z}\sum\limits_{i} {e^{-\beta E_{i}}} = 1$$
- the boltzmann distribution: 
$$\boxed{P(E_{i}) = \frac{e^{-\beta E_{i}}}{Z}}$$
	where, $Z$ is the **partition function** such that:  
$$\boxed{ Z = \sum\limits_{i}e^{-\beta E_{i}}}$$
## example: two state system
- the expected energy: 
$$\begin{align*}
	\langle{E}\rangle &= \sum\limits_{i} E_{i}P_{i} \\
	&= 0 \times P(0) + E \times P(E) \\
	&= E \times \frac{e^{-\beta E}}{Z}
\end{align*}$$
	where, $Z = e^{-\beta\cdot0} + e^{-\beta E}$
$$\therefore \langle{E}\rangle = \frac{Ee^{-\beta E}}{1+e^{-\beta E}} = \frac{E}{e^{\beta E}+1}$$
