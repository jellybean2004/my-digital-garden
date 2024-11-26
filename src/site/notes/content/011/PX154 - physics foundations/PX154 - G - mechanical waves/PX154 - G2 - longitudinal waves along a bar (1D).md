---
dg-publish: true
---

- when the end of a bar is hit, a compression is created within the bar that then will propagate along it
- let's say the element $dx$ is compressed by an amount $d\sigma$ 
	- [YF fig 11.14] stress/strain
		- $strain = \frac{\Delta l}{l_{0}}$
	- force creates a stress: 
	$$stress= \frac{F}{A}$$
	- and a strain: 
	$$strain = \frac{d\sigma}{dx}$$
	- the stress and strain are linked by young's modulus: 
	$$Y= \frac{stress}{strain}$$
		$$or, \;stress = \frac{F}{A} = Y \frac{d\sigma}{dx}$$
	- if we follow yesterday's derivation: 
	$$\frac{Y}{\rho} \frac{\partial^{2}\sigma}{\partial x^{2}} = \frac{\partial^{2}\sigma}{\partial t^{2}}$$
		- another wave equation
		- wave speed: $v= \sqrt{\frac{Y}{\rho}}$
			- for steel: $Y = 2\times10^{11}Nm^{-2}$ ; $\rho = 8\times10^{3}kgm^{-3}$
				- $v = 5\times10^{3}ms^{-1}$
