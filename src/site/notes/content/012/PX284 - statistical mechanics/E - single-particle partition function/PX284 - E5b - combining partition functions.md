---
{"dg-publish":true,"permalink":"/content/012/px-284-statistical-mechanics/e-single-particle-partition-function/px-284-e5b-combining-partition-functions/","noteIcon":"1","created":"2024-11-29T17:53:29.459+00:00","updated":"2024-12-23T22:59:36.591+00:00"}
---

- if the  energy depends on two independent and distinct contributions:
$$E_{i,j} = E_{i} + E_j$$
	where, $E_{i}$ and $E_{j}$ belong to two subsystems, $A$ and $B$, respectively

- the total partition function:
$$\begin{align*}
	Z_{tot} &= \sum\limits_{i} \sum\limits_{j} \exp(-\beta(E_{i}+E_{j})) \\
	&= \sum\limits_{i}\exp(-\beta E_{i}) \sum\limits_{j}\exp(-\beta E_{j}) \\
	&= Z_{a} \times Z_b
\end{align*}$$
- similarly, for more than two contributions:
$$Z_{tot}= Z_{a} \times  Z_{b} \times \dots$$
- for functions that depend on $\ln(Z)$, the contributions add up:
$$\begin{align*} 
	U_{tot} &= U_{a} + U_{b}+U_{c} + \dots \\
	F_{tot} &= F_{a} + F_{b} + F_{c} + \dots
\end{align*}$$
