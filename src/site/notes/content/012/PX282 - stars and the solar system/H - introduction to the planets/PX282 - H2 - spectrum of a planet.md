---
{"dg-publish":true,"permalink":"/content/012/px-282-stars-and-the-solar-system/h-introduction-to-the-planets/px-282-h2-spectrum-of-a-planet/","noteIcon":"1","created":"2025-01-10T11:27:46.125+00:00","updated":"2025-01-10T16:32:52.949+00:00"}
---


![PX282 - H2 - spectrum of a planet.png|500](/img/user/pics/PX282%20-%20H2%20-%20spectrum%20of%20a%20planet.png)
*image: D.C. Catling & J.F. Kasting, Exoplanets: Habitability and Characterization*

- there are two components in the spectrum
## the reflected component
- the luminosity:
$$L_{reflect} = \frac{L_{\odot}}{2\pi a^{2}} A_{G} \pi R_{p}^{2}$$
	where, 
		$a$ is the orbital separation of the planet from the sun, so the fraction on the RHS is the solar flux at the planet
		$A_G$ is the geometric ***albedo***, which depends on the viewing angle
		$R_{p}$ is the radius of the planet, so $\pi R_{p}^{2}$ is its cross-sectional area
- for the earth, $A_G \simeq 0.3$, so $L_{reflect} \simeq 5\times10^{16}$ W 

## the thermal component
- by equating heating and cooling, assuming no significant source of internal heat:
$$L_{in} = \frac{L_{\odot}}{4\pi a^{2}} \pi R_{p}^{2} (1-A_{B}) = 4\pi \frac{R_{\odot}^{2}\sigma T_{\odot}^{4}}{4\pi a^{2}} \pi R_{p}^{2} (1-A_{B})$$
	where, $A_{B}$ is the bond albedo (angular average)

- assuming efficient heat redistribution, eg. rapid rotation, or atmospheric lag
- (this assumes that the planet is emitting from its entire surface area, whereas only receives sunlight on half of its surface at a time)
$$L_{out} = 4\pi R_{p}^{2}\sigma T_{p}^{4}$$
- equating the incoming and outgoing luminosities, the equilibrium temperature of a planet is:
$$T_{p} = (1-A_{B})^{1/4} \left( \frac{R_{\odot}}{2a} \right)^{1/2} T_\odot$$
- **note:** it does not depend on the size of the object
- for earth: $T_{p} = 255$K $=-18\degree$C
- surface temperature can be higher due to the **greenhouse effect**
- $L_{thermal} \simeq 1.2\times10^{17}$ W
- from [[content/011/PX156 - quantum phenomena/PX156A - quantum phenomena/PX156 - A - light/PX156 - A2 - blackbody radiation and laws\|wien's displacement law]]: $\lambda_{peak} = \frac{0.0029}{T_{p}} \simeq 11\,\mu$m for earth
 
![PX282 - H2 - spectrum of a planet-1.png|500](/img/user/pics/PX282%20-%20H2%20-%20spectrum%20of%20a%20planet-1.png)

