---
{"dg-publish":true,"permalink":"/content/012/px-282-stars-and-solar-system/term-2-solar-system/l-formation-of-solar-system/px-282-l2-core-accretion/","noteIcon":"1","created":"2025-08-27T13:15:28.490+01:00","updated":"2025-03-16T11:27:27.000+00:00"}
---

- firstly, the young sun and the protoplanetary disc is formed by gravitational collapse

- ***sub-micron sized dust particles*** are formed by condensation

![PX282 - L2a - core accretion I.png|500](/img/user/pics/PX282%20-%20L2a%20-%20core%20accretion%20I.png)

![PX282 - L2 - core accretion.png|500](/img/user/pics/PX282%20-%20L2%20-%20core%20accretion.png)
*image: NASA, CalTech, JPL, Leiden Observatory*

- growth of particles by **pair-wise collisions***, up to $\sim 10$ km ***planetesimals***
- initially assisted by electrostatic forces, icy particles stick together readily, so they grow more rapidly beyond the snowline
- there are two problems:
	- particles become fragile as they grow and can be **eroded by higher velocity collisions**
	- **gas drag** on particles in the disc, causing the larger particles to spiral in towards the sun
- considering orbit with the gas disc:
$$\underbrace{\frac{v^{2}}{r} = \frac{GM_{\odot}}{r^{2}}}_\text{keplerian orbits} + \underbrace{ \frac{dP}{dr} \frac{1}{\rho}}_\text{additional term}$$
- the additional term is for support against gravity for gas only, assuming a negative pressure gradient in disc
- $v_{g}\simeq 0.0995\,v_{kep} \implies$ solid particles feel a headwind; at $1$ AU, $v_{wind} \simeq 100$ ms$^{-1}$
- there will be significant drag on the solids that leads to settling of solid particles into disc mid-plane and gradual spiral in towards the proto-sun
- the drag force:
$$F_{D} = \frac{1}{2} C_{D} \, \pi R_{p}^{2} \, \rho_{gas} \, (v_{kep} - v_{gas})^{2} $$
	where, $C_{D}$ is the drag coefficient, $\pi R_{p}^{2}$ is the cross-section of the particle

- the characteristic timescale to modify the orbit:
$$\begin{gather}
\tau_{D }\simeq \frac{m_{p}v_{kep}}{|F_{D}|} \\\\
m_{p} = \frac{4}{3} \pi R_{p}^{3} \rho_{p} \\\\
\tau_{D }\simeq \frac{8}{3} \frac{1}{C_{D}} \frac{\rho_{p}}{\rho_{gas}} \frac{R_{p}v_{kep}}{(v_{kep}-0.995v_{kep})^{2}} \\
\simeq \frac{8}{3} \frac{1}{C_{D}} \frac{\rho_{p}}{\rho_{gas}} \frac{1}{0.005^{2}} \frac{R_{p}}{v_{kep}}
\end{gather}$$
- at 1 AU: $v_{kep} = 3\times10^{4}$ ms$^{-1}$ $\implies v_{wind}\simeq 100$ ms$^{-1}$
- for a planet, $\tau_{D} \sim 10^{8}$ yr $\gg$ life time of a gas disc $(\sim 10^{6} - 10^{7})$
- for a dust particle, $\tau_{D} \sim$ seconds, so it is carried by gas
- for a 1 m object, $\tau_{D} \sim 1000$ years, so they will spiral into the sun and will be lost from the disc

- there is a significant pattern for core-accretion scenario
- possible solutions:
	- structures in disc can trap particles in high pressure regions promoting rapid growth
	- streaming instabilities can cause clumps of particles, shielding each other from the disc headwind

- the planetesimals further grow into **proto-planets** $(\sim 0.1\,M_{\oplus})$ assisted by mutual gravity
- this stops at **isolation mass**, when the hill sphere of the planet has swept out an annuls of the disc

- more massive cores form beyond the snowline, where ices can form
- the surface density of disc:
$$\begin{gather}
\Sigma \propto r^{-3/2} \\
\implies dm \propto 2\pi r \, dr \, r^{-3/2} \propto r^{-1/2}\,dr
\end{gather}$$
	where, ${} 2\pi r \,dr {}$ is the area of an annulus of disc, and $dm$ is the mass of solids in an annulus of thickness, $dr$

- spacing of the planets $(dr)$ increases $\propto r \implies m_{core} \propto r^{1/2}$
- for jupiter:
$$M_{core}(5\,\text{ AU}) \simeq M_{core}(1\,\text{AU}) \times 5^{1/2} \times 4 \simeq 9M_\oplus$$
- taking $M_{core}$ at 1 AU to be $M_{\oplus}$, and the factor of $4$ accounts for ice as well as rock
- massive cores form rapidly beyond the snowline, capable of accreting gas

- massive cores accrete gas from disc
- gas fills the hill sphere of the planet, but it must radiate its gravitational potential energy to cool and settle on the planet
- initially, this is slow as diffuse gas cools inefficiently (cooling rate $\propto \rho^{2}$)
- the gas accretion rate increases as gas mass increases, and the gas gets compressed, so it radiates more efficiently
- eventually, it becomes a runaway process that rapidly accretes all the gas in disc annulus
- this is how a gas giant is formed
- the timescale is similar to disc lifetime
- if the disc is dispersed during slow gas accretion phase, an ice giant is formed

![PX282 - L2 - core accretion-2.png|500](/img/user/pics/PX282%20-%20L2%20-%20core%20accretion-2.png)
*image: Pollack, et al (1996)*; legend: $M_{z} :$ solids, $M_{XY}:$ gases, $M_p:$ planet (combined)

- initially, rocky/icy core assembles rapidly
- then, there is slow accretion of gas, limited by cooling
- eventually, there is runaway gas accretion to a gas giant
- the gas accretion is halted by photoevaporation of the disc by the young sun
- recalling, for planet atmospheres:
$$\frac{3}{2} kT  \simeq \frac{1}{2} m_{p} \bar v^{2}$$
	where, $T$ is the temperature of the heated disc atmosphere $\simeq 10000$ K
- considering the escape velocity from the sun:
$$v_{esc} = \sqrt{\frac{GM_{\odot}}{r}}$$
	where, $r$ is the distance from the sun

- equating the two velocities:
$$r = \frac{2GM_{\odot}m_{p}}{3kT }\simeq 10\,\text{Au}$$
- beyond this $r$, photoevaporation of the outer disc can be seen, shutting off the supply of gas to the inner disc

- terrestrials assembled via giant collisions between protoplanets, after disc dispersal
- the gravitational perturbation of orbits cause the eccentricity to be increased, causing crossing orbits and collisions
- previously, orbits were circularised by interaction with the gas disc
- evidence for giant collisions:
	- presence and composition of earth's moon (same as earth's mantle)
	- high density of mercury (missing mantle material, lost in collision)
	- spin obliquity of uranus
- from the radioisotope dating of moon rocks and meteorites, the moon can be dated back to $\sim 4.5$ Gyr
- the solar system is $4.6$ Gyr old, and the assembly of the terrestrials took $\sim 10^{8}$ years
