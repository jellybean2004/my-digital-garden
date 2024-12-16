---
{"dg-publish":true,"permalink":"/content/011/px-154-physics-foundations/px-154-g-mechanical-waves/px-154-g5-waves-in-bulk-gases-sound-waves/","noteIcon":"1","created":"2024-11-25T10:50:32.000+00:00","updated":"2024-11-26T19:52:28.580+00:00"}
---

## speed of sound
- we have longitudinal waves
- start with our usual plot of displacement, $u(x,t) = A\cos{(kx-\omega t)}$
![Pasted image 20231127183306.png](/img/user/pics/Pasted%20image%2020231127183306.png)

- consider a loud speaker
![Pasted image 20231127183336.png](/img/user/pics/Pasted%20image%2020231127183336.png)

- remember [[content/011/PX154 - physics foundations/PX154 - C - thermal physics 2/PX154 - C1 - ideal gas equation of state\|ideal gas law]]: 
$$pV = nRT \implies p = \rho RT$$
- oscillations of the speaker cone produce density oscillations and pressure gradients that provide the restoring force that leads to *SHM* 
- we find that the pressure is described by: 
$$p = AkB\sin(kx-\omega t)$$
		where, $B=$ bulk modulus of air [YF eqn 16.4]
- we will obtain the speed of sound: 
$$v = \sqrt{\frac{B}{\rho}}$$
	- $v_{air} = 344 ms^{-1}$
## speed of sound in a ideal gas
[YF 16.2]
- for sound waves in an ideal gas, the propagation is fast enough that there is no heat flow. thus, we can consider it to be an *adiabatic process*
- the *bulk modulus* is given by: 
$$B = -V  \frac{\partial p}{\partial V}$$
- for an [[content/011/PX154 - physics foundations/PX154 - D - the first law of thermodynamic/PX154 - D5 - summary of processes\|adiabatic process]]: 
$$pV^{\gamma} = constant = k$$
	where, $\gamma = \frac{c_{P}}{c_{V}}$
$$\begin{align*}
	\frac{\partial p}{\partial V} &= \frac{\partial}{\partial V}( kV^{-\gamma}) \\
	&= -\gamma\,k\,V^{-\gamma-1} \\
	&= -\frac{\gamma}{V} k \,V^{-\gamma} \\
	&= -\frac{\gamma}{V}p
\end{align*}$$
$$\therefore B = \gamma\,p$$
- for the wave speed: 
$$v = \sqrt{\frac{B}{\rho}} = \sqrt{\frac{\gamma \,p}{\rho}}$$
- to make this more usable, $\rho= \frac{m}{V} = \frac{NM}{V}$
- then, 
$$v = \sqrt{\frac{\gamma pV}{NM}}$$
- using $pV = Nk_{B}T$: 
$$v_{ideal \; gas} = \sqrt{\gamma \frac{k_{B}T}{M}}$$
	- oxygen at $300K: v = 340 ms^{-1}$ ; $\gamma = \frac{7}{5}$
	- helium at $300K: v = 1370 ms^{-1}$ ; $\gamma = \frac{5}{3}$

- we can compare with [[content/011/PX154 - physics foundations/PX154 - C - thermal physics 2/PX154 - C7 - maxwell-boltzmann distribution\|boltzmann distribution]]: 
$$v_{rms} = \sqrt{\frac{3k_{B}T}{M}}$$
- hence, $v = v_{rms} \sqrt{\frac{\gamma}{3}}$
	- oxygen at $300K: v_{rms} = 464 ms^{-1}$ 
	- helium at $300K: v_{rms} = 1370 ms^{-1}$ 