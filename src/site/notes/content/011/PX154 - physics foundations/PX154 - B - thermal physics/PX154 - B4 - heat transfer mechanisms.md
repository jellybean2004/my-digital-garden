---
{"dg-publish":true,"permalink":"/content/011/px-154-physics-foundations/px-154-b-thermal-physics/px-154-b4-heat-transfer-mechanisms/","created":"2024-11-25T10:50:32.000+00:00","updated":"2024-11-26T19:49:27.572+00:00"}
---

[YF 17.6]
## conduction
- important one for solids, occurs in liquids too
	- no mass transport for solids
- consider heat along a 1D rod ![Pasted image 20231016150931.png](/img/user/pics/Pasted%20image%2020231016150931.png)
	- heat flow/flux:  
	$$\frac{dQ}{dt}=-\kappa A \frac{dT}{dx}$$
		- where,
			- $A=$ cross-sectional area
			- $\frac{dT}{dx}=$ temperature gradient ![Pasted image 20231017090954.png](/img/user/pics/Pasted%20image%2020231017090954.png)
			- $\kappa=$ thermal conductivity
				- for copper/silver, $\kappa=400Wm^{-1}K^{-1}$
				- for glass, $\kappa=0.8Wm^{-1}K^{-1}$
				- for diamond, $\kappa=1800Wm^{-1}K^{-1}$
				- for expanded polystyrene, $\kappa=0.08^{-1}K^{-1}$
			- need the negative sign as heat flows from hot to cold
- heat conduction can be via electrons in an electrical conductor and via vibrations of the atoms
### examples of conduction
- case 1
	![Pasted image 20231017091017.png](/img/user/pics/Pasted%20image%2020231017091017.png)
	- in equilibrium, $\frac{dQ}{dt}$ is the same in both materials, ie: $\frac{dQ_1}{dt}=\frac{dQ_2}{dt}$
		- [YF 17.12 example]
- case 2
	![Pasted image 20231017091031.png](/img/user/pics/Pasted%20image%2020231017091031.png)
	- $\frac{dT}{dx}$ is the same for both rods
		$\therefore$ total $\frac{dQ}{dt}=\frac{dQ_1}{dt}+\frac{dQ_2}{dt}$
- eg:
	![Pasted image 20231017091100.png](/img/user/pics/Pasted%20image%2020231017091100.png)
	$$\frac{dQ_1}{dt}=\frac{dQ_2}{dt}+\frac{dQ_3}{dt}$$
## convection
- heat flow arising from motion of a fluid
## radiation
- a surface at temperature $T$ will radiate at a power $P$ proportional to the surface area $A$ and $T^4$:
$$P= \frac{dQ}{dt}=e\sigma AT^4$$
		$e=$ surface emissivity
		$\sigma=5.67\times 10^{-8}Wm^2K^{-1}$ (stephan boltzmann constant)
	- all bodies emit and absorb radiation
	- we will need a quantum theory to describe it properly - [[content/011/PX156 - quantum phenomena/PX156A - quantum phenomena/PX156 - A - light/PX156 - A2 - blackbody radiation and laws#PX158 - F1 - black body radiation stefan-boltzmann law stefan-boltzmann law for blackbodies\|stefan-boltzmann law for blackbodies]]
