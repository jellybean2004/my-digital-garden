---
{"dg-publish":true,"permalink":"/content/011/px-154-physics-foundations/px-154-e-the-second-law-of-thermodynamics/px-154-e6c-adiabatic-processes/","created":"2024-11-25T10:50:32.000+00:00","updated":"2024-11-26T19:51:18.343+00:00"}
---

### reversible
$$\Delta S = \int_{state\,1}^{state\,2} \frac{dQ}{T}$$
- however, $\Delta Q = 0$ for an adiabatic process, so: 
$$\Delta S = 0$$
- ***isentropic process*: entropy doesn't change**
![Pasted image 20240528203235.png](/img/user/pics/Pasted%20image%2020240528203235.png)
### irreversible
- free expansion of an ideal gas [YF ex 20.8]
![Pasted image 20240121175409.png](/img/user/pics/Pasted%20image%2020240121175409.png)
- process is adiabatic: $Q = 0$
- no work is done by the gas as there is no piston to push: $W=0$ 
- no change in internal energy: $\Delta U = 0 \implies T_{2}= T_{1}$
- does the entropy change?
	- process is irreversible, so, come up with a reversible isothermal process that achieves the same change in state
	- start and end points identical, but, the isothermal process requires: 
$$\begin{align*}
	Q = W &= nRT\ln{\frac{V_{2}}{V_{1}}} \\
	\Delta S &= nR\ln{\frac{V_{2}}{V_{1}}} \\
	&= nR \ln{2}
\end{align*}$$
	- the entropy increases
