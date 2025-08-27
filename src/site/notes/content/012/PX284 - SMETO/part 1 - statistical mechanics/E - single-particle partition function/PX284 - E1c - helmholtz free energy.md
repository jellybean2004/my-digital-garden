---
{"dg-publish":true,"permalink":"/content/012/px-284-smeto/part-1-statistical-mechanics/e-single-particle-partition-function/px-284-e1c-helmholtz-free-energy/","noteIcon":"1","created":"2025-08-27T13:15:25.027+01:00","updated":"2024-12-23T22:16:49.000+00:00"}
---

- the hemholtz free energy is given by:
$$\boxed{F = U - TS}$$
- from [[content/012/PX284 - SMETO/part 1 - statistical mechanics/E - single-particle partition function/PX284 - E1b - entropy\|PX284 - E1b - entropy]]:
$$S = k_{B}(\beta U + \ln  Z)$$
- in terms of $Z_{i}:$ 
$$F = U - k_{B}T (\beta U + \ln Z)$$
$$\boxed{\therefore F = - k_{B}T\ln Z}$$
- conversely, the partition function:
$$Z = \exp(-\beta F)$$
### aside on thermodyanamics
- but $dU = T\,dS - p\,dV$
$$dF = (T\,dS - p\,dV) - T\,dS - S\,dT = -S\,d - p\,dV$$
$$\begin{align*}
	\left(\frac{\partial F}{\partial T}\right)_{V} &=  -S \\
	\left(\frac{\partial F}{\partial V}\right)_{T } &= -p
\end{align*}$$
