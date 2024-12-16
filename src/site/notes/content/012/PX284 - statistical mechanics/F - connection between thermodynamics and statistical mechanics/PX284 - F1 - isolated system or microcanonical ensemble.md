---
{"dg-publish":true,"permalink":"/content/012/px-284-statistical-mechanics/f-connection-between-thermodynamics-and-statistical-mechanics/px-284-f1-isolated-system-or-microcanonical-ensemble/","noteIcon":"1","created":"2024-11-29T18:43:20.801+00:00","updated":"2024-12-05T15:14:12.534+00:00"}
---

- in statistical mechanics:
$$\begin{gather*}
	S = - k_{B} \sum\limits_{i} P_{i}\ln P_{i} \\ 
	U = \sum\limits_{i} E_{i}P_{i} 
\end{gather*}$$
## thermodynamics
- [[content/011/PX154 - physics foundations/PX154 - E - the second law of thermodynamics/PX154 - E3 - the second law of thermodynamics\|the second law of thermodynamics]] states that, for all processes in an isolated system:
$$dS \geq 0$$
	where, the equality is for **reversible changes**
- a process is **reversible** if it:
	- is performed **quasi-statically** (slow chances via equilibrium states)
	- involves no dissipation (eg.: turbulence, electrical resistance)

- for a general process, $S$ increases until $dS = 0$ at equilibrium, ie. $S$ is maximized
## statistical mechanics
- in statistical mechanics: $S$ for an isolated two-state system:
$$S = -k_{B} \sum\limits_{i} P_{i}\ln P_{i} = - k_{B} [P_{1} \ln P_{1} + P_{2}\ln P_{2}]$$
$$\frac{dS}{dP_{1}}= - k_{B} \left[ \ln P_{1} + 1 + \frac{dP_{2}}{dP_{1}}(\ln P_{1} +1 ) \right] = 0$$
	at maximum (equilibrium)
- but, $P_{1} + P_{2} = 1$
- so, $\frac{dP_{2}}{dP_{1}}=1$
- at maximum $S: \ln P_{1} + 1 - \ln P_{2} -1 =0 \implies ln P_{1} = \ln P_{2} \implies P_{1} = P_{2}$
- this shows that the microstates are equiprobable
- it can be shown that this is true for an $N$ state system
- therefore, maximizing $S \equiv$ equiprobable microstates
- this is he definition of equilibrium in microcanonical ensemble
