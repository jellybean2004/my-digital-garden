---
{"dg-publish":true,"permalink":"/content/011/px-153-mathematics-for-physicists/term-1/px-153-g-functions-of-many-variables-calculus/px-153-g1-partital-differentiation/","noteIcon":"1","created":"2025-08-27T13:14:05.067+01:00","updated":"2024-11-26T19:37:34.000+00:00"}
---

- we need to extend calculus to cover multivariate functions
- the derivative of a function of one variable is defined by: 
$$df\frac{x}{dx} = \lim_{\Delta x\to \infty} \frac{f(x+\Delta x)- f(x)}{\Delta x}$$
- for a function of two variables, we define the partial derivative: 
$$\frac{\partial
f(x,y)}{\partial x} = \lim_{\Delta x \to \infty} \frac{f(x+\Delta x, y)- f(x,y)}{\Delta x} = (\frac{\partial f(x,y)}{\partial x})_y$$
	- the subscript $y$ implies constant $y$
- similarly, 
$$\frac{\partial
f(x,y)}{\partial y} = \lim_{\Delta y \to \infty} \frac{f(x, y+\Delta y)- f(x,y)}{\Delta y} = (\frac{\partial f(x,y)}{\partial y})_x$$
- we don't always specify what is held constant, but it is important that you're always clear about what is held constant
- for multiple variables, $x_i$: 
$$\frac{\partial}{\partial x_{i}}f(x_{1},...x_{i},...x_{N}) = \lim_{\Delta x_{i}\to\infty} \frac{f(x_{1},...x_{i}+ \Delta x_{i},...x_{N})-fx_{1},...x_{i},...x_{N}}{\Delta x_{i}}$$
- eg: $f(x,y)=e^{xy^{2}} + \frac{y}{2}$
	- $f_{x} = y^{2}e^xy^{2}$ and $f_{y} = 2yxe^{xy^{2}} + \frac{1}{2}$
- eg: $f(x,y) = e^{x}\cos y +6x +3$
	- $f_{x} = e^{x}\cos y +6$ and $f_{y} = -e^{x}\sin y$

- similarly, we can define higher order derivatives
- eg: 
$$\frac{\partial}{\partial x \partial y}f(x,y) = \frac{\partial}{\partial x}\left(\frac{\partial f}{\partial y}\right)= \lim_{\Delta\to\infty} \frac{\frac{\partial f}{\partial y}(x-\Delta x,y)-\frac{\partial f}{\partial y}(x,y)}{\partial y\partial x}$$

- eg: to find all first and second order derivatives of:
	$$f(x,y) = x^{3}y^{2}+ye^{x}+6y^{3}+1$$
	$$\frac{\partial f}{\partial x} = 3x^{2}y^{2}+ye^{x}$$
	$$\frac{\partial f}{\partial y} = 2x^{3}y + e^{x} + 18y^{2}$$
	$$\frac{\partial^{2} f}{\partial x^{2}} = 6xy^{2}+ye^{x}$$
	$$\frac{\partial^{2} f}{\partial y^{2}} = 2x^{3}+36y$$
\1\n\2\n