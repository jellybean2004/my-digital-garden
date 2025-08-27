---
{"dg-publish":true,"permalink":"/content/011/px-157-electricity-and-magnetism/px-157-d-induction/px-157-d3a-inductors/","noteIcon":"1","created":"2025-08-27T13:14:00.362+01:00","updated":"2024-11-26T20:10:48.000+00:00"}
---

## self-inductance
![Pasted image 20240322163707.png](/img/user/pics/Pasted%20image%2020240322163707.png)
- a solenoid with $N$ turns, of length, ${} l$, and magnetic flux, $\phi_{B}$
- if $I_{s}(t) \implies B(t) \implies \phi_{B}(t):$ [[content/011/PX157 - electricity and magnetism/PX157 - D - induction/PX157 - D1a - faraday's law\|faraday's law]]:
$$
\phi_{B}= -N \frac{d\phi_{B}}{dt}= - \frac{d}{dt}(N\phi_{B})
$$
- $N\phi_{B}$ is called the *flux linkage*
	- units: $weber\,(Wb)$
- $\phi_{B} \sim B \sim I_{s} \implies \phi_{B}\sim I_{s}$

- *self-inductance* is defined as:
$$
\boxed{L = \frac{N\phi_{B}}{I}}
$$
	- units: $henry\,(H) = kg\,m^{2}\,C^{-2}$
	- compare with $C=\frac{Q}{V}$, or $\frac{1}{R}=\frac{I}{V}$ 
- for a long solenoid:
$$\begin{align*}
	B &= \mu_{0} \frac{N}{l}I \\
	\phi_{B} &= \mu_{0} \frac{N}{l} AI \\
	L &= \frac{\mu_{0}N^{2}A}{l}
\end{align*}$$
- if a ferromagnetic material is added inside the solenoid, $\mu_{0}\to\mu_{0}\mu_{r}:$
$$
L = \frac{\mu_{r}\mu_{0}N^{2}A}{l}
$$
