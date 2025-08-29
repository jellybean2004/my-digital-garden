---
{"dg-publish":true,"permalink":"/content/012/px-282-stars-and-solar-system/term-2-solar-system/k-giant-planets/px-282-k2a-interiors-of-gas-giants/","noteIcon":"1","created":"2025-08-27T13:15:23.051+01:00","updated":"2025-05-28T18:20:40.000+01:00"}
---

- the radius vs mass can be calculated for a given composition by assuming hydrostatic equilibrium
- balancing gravity with pressure gradient:
$$\frac{dP}{dr} = - \frac{GM_{r}\rho(r)}{r^{2}}$$
	where, $M_r$ is the mass enclosed within radius, r
- to solve for $\rho(r)$, $P(\rho)$ is needed, so **the equation of state** is needed
- this can be very complex and difficult to measure at high pressures
- but for H and He, it can be assumed that:
$$P \simeq K \rho^{2}$$
	where, $K$ is a constant, empirically obtained to be ${} 2.7\times10^5$ N m$^4$ kg$^{-2}$

![PX282 - K2 - radius calculation.png|500](/img/user/pics/PX282%20-%20K2%20-%20radius%20calculation.png)
*image: Stevenson 1982, AREPS 10, 257*

$$\begin{gather}
\frac{dP}{dr} = 2K\rho \frac{d\rho}{dr} = - \frac{GM_{r}\rho}{r^{2}} \\
\implies r^{2} \frac{d\rho}{dr} = - \frac{GM_{r}}{2K} 
\end{gather}$$

- using the mass conservation equation, for a small shell of radius $dr:$
$$dM_{r} = 4\pi r^{2} \rho(r)\, dr$$

$$\begin{gather}
\frac{d^{2}\rho}{dr^{2}}+ \frac{2}{r} \frac{d\rho}{dr} + \frac{2\pi G}{K}\rho = 0 \\
\implies \rho(r) = \rho_{C}  \frac{\sin kr}{kr} 
\end{gather}$$
	where, $\rho_{C} =$ central density of the planet, $k = \sqrt{2\pi G/K}$

- to find the radius of a planet, where $\rho(R ) = 0$, which occurs when:
$$\sin\left(\sqrt{\frac{2\pi G}{K}}r\right) = 0 \implies R = \sqrt{\frac{\pi K}{2G}}$$
- for jupiter, it is found that $R = 7.97 \times10^{7}$ m, which is $=1.12\,R_{J}$ (a really good simple approximation)

![PX282 - K2 - radius calculation-1.png|500](/img/user/pics/PX282%20-%20K2%20-%20radius%20calculation-1.png)
*image: ESO 2002*

- for central density, $\rho_C$, integrating the mass conservation equation:
$$M = \int_{0}^{R} 4\pi r^{2} \rho(r) \, dr = \frac{4\pi \rho_{c}}{k} \int_{0}^{R} r\sin kr\, dr$$
- integrating by parts, and $kR = \pi:$
$$\rho_{C} = \frac{\pi M}{4R^{3}}$$

- for jupiter, $\rho_{C} \simeq 4400$ kg m$^{-3}$
- H/He gas with density similar to rock

- from the equation of state, the central pressure: $P_{C} = K\rho_{C}^{2} = 5\times10^{12}\,\text{Pa} = 5\times10^{7}\,\text{bar}$
- the real phase diagram of H implies a metallic liquid at this pressure
- the electrons are no longer localised to individual atoms, and it conducts electricity - metallic hydrogen
- expect a rocky icy core, then a layer of metallic hydrogen
- higher up in the envelope, H transitions to molecular fluid

- saturn should have the same layers
- but due to lower pressure, the metallic layer is smaller
- possible 'rain out' of He, as it forms droplets due to no longer being soluble in H, which drives ongoing differentiation and heating

![PX282 - K2 - interiors.png|500](/img/user/pics/PX282%20-%20K2%20-%20interiors.png)
*image: Carroll & Ostile, An Introduction to Modern Astrophysics (2007)*

- both of them rotate rapidly ($<0.5$ day, which makes them ***oblate***
- this breaks their spherical symmetries
- so, the gravitational potential probes the interior structure
- eg: samples with juno mission are used for the measurement of $\rho(r)$, and also north-south asymmetries
- the banding pattern extends into deep interior, which implies a ***global convection***

![PX282 - K2 - interiors-1.png|500](/img/user/pics/PX282%20-%20K2%20-%20interiors-1.png)
*image: IESS, et al 2018*

- convection, rotation and conducting (metallic) interior forms a magnetic dynamo
- therefore, jupiter has a strong magnetic field
- the magnetic moment of jupiter $\sim 20000\times$ that of earth
- the magnetic moment of saturn $\sim 600\times$ that of earth, due to less metallic H

- the strong magnetic fields lead to aurorae in poles, as well as radio emissions via both cyclotron and synchrotron emissions by low and high energy electrons orbiting the magnetic field lines

![PX282 - K2 - interiors-3.png|500](/img/user/pics/PX282%20-%20K2%20-%20interiors-3.png)
![PX282 - K2 - interiors-2.png|500](/img/user/pics/PX282%20-%20K2%20-%20interiors-2.png)
*image: de Pater, et al 1997*

- the combination of strong magnetic moment and lower solar wind flux at $5$ au leads to a very large ***magnetosphere***
- the extent can be estimated by equating magnetic energy density $(u_{B})$ with the kinetic energy density of solar winds $(u_{w}):$
$$\begin{gather}
u_{B }= \frac{B^{2}}{2\mu_{0}}\\
u_{w} = \frac{1}{2} \rho_{w} v_{w}^{2} \\
\end{gather}$$
- for a magnetic dipole:
$$B(r) = \frac{\mu_{0}}{2\pi} \frac{\mu}{r^{3}}$$
	where, $\mu$ is the magnetic dipole moment
$$\begin{gather}
\frac{\mu_{0}\mu^{2}}{8\pi^{2}r^{6}} = \frac{1}{2} \rho_{w}v_{w}^{2} \\
R_{m} = \left( \frac{\mu_{0}}{\rho_{w}}\right)^{1/6} \left(\frac{\mu}{2\pi v_{w}}\right)^{1/3}
\end{gather}$$
	where, $R_m$ is the radius of the magnetosphere

- this can easily be scaled between planets:
$$\begin{gather}
u_{B} \propto \left(\frac{\mu}{r^{3}}\right)^{2} \\
u_{w} \propto \frac{1}{a^{2}} \\
\frac{\mu}{R_{m}^{3}}\propto \frac{1}{a} \implies R_{m} \propto (\mu a)^{1/3}
\end{gather}$$
	where, $a$ is the orbital separation of the planet

- the magnetic dipole moments: $\mu_{J}/\mu_{E} \simeq 20000$, and the orbital separations: $a_{J}/a_{E} = 5.2 \implies R_{m,J} \simeq 50 R_{m,E}$
- $R_{m,E} \simeq 10\, R_{E} \implies R_{m,J} \simeq 500\,R_{E} \simeq 50\,R_{J }\simeq 5\,R_{\odot}$
- so, jupiter's magnetosphere is the largest object in the solar system

