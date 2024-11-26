---
{"dg-publish":true,"permalink":"/content/011/px-155-classical-mechanics-and-special-reltivity/special-relativity/px-155-i-relativistic-momentum-mass-and-energy/px-155-i5-relativistic-kinetic-energy/","created":"2024-10-01T18:27:09.801+01:00","updated":"2024-11-26T19:59:33.293+00:00"}
---

- we have:
$$E_{K} = \int F.dx = \int \frac{dp}{dt} \frac{dx}{dt} .dt= \int v \frac{dp}{dt}.dt$$
- integrating by parts:
$$E_{K} = vp - \int p \frac{dv}{dt} .dt = vp - \int p.dv$$
- integrating from $0$ to $v$: $$E_{K}= [vp]_{0}^{v} - \int_{0}^{v}p.dv$$
$$E_{K}= \frac{m_{0}v^{2}}{(1- \frac{v^{2}}{c^{2}})^\frac{1}{2}} - \int_{0}^{v}\frac{m_{0}v}{(1- \frac{v^{2}}{c^{2}})^\frac{1}{2}}.dv$$
- here,
$$\frac{d}{dv} (1- \frac{v^{2}}{c^{2}})^{\frac{1}{2}} = -2\frac{v}{c^{2}}\frac{1}{2} (1- \frac{v^{2}}{c^{2}})^{-\frac{1}{2}} = -\frac{v}{c^{2}} \frac{1}{(1- \frac{v^{2}}{c^{2}})^\frac{1}{2}}$$
- we have:
$$E_{K}= \frac{m_{0}v^{2}}{(1- \frac{v^{2}}{c^{2}})^{\frac{1}{2
- 
- }}} + m_{0}c^{2} \left[ (1- \frac{v^{2}}{c^{2}})^{\frac{1}{2}}\right]_{0}^{v}$$
$$E_{K} = \frac{m_{0}v^{2}}{(1- \frac{v^{2}}{c^{2}})^{\frac{1}{2}}} + m_{0}c^{2}(1- \frac{v^{2}}{c^{2}})^{\frac{1}{2}} - m_{0}c^{2}$$
$$E_{K}= \gamma m_{0}c^{2}-m_{0}c^{2}$$
$$\therefore E_{K} = (\gamma-1)m_{0}c^{2}$$
## equivalence of mass and energy
- *[[content/011/PX155 - classical mechanics and special reltivity/special relativity/PX155 - I - relativistic momentum mass and energy/PX155 - I2 - relativistic momentum\|here]]*, to particles of rest mass, $m_{0}$, were collided to form a new particle with $M_{0}=2\gamma m_{0}$
- increase in rest mass was:
$$\Delta m_{0} = 2(\gamma-1)m_{0} = \frac{\Delta E_{K}}{c^{2}}$$
	- before collision:
$$E_{K} = 2(\gamma-1)m_{0}c^{2}$$
	- after collision:
$$E_{K}= 0$$
$$\Delta E_{K} = 2(\gamma-1)m_{0}c^{2}= \Delta m_{0}c^{2}$$
- if something already has a rest mass of $m_{0}$, then an amount of energy must have gone into creating it. the *rest mass energy*:
$$E_{0} = m_{0}c^{2}$$
- total energy (kinetic + rest mass): $$E = E_{0} + E_{K} = m_{0}c^{2} + (\gamma-1)m_{0}c^{2} = \gamma m_{0}c^{2}$$
$$\therefore E=mc^{2}$$
- eg: the sun's luminosity, $L = 3.8 \times10^{26}W$. at what rate does it lose mass?
		$E=mc^{2}$
	- so:$$\dot m = \frac{\dot E}{c^{2}} = - \frac{L}{c^{2}} = -4.3 \times10^{9} kg\,s^{-1}$$

- eg: calculate speed of an electron which has $E_{K}= 30 keV$ ($E_{0}$ for electron is $511keV$)
	$$E_{K} = (\gamma -1)m_{0}c^{2} = (\gamma -1)E_{0}$$
	$$\gamma-1 = \frac{E_{K}}{E_{0}} = 1+ \frac{30}{511}$$
	$$v = c \sqrt{1- \frac{1}{\gamma^{2}}} = 0.33c$$
