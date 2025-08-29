---
{"dg-publish":true,"permalink":"/content/011/px-154-physics-foundations/px-154-g-mechanical-waves/px-154-g1a-waves-on-a-taut-string/","noteIcon":"1","created":"2025-08-27T13:14:04.739+01:00","updated":"2024-11-26T19:52:20.000+00:00"}
---

[YF 15.4 "second method"]
 ![Pasted image 20231125154446.png](/img/user/pics/Pasted%20image%2020231125154446.png)
- string with a mass per unit length, $\mu$
- consider a transverse wave propagating along the string
	- oscillations of the string are only along the y-direction (no physical motion along the x-direction)
- we analyse the behaviour of a small element
![Pasted image 20231125155123.png](/img/user/pics/Pasted%20image%2020231125155123.png)
- this is a *flexible string*, ie: forces can only act along the string itself

- originally, we have tension, $T$, in the string
- motion of the string is only along the y-direction
	- therefore, $F_{1x}$ and $F_{2x}$ should be equal and opposite to each other
	- no net force, hence no acceleration, along the x-direction
	- we set $F_{1x}=F_{2x}= T$
- there will be components of force along the y-direction with a resultant force (unless the string is straight, ie: $\theta_{1}=\theta_{2}$)
	- there is a net force along $y$
	- at x, 
	$$F_{1y} = F_{1x}\tan{\theta_{1}}$$
		- acting downwards
	- writing it in terms of gradient: 
	$$F_{1y} = F_{1x} \left(\frac{dy}{dx}\right)_x$$
	- at $x+\Delta x$: 
	$$F_{2y} = F_{2x} \tan \theta_{2}$$
		- writing in terms of the gradient: 
		$$F_{2y} = F_{2x} \left(\frac{dy}{dx}\right)_{x+dx}$$
	- net force acting upwards: 
	$$F_{y} = F_{2y}-F_{1y}$$
		- if $F_{y}\neq0$, then there will be an acceleration along the y-direction, since $F=ma$, where $a = \frac{d^{2}y}{dx^{2}}$
		- for mass, we use $m=\mu x$
	- hence: 
	$$F_{y} = \mu \Delta x \frac{d^{2}y}{dx^{2}} = F_{2y}-F_{1y}$$
	- remember $F_{1x}=F_{2x}=T$: 
	$$\mu \Delta x \frac{d^{2}y}{dx^{2}} = T\left(\left(\frac{dy}{dx}\right)_{x+\Delta x}- \left(\frac{dy}{dx}\right)_{x}\right)$$
			$$\mu \frac{\partial^{2}y}{\partial t^{2}} = \frac{T\left(\left(\frac{\partial y}{\partial x}\right)_{x+\Delta x}- \left(\frac{\partial y}{\partial x}\right)_{x}\right)}{\Delta x}$$
	- let $\Delta x\to 0$: 
	$$\frac{\partial^{2}y}{\partial t^{2}} = \frac{T}{\mu} \frac{\partial^{2}y}{\partial x^{2}}$$
		- this is a wave equation
		- comparing with *[[content/011/PX154 - physics foundations/PX154 - F - waves/PX154 - F2 - the wave equation#^c8f14b\|the wave equation]]*, we see 
		$$v = \sqrt{\frac{T}{\mu}}$$
	- ***comments***:
		- this is a simple model
			- we could account for the stretching of the string
			- we could account for stiffness (perhaps a metal wire)
			- or consider the 'bead model' for wavelengths approaching distance between atoms in solids. [Y2, Y3: phonons]
