---
{"dg-publish":true,"permalink":"/content/012/px-282-stars-and-solar-system/term-2-solar-system/l-formation-of-solar-system/px-282-l2-core-accretion/","noteIcon":"1","created":"2025-03-07T11:30:07.587+00:00","updated":"2025-03-07T18:25:35.067+00:00"}
---

- firstly, the young sun and the protoplanetary disc is formed by gravitational collapse
- ***sum micron sized dust particles*** are formed by condensation
	- **sublimation zone:** very close to the proto sun, where there are no solids
	- where $T_{disc} \sim 1500$ K, there are calcium and aluminium rich minerals, as seen in meteorites
	- further out, there are silicates (eg: chondrules in meteorites and terrestrials)
	- there are also dusts of refractor elements with high sublimation temperature
	- beyond the snow line, there is water ice and volatiles in solid form, with 4 times more solid material available
	- further out is the methane line

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
where, $C_{D}$ is the drag coefficient
- the characteristic timescale to modify the orbit:
$$\begin{gather}
\tau_{D }\sim \frac{m_{p}v_{kep}}{|F_{D}|} \\
m_{p} = \frac{4}{3} \pi R_{p}^{3} \rho_{p} \\
\tau_{D }\simeq \frac{8}{3} \frac{1}{C_{D}} \frac{\rho_{p}}{\rho_{gas}} \frac{R_{p}v_{kep}}{(v_{kep}-0.995v_{kep})^{2}} \\
= \frac{8}{3} \frac{1}{C_{D}} \frac{\rho_{p}}{\rho_{gas}} \frac{1}{0.005^{2}} \frac{R_{p}}{v_{kep}}
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

- more massive cores beyond the snowline, where ices can form
$$\begin{gather}
\Sigma \propto r^{-3/2} \\
dm \propto 2\pi r \, dr \, r^{-3/2} \propto r^{-1/2}\,dr
\end{gather}$$
	where, $2\pi r dr$ is the area of an annulus of disc, and $dm$ is the mass of solids in an annulus of thickness, $dr$
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
