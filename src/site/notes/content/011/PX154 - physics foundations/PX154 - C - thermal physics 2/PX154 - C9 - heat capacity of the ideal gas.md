---
{"dg-publish":true,"permalink":"/content/011/px-154-physics-foundations/px-154-c-thermal-physics-2/px-154-c9-heat-capacity-of-the-ideal-gas/","noteIcon":"1","created":"2024-11-25T10:50:32.000+00:00","updated":"2024-12-23T10:15:20.457+00:00"}
---

[YF 18.6]
## relating heat capacity
- need to relate the *[[content/011/PX154 - physics foundations/PX154 - B - thermal physics/PX154 - B3 - heat capacity\|heat capacity]]* of our gas to its motion (the motion of its molecules)
- two definitions to consider:
	- ${} C_v=$ heat capacity at constant volume
	- ${} C_p=$ heat capacity at constant pressure
## heat capacity at constant volume
- for now, consider $C_{V}$: 
$$C_{V}=\frac{1}{n} \frac{dQ}{dT}$$
- if some heat, $Q$, is added, the kinetic energy of the gas increases: 
$$C_{V}=\frac{1}{n} \frac{dK_{tr}}{dT}=\frac{3}{2}R=12.47 Jmol^{-1}K^{-1}$$
- from *[[content/011/PX154 - physics foundations/PX154 - C - thermal physics 2/PX154 - C6 - kinetic-molecular model of the ideal gas#^8082ac\|here]]*: 
$$\bar{E}_{K}=\frac{3}{2}k_{B}T$$
- for $N$ molecules: 
$$\bar{E}_{K}=\frac{3}{2}Nk_{B}T$$
- and for $n$ moles: 
$$\bar{E}_{K}=\frac{3}{2}nk_{B}T$$
- ${} K_{tr}$ used instead of $\bar E_K$ - kinetic energy owing to translation 
$$C_{V} = \frac{1}{n} \frac{dK_{tr}}{dT}= \frac{3}{2}R$$
- at $STP$, measured values:

| gas   | $c_v$ |
| ----- | ----- |
| He    | 12.5  |
| Ar    | 12.5  |
| Ne    | 12.7  |
| Kr    | 12.3  |
| $N_2$ | 20.8  |
| $H_2$ | 20.4  |
| $O_2$ | 21.1  |

- key observations:
	- noble gases - monatomic $:C_{V}\approx\frac{3}{2}R$
	- other - diatomic $:C_{V}\approx\frac{5}{2}R$
- reason: 
	- *monatomic* particles *only translation*
	- for *diatomic*, there may be *rotation and vibration*
## equipartition of energy
- each form of motion is a "*degree of freedom*" and contributes to $\frac{1}{2}k_{B}T$ of energy per atom
### translation
![Pasted image 20231101093530.png](/img/user/pics/Pasted%20image%2020231101093530.png) [YF 18.18]
- our translation is in 3D, and translation in each of these is a degree of freedom contributing $\frac{1}{2} k_{B}T$
- translation in 3D contributes to a total energy $\frac{3}{2}k_{B}T$ per atom
- for $n$ moles, $\frac{3}{2}nRT$ : 
$$C_{V}= \frac{1}{n}\frac{dQ}{dT}=\frac{3}{2}R$$
### rotation
- neglect this for monatomic gases
- diatomic gases: 
	- molecule can rotate, but not about all 3 axes: 
	![Pasted image 20231101093609.png](/img/user/pics/Pasted%20image%2020231101093609.png) [YF 18.18]
	- it is found that rotation can only be observed about $y$ and $z$ axes
	- one of these axes is along the molecule's axis, effectively the same as the monatomic case, so there is no contribution
	- this gives 2 degrees of freedom
		- $2\times \frac{1}{2}k_{B}T = k_{B}T$ per atom $=RT$ per mole
	- for $C_{V}$, an extra $R$ is obtained 
	$$\therefore C_{V} \; for \; translation \; and \; rotation = \frac{5}{2}R$$
### vibration
- doesn't exist for monatomic molecules
- molecules can vibrate via stretching/contracting, or sometimes by bending of the interatomic bonds
- the bond can be modelled as a spring and treat it as a *harmonic oscillator*, *[[content/011/PX155 - classical mechanics and special relativity/classical mechanics/PX155 - D - simple harmonic motion/PX155 - D1 & D2 - oscillations & mass on a spring\|SHM]]* 
![Pasted image 20231101093623.png](/img/user/pics/Pasted%20image%2020231101093623.png) [YF 18.18]
- $KE$ and $PE$ from the vibration have to be included. each adds one degree of freedom
	- total $k_BT$ 
	- contribution to $C_{V}$ is $R \; per \; mole$ 
- at room temperature, vibration doesn't contribute to the heat capacity
- vibration is quantized
	- requires a quantum mechanical model [[content/012/PX262 - quantum mechanics/PX262A - 0 - quantum mechanics\|PX262 - 0 - quantum mechanics and its applications]]
	- eg: for $N_2$, minimum energy to be absorbed to increase vibration is $0.3 eV$
	- using $k_BT$, this corresponds to a temperature of $3000K$
- ![Pasted image 20231101093653.png](/img/user/pics/Pasted%20image%2020231101093653.png) [YF fig 18.19] 

- comment:
	- for larger molecules, vibrations are more complicated with different modes available
	- ![Pasted image 20231025085547.png](/img/user/pics/Pasted%20image%2020231025085547.png)
	- $CO_2$ at $STP: C_{V} = 28.5 J mol^{-1}K^{-1}$ 