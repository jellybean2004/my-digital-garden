---
{"dg-publish":true,"permalink":"/content/012/px-282-a-stars/e-stellar-evolution/px-282-e1a-star-formation/","created":"2024-11-25T10:50:32.000+00:00","updated":"2024-12-06T17:12:45.682+00:00"}
---

![Pasted image 20241121102048.png|500](/img/user/pics/Pasted%20image%2020241121102048.png)
*image magnus vilhelm*

- stellar evolution begins with star formation, which happens from the gravitational collapse of clouds of material
- from [[content/012/PX282A - stars/D - stellar structure and interiors/PX282 - D4 - energy in stars#^b7947e\|the virial theorem]]: 
$$2U + \Omega = 0$$
- if $2U > |\Omega|$, the cloud expands, and if $2U < |\Omega|$, the cloud collapses
$$\Omega_{tot} = - \int_{0}^{R} \frac{GM_{r}(r)}{r} \rho \, 4\pi r^{3}\,dr$$
- for a constant $\rho$, 
$$M_{r}= M \left(\frac{r}{R}\right)^{3}$$
	- where, $M_{r}$ is the mass within the radius, $r$, and $M$ us the total mass if the cloud with radius, $R$, and density: 
	$$\rho = \frac{M}{\frac{4}{3}\pi R^{3}}$$
$$\Omega_{tot} = - \frac{4\pi GM\rho}{R^{3}} \, \int_{0}^{R}  r^{4}\,dr \, $$
$$\Omega = - \frac{3}{5} \frac{GM^{2}}{R}$$
- since $U = \frac{3}{2}k_{B}T$ per particle:
$$U_{tot} = \frac{3}{2}Nk_{B}T$$
	- where, $N=\frac{M}{\mu m_{H}}$ is the number of particles
- for collapse: 
$$3Nk_{B}T  < \frac{3}{5} \frac{GM^{2}}{R} \implies M > \frac{5Rk_{B}T}{\mu m_{H}G}$$
- removing $R:$ 
$$M_{J} > \left(\frac{5k_{B}T}{\mu m_{H}G}\right)^{\frac{3}{2}} \left(\frac{3}{4\pi\rho}\right)^\frac{1}{2}$$
	- where, $M_{J}$ is called the **jeans mass**

- a typical molecular cloud has $T=20\,K$, $R\approx 2\,pc$, $\mu=2$, and therefore, $M> \sim100\,M_{\odot}$