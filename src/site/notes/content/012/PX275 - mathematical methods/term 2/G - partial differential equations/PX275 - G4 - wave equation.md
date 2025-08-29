---
{"dg-publish":true,"permalink":"/content/012/px-275-mathematical-methods/term-2/g-partial-differential-equations/px-275-g4-wave-equation/","noteIcon":"1","created":"2025-08-27T13:15:23.642+01:00","updated":"2025-01-23T19:52:27.000+00:00"}
---

- **caveat:** 
	- PDEs only tend to give nice solutions in well posed problems
	- so, only well posed problems with sufficient constraints are considered to get solutions
	- considering examples that produce 'separable solutions'

![PX275 - G4 - wave equation-1.png|500](/img/user/pics/PX275%20-%20G4%20-%20wave%20equation-1.png)

- considering the displacement of a vibrating spring, $u(x,t)$
	- density waves in a medium, $\rho(x,t)$
- forces act along the local gradient, $\cfrac{\partial u}{\partial x}$
- given a string of unknown $\tau$, the force on a test element at a position, $x:$
$$F = \tau \left[ \frac{\partial u(x+\Delta x)}{\partial x} - \frac{\partial u(x)}{\partial x}\right]$$
- from newton's second law:
$$F = ma = m \frac{\partial^{2} {u}}{\partial {t}^{2}} = \rho\, \Delta x \frac{\partial^{2} {u}}{\partial {t}^{2}}$$
	where $\rho$ is the mass density (mass per unit length)
$$\tau \left[ \frac{\partial u(x+\Delta x)}{\partial x} - \frac{\partial u(x)}{\partial x}\right]  = \rho\, \Delta x \frac{\partial^{2} {u}}{\partial {t}^{2}}$$
$$\frac{\partial^{2} {u}}{\partial {t}^{2}} = \frac{\tau}{\rho} \frac{1}{\Delta x} \left[  \frac{\partial u(x+\Delta x)}{\partial x} - \frac{\partial u(x)}{\partial x} \right] \to \frac{\tau}{\rho} \frac{\partial^{2} {u}}{\partial {x}^{2}}$$
	in the limit $\Delta x \to 0$
- so, the wave PDE:
$$\frac{\partial^{2} {u}}{\partial {t}^{2}} = \frac{\tau}{\rho} \frac{\partial^{2} {u}}{\partial {x}^{2}}$$

- the wave speed can be defined as: $c = \sqrt{\tau/\rho}$
$$\frac{\partial^{2} {u}}{\partial {t}^{2}} = c^{2}  \frac{\partial^{2} {u}}{\partial {x}^{2}}$$
- if there is friction: friction $\propto \cfrac{\partial u}{\partial t}$
	$$\implies \frac{\partial^{2} {u}}{\partial {t}^{2}} = - \eta \frac{\partial u}{\partial t} + c^{2}\frac{\partial^{2} {u}}{\partial {x}^{2}}$$
