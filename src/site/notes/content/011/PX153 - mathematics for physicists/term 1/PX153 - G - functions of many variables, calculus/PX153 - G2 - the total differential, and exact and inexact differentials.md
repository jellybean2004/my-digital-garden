---
{"dg-publish":true,"permalink":"/content/011/px-153-mathematics-for-physicists/term-1/px-153-g-functions-of-many-variables-calculus/px-153-g2-the-total-differential-and-exact-and-inexact-differentials/","noteIcon":"1","created":"2024-11-25T10:50:32.000+00:00","updated":"2024-11-26T19:37:36.862+00:00"}
---

- if we think of a 3D plot of $f(x,y)$, it is clear that the gradient changes depending on the direction
- we define the *total differential* as: 
$$df = \frac{\partial f}{\partial x}dx + \frac{\partial f}{\partial y}dy$$
- more generally, we can write the small change as you change variables by a small amount as: 
$$df = A(x,y)dx + B(x,y)dy$$
	- this is no longer explicitly l\inked to a function, $f(x,y)$

- we say that a differential is exact if and only if it can be integrated to a function of the variables, $f(x,y)$. 
- an exact differential can always be integrated to a function, and the differential found from the derivative of a function is always exact
- comparing the two equations above gives:
$$A(x,y) = \frac{\partial f}{\partial x} \;and \; B(x,y) = \frac{\partial f}{\partial y}$$ such that: 
$$\frac{\partial A}{\partial y} = \frac{\partial^{2} f}{\partial y \partial x}= \frac{\partial^{2} f}{\partial x \partial y} = \frac{\partial B}{\partial x}$$
- so, a differential is exact if and only if: 
$$\frac{\partial A}{\partial y} = \frac{\partial B}{\partial x}$$
- eg: is $x.dy+2y.dx$ exact?
	- compare with $df = A.dx + B.dy$
	- $A = 2y$ and $B=x$ 
	- $\frac{\partial A}{\partial y} = 2 \neq \frac{\partial B}{\partial yx} = 1$
	- so, not an exact differential
- we can extend this to multiple variables: 
$$df = \sum\limits_{i=1}^{n} g_{i}(x_{1}...x_{n})dx_{i}$$
- is exact if 
$$\frac{\partial g_{i}}{\partial x_{j}} = \frac{\partial g_{j}}{\partial x_{i}}$$ for all pairs of $i$ and $j$

- eg: show that the following pairs of differential is exact and find the function from which the differential is derived: 
$$(y+z).dx +x.dy +x.dz$$
	$$df = g_{x}.dx +g_{y}.dy+g_{z}.dz$$
		$g_{x}=y+z$, $g_{y}= x$, and $g_{z}=x$
		$\frac{\partial g_{x}}{\partial y} = 1 = \frac{\partial g_{y}}{\partial x}$, $\frac{\partial g_{x}}{\partial z} = 1 = \frac{\partial g_{z}}{\partial x}$, $\frac{\partial g_{y}}{\partial x} = 0 = \frac{\partial g_{z}}{\partial y}$
	- so, it is exact: 
	$$df = \frac{\partial f}{\partial x}dx + \frac{\partial f}{\partial y}dy + \frac{\partial f}{\partial z}dz$$
	$$\frac{\partial f}{\partial x} = y+z \implies f(x,y,z) = x(y+z)+h_{x}(y,z)+c$$
	$$\frac{df}{dy}= x \implies f(x,y,z) = xy + h_{y}(x,z) +c$$
	$$\frac{df}{dz}= x \implies f(x,y,z) = xz + h_{z}(x,y) +c$$
		- these are satisfied by: $f(x,y,z) = x(y+z)+c$

		- the constant of integration could involve other variables held constant