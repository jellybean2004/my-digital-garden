---
{"dg-publish":true,"permalink":"/content/012/px-284-smeto/part-1-statistical-mechanics/i-chemical-potential/px-284-i3-grand-canonical-ensemble/","noteIcon":"1","created":"2025-01-16T15:30:50.775+00:00","updated":"2025-01-16T15:50:03.862+00:00"}
---

[[content/012/PX284 - SMETO/part 1 - statistical mechanics/B - introduction/PX284 - B4 - ensembles\|PX284 - B4 - ensembles]]
## microcanonical ensemble
- isolated, so fixed energy
$$\begin{gather}
P_{i} = \frac{1}{\Omega} \\\\
S = k_{B}\ln\Omega \\ \\
\Omega = \exp(\beta T S)
\end{gather}$$
## canonical ensemble
- exchanges energy with a reservoir, so fixes $T$
$$\begin{gather}
P_{i} = \frac{\exp(-\beta E_{i})}{Z} \\\\
F = - k_{B}T \ln Z \\\\
Z = \exp(-\beta F)
\end{gather}$$
## grand canonical ensemble
- exchanges energy and particles with a reservoir, so fixes $T$ and $\mu$

- considering a system with an energy state, $E_{i}$, and particle state, $N_{i}$, connected with a very large reservoir with an energy, $U-E_{i}$, and $N-N_{i}$ particles
- assuming $U\gg E_{i}$ and $N \gg N_{i}$, the entropy of the reservoir is given by : 
$$\begin{align*}
S(U-E_{i}, N-N_{i}) &\approx S(U,N) - E_{i}\left(\frac{\partial S}{\partial U}\right)_{N,U} - N_{i}\left(\frac{\partial S}{\partial N}\right)_{N,U} \\
&= S(U,N) - \frac{1}{T }(E_{i} - \mu N_{i})
\end{align*}$$
- as for seen the canonical ensemble:
$$P_{i}(E_{i},N_{i}) \propto \Omega(U-E_{i}, N-N_{i})$$
	where, $\Omega$ is the number of microstates of the bath
- but: $S = k_{B}\ln\Omega \implies \Omega = \exp(\beta TS)$
$$P_{i} \propto \exp(\beta TS)$$
$$\implies P_{i} \propto \exp(-\beta(E_{i}  - \mu N_{i}))$$
- after normalizing:
$$P_{i} = \exp\frac{-\beta(E_{i}  - \mu N_{i})}{\mathscr{Z}}$$
	where, $\mathscr Z = \sum\limits_{i} \exp(-\beta (E_{i}- \mu N_{i}))$ 
- this is the **gibbs distribution**, and $\mathscr Z$ is the **grand partition function**

- **note:** if $\mu = 0: P_{i} = \exp(-\beta E_{i})/Z$, ie. the boltzmann distribution

- a **grand potential** can also be defined:
$$\Phi_{G} = - k_{B}T \ln\mathscr Z$$
- such that:
$$\mathscr Z = \exp(-\beta\Phi_{G})$$
