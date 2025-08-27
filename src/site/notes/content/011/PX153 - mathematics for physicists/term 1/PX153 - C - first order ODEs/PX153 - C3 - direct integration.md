---
{"dg-publish":true,"permalink":"/content/011/px-153-mathematics-for-physicists/term-1/px-153-c-first-order-od-es/px-153-c3-direct-integration/","noteIcon":"1","created":"2025-08-27T13:14:08.768+01:00","updated":"2024-11-26T19:36:53.000+00:00"}
---

## definition
- the simplest first order ODE is of the form $\frac{dy}{dx}=f(x)$, which can be solved by direct integration

- *aside*: 
	- commonly used shorthand: $\int f(x).dx$ the indefinite integral
		- further reading: section 2.2.1 and 2.2.2 of textbook
	- integration is defined by the sum, $S=\sum\limits_{i=1}^{n}f(x)(\zeta_{i}-\zeta_{i-1})$
		$S=\int_{a}^{b}f(x).dx$
			$S$ is *not* a function of $x$
			$x$ is a dummy variable
		- $S(b)$ is a function of the limits of integration
	- we can so that, if $F(x)=\int_{a}^{x}f(u).du$, then, $\frac{d}{dx}F(x)= \frac{d}{dx}(\int_{a}^{x} f(u).du)=f(x)$
	- *integration is the inverse of differentiation*
		- ***but*** differentiation does *not* have a unique inverse, therefore there is a *constant of integration*
		- so, if we have $\frac{dy}{dx}=f(x)$, then $y(x)=\int^{x}f(s).ds$
			- $y(x)=\int f(x).dx$ - is *strictly incorrect but usually used*

-  eg: $\frac{dy}{dx}=3\cos{2x}$
		$y(x)=\int 3\cos{2x}.dx$
		$y(x)=\int 3\cos{2x}.dx(=\int^x 3\cos{2x}.dx)$
		$y(x)= \frac{3}{2}\sin{2x}+c$ 
