---
{"dg-publish":true,"permalink":"/content/011/px-155-classical-mechanics-and-special-reltivity/classical-mechanics/px-155-c-work-and-energy/px-155-c4-using-energy-conservation/","created":"2024-10-01T18:27:09.530+01:00","updated":"2024-11-26T19:55:26.822+00:00"}
---

- if no mention of time in a problem and only conservative forces act, try using energy conservation
- eg: object released from rest at a height $h=3000km$ above the earth
	- ignore air resistance
	- to find: speed at which it hits the ground
		- $E=T+U$
		- when released:
			- $U=- \frac{GM_{E}m}{R_{E}+h}$
			- $T=0$
		- when it hits the ground:
			- $U=- \frac{GM_{E}m}{R_{E}}$
			- $T= \frac{1}{2}mv^2$
		- equating
$$- \frac{GM_{E}m}{R_{E}+h}+0=-\frac{GM_{E}m}{R_{E}}+ \frac{1}{2}mv^2$$
		
$$v^2=2GM_{E}[\frac{h}{R_E(R_E+h)}]$$
		- plugging in the numbers: $v=6.3kms^{-1}$
			- if $U=mgh$, $v=7.7kms^{-1}$
- eg: escape velocity : what speed is needed to escape the gravitational pull of a body of mass $M$ and radius $R$?
	- on the surface:
		- $T=\frac{1}{2}mv_E^2$
		- $U=- \frac{GMm}{R}$
	- at $r=\infty$:
		- $T=0$
		- $U=0$
	- equating:
$$\frac{1}{2}mv_{E}^{2}- \frac{GMm}{R}=0$$
	
$$v_{E}=\sqrt{2 \frac{GM}{R}}$$
	- plugging in numbers: 
		- for earth: $v_E=11.2kms^{-1}$
		- for sun: $v_E=618kms^{-1}$
