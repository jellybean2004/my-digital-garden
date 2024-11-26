---
{"dg-publish":true,"permalink":"/content/011/px-154-physics-foundations/px-154-c-thermal-physics-2/px-154-c7-maxwell-boltzmann-distribution/","created":"2024-11-25T10:50:32.000+00:00","updated":"2024-11-26T23:16:04.489+00:00"}
---

## molecular speeds and energy
 - the molecules in a gas  have different speeds, and we define a distribution function [YF eqn 18.32] 
 $$f(v) = 4 \pi \left(\frac{m}{2\pi k_{B}T}\right)^{\frac{3}{2}}v^2\exp{\left(\frac{-mv^{2}}{2k_{B}T}\right)}$$
 - for $N_2$ at three temperatures:
 ![Pasted image 20231025082058.png](/img/user/pics/Pasted%20image%2020231025082058.png)
 - as $T$ increases:
	 - peak of the distribution moves to higher speeds
	 - the distribution also becomes broader
	 - some slow molecules at high $T$, conversely some fast molecules at a low $T$
- if we have $N$ molecules, the number whose speeds between $v$ and $v+dv$ is: $dN=Nf(v)dv$    [YF p627 ] 
 ![Pasted image 20231024143307.png](/img/user/pics/Pasted%20image%2020231024143307.png)

- $v_{prob}$ is the most probable speed $=\sqrt{\frac{2}{m}k_{B}T}$
- $v_{avg}$ is the average speed = $=\sqrt{\frac{8}{\pi m}k_{B}T}$
- $v_{rms}=\sqrt{\bar{v}^2} = \sqrt{\frac{3}{m}k_{B}T}$  
	- fits with our [[content/011/PX154 - physics foundations/PX154 - C - thermal physics 2/PX154 - C6 - kinetic-molecular model of the ideal gas\|kinetic model for the ideal gas]] and its prediction for $\bar{v}^2$
	- $v_{rms}$ at $STP$ for $N_{2} = 484 ms^-1$
- we can find the energy distribution too: 
- $dN = Nf(v)dv$ using $E=\frac{1}{2}mv^{2} \implies dE=mv dv$, we get: $dN=Nf(E)dE$ 
$$f(E)=\frac{2}{\sqrt{\pi}}\left(\frac{1}{k_{B}T}\right)^{\frac{3}{2}}E^{\frac{1}{2}}\exp{\left(- \frac{E}{k_{B}T}\right)}$$
 ![Pasted image 20231024143328.png](/img/user/pics/Pasted%20image%2020231024143328.png)
	- $peak: E \approx k_{B}T$
- $k_BT$ gives the energy associated with a given temperature
	- at $RTP (T=290K), k_BT=4\times 10^{-21}J\approx25meV$
