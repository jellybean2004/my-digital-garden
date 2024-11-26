---
dg-publish: true
---

## adiabatic expansion of an ideal gas
![Pasted image 20240225141502.png](/img/user/pics/Pasted%20image%2020240225141502.png)
$$Q=0$$
$$dU = -dW = -pdV$$
$$nC_{V}dT = \frac{-nRT}{V}dV$$
- rearrange: 
$$\frac{dT}{T}= - \frac{R}{C_{V}} \frac{dV}{V}$$
	- note: for $\frac{R}{C_{V}}= \frac{C_{P}-C_{V}}{C_{V}} = \gamma -1$
		$\frac{dT}{T} = - (\gamma - 1) \frac{dV}{V}$
		$\frac{dT}{T} + (\gamma - 1) \frac{dV}{V} = 0$
	- integrate: $\ln(TV^{\gamma-1})=constant$ 
	$$TV^{\gamma-1}=constant$$
	- using *[[content/011/PX154 - physics foundations/PX154 - C - thermal physics 2/PX154 - C1 - ideal gas equation of state\|ideal gas law]]*: 
	$$pV^{\gamma}=constant$$

- compare with the isotherm: 
	- here, $pV=nRT$ with $T$ constant
	- so, for isotherm: $pV=constant$

 ![Pasted image 20231102161930.png](/img/user/pics/Pasted%20image%2020231102161930.png) 
## work done along the adiabat
- we have, $W = -\Delta U$, since $Q=0$
- take $dW=dU$
		$W = - \int nC_{V}dT$  , here, ($C_{V}=\frac{1}{n} \frac{dU}{dT}$)
			$= -n C_{V}(T_{2}-T_{1})$ 
		$$\therefore W = -n C_{V} \Delta T$$
	- can also be written as: 
	$$W= - \frac{1}{\gamma-1}(p_{2}V_{2}-p_{1}V_{1})$$
- note: ![Pasted image 20231102162532.png](/img/user/pics/Pasted%20image%2020231102162532.png)
- whether we go $A\to B$ via adiabat or $A\to C \to B$, $\Delta T$ is the same $\because \Delta U$ is the same
- for $A \to C \to B$:
	- isotherm: $\Delta U = 0$
	- isochore: $\Delta U = n C_{V} \Delta T$
		$\therefore\Delta U_{total}= 0+ nC_{V}\Delta T$
- for adiabat: $W=\Delta U$
	- $\therefore W=-nC_{V}\Delta T$
		- $C_{V}=$ heat capacity at constant volume, even though, V is not constant
