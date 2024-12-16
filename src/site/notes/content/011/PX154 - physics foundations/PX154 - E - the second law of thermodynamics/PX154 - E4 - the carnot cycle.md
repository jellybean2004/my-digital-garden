---
{"dg-publish":true,"permalink":"/content/011/px-154-physics-foundations/px-154-e-the-second-law-of-thermodynamics/px-154-e4-the-carnot-cycle/","noteIcon":"1","created":"2024-11-25T10:50:32.000+00:00","updated":"2024-11-26T19:51:10.731+00:00"}
---

## introduction
- introduced by sadi carnot in 1834 as an ideal model of a reversible heat engine cycle
- it's theoretical and it can be shown that it's the most efficient heat engine cycle
- all real engines have an efficiency lower than that of a carnot engine
![Pasted image 20231101100919.png](/img/user/pics/Pasted%20image%2020231101100919.png)
![Pasted image 20231107140821.png](/img/user/pics/Pasted%20image%2020231107140821.png)
- work done = area enclosed by the cycle
- if this is reversed, a heat pump would be created
## work done in the carnot cycle
- $A \to B:$ isothermal expansion at $T_{H}$
	${} W_{A\to B}=nRT_{H}ln\frac{V_{2}}{V_{1}} {}$
	$\Delta U = 0$
	$Q_{A\to B}=W_{A\to B}$
	
- $B\to C:$ adiabatic cooling
	$Q_{B\to C}=0$
	${} W_{B\to C} = -nC_{V}(T_{C}-T_{H}) {}$
	$\Delta U = -W_{B\to C}$
	
- $C \to D:$ isothermal compression at $T_{C}$
	- heat expelled from engine to the cold reservoir
	$W_{C \to D}=nRT_{C}ln\frac{V_{3}}{V_{4}}$
	$\Delta U = 0$
	$Q_{C \to D}= W_{C \to D}$
	
- $D \to A:$ adiabatic compression 
	$Q=0$
	$W_{D \to A}=-nC_{V}(T_{H}-T_{C}) = -W_{B \to C}$
	$\Delta U = -W_{D \to A}$
	
- for one cycle:
	$\Delta U = 0$
	${} W_{total}= nRT_{H}\ln{\frac{V_{2}}{V_{1}}} +nRT_{C}\ln\frac{V_{4}}{V_{3}} {}$
	$Q_{total}= W_{total}$
- can simplify using: $TV^{\gamma-1}=constant$, for adiabatic process
	- for $B \to C:$ 
	$$T_{H}V_{2}^{\gamma-1} = T_{C}V_{3}^{\gamma-1}$$
	- for $D \to A:$ 
	$$\begin{align*}
			T_{H}V_{1}^{\gamma-1} &= T_{C}V_{4}^{\gamma-1} \\\\
			\therefore \frac{V_{2}}{V_{1}} &= \frac{V_{3}}{V_{4}}
		\end{align*}$$
	- so: 
	$$W_{total}=Q_{total}= nR(T_{H}-T_{C})\ln{\frac{V_{2}}{V_{1}}}$$
## efficiency of the carnot cycle
[YF 20.6]
- we have: $\epsilon = \frac{W}{Q_{H}} = 1- \frac{|Q_{C}|}{|Q_{H}|}$
	- $Q_{H}=$ heat absorbed from ${} A \to B {}$
	- $Q_{C}=$ heat expelled from $C \to D$
$$\epsilon = 1 - \frac{|Q_{3\to4}|}{|Q_{1\to2}|}$$
	${} Q_{A \to B}=nRT_{H}ln\frac{V_{2}}{V_{1}} {}$
	$Q_{C \to D}=nRT_{C}ln\frac{V_{4}}{V_{3}}$
- just showed that $\frac{V_{2}}{V_{1}}= \frac{V_{3}}{V_{4}}$: 
$$\therefore \epsilon = 1- \frac{T_{C}}{T_{H}}$$
- eg:
	- $T_{C}=273K$, $T_{H}=373K$, $\epsilon = 0.27\implies 27\%$
	- $T_{C}=300K$, $T_{H}=600K$, $\epsilon = 0.5\implies 50\%$
	- petrol engine $\sim 20.35\%$
	- diesel engine $\sim 50\%$
	- stirling engine $\sim 15-30\%$
	- humans $\sim 25\%$

- *always* use kelvin for temperature
- all reversible engines operating between the same temperatures have the same efficiency
