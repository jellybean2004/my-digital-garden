---
{"dg-publish":true,"permalink":"/content/012/px-282-a-stars/c-stellar-atmosphere/c10-13-radiative-transfer/px-282-c11-radiation-pressure/","noteIcon":"1","created":"2024-11-25T10:50:32.000+00:00","updated":"2024-12-22T16:19:45.737+00:00"}
---

- photons carry momentum: 
$$E_{\gamma} = pc$$
- hence, they exert a pressure

- examples of radiation pressure in action:
	- protoplanetary pressure
	- kepler's second light (KS) mission 
	- dust tail of comets

- consider a beam of photons, with a momentum, $p_{\gamma}$, hits a surface at an angle, $\theta$ with the $z$-axis, and gets reflected with a momentum, $p_{\gamma}'$
- the change in the $z$-component of the momentum: 
$$\Delta p_{z} = p_{z}' - p_{z} = \frac{E\cos\theta}{c} - \frac{-E\cos\theta}{c} = \frac{2E\cos\theta}{c}$$
- the energy: 
$$E = I\cos\theta\,dt\,dA\,d\Omega$$
- therefore, a small change in momentum can be given by:
$$dp = \frac{2}{c} I\,dt\,dA\, \cos^{2}\theta\,d\Omega$$
- force, $F=\frac{dp}{dt}$, leads to: 
$$P = \frac{dp}{dt\,dA}$$
- the radiation pressure is given by: 
$$P_{rad}= \int_{H} \frac{2}{c}I\cos^{2}\theta \,d\Omega$$
	- where, the integral is over a hemisphere ($H$)

- in a gas, there is no surface to reflect, so the integral will be over the entire sphere ($S$), and the factor of $2$ will be removed: 
$$P_{rad}= \frac{1}{c} \int_{S} I\cos^{2}\theta\,d\Omega = \frac{I}{c}\int_{0}^{2\pi} d\phi \int_{0}^{\pi}d\theta \cos^{2}\theta \sin\theta$$
$$\therefore P_{rad}= \frac{4\pi}{3c} I$$
- since it is integrated over a sphere, the average intensity can be taken:
$$P_{rad} = \frac{4\pi}{3c} \langle{I}\rangle$$
- for a blackbody emitter: 
$$I = \frac{\sigma T^{4}}{\pi}$$
$$\therefore P_{rad,\,bb} = \frac{4\sigma}{3c} T^{4} = \frac{1}{3}aT^{4}$$
	where, $a = \frac{4\sigma}{c} = 7.57\times10^{-16}\,Jm^{-3}K^{-4}$


- for the earth, $T\sim300\,K$, $P_{rad} \sim 2\times10^{-6}\,Nm^{-2} \sim 10^{-11}\,bar$
- for the sun: 
	- $T_{surface}\sim 5800\,K$, $P_{rad} \sim 2.9\times10^{-1}\,Nm^{-2} \sim10^{-6}\,bar$
	- $T_{core} \sim 1.5\times10^{7}\,K$, $P_{rad}\sim 1.3\times10^{13\,Nm^{-2}}\sim 10^{8}\,bar$
