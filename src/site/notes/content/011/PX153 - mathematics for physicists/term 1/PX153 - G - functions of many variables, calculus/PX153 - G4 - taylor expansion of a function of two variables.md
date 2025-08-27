---
{"dg-publish":true,"permalink":"/content/011/px-153-mathematics-for-physicists/term-1/px-153-g-functions-of-many-variables-calculus/px-153-g4-taylor-expansion-of-a-function-of-two-variables/","noteIcon":"1","created":"2025-08-27T13:14:05.061+01:00","updated":"2024-11-26T19:37:39.000+00:00"}
---

- consider a power series approximation to a function of two variables, $f(x,y)$, about $x=a, y=b$
$$\begin{align} 
	f(x,y) \approxeq f(a,b) + A_{1}(x-a) + B_{1}(y-b) + A_{2}(x-a)^{2} \\+ B_{2}(y-b)^{2}+ C_{2}(x-a)(y-b)... 
\end{align}$$
- to find $A,B,C,...$ , consecutive partial derivatives of the left and the right-hand sides need to be taken: 
$$\frac{\partial f}{\partial x} = A_{1} + 2A_{2}(x-a) + C_{2}(y-b) +...$$
- evaluate at $x=a$ and $y=b$: 
$$\implies A_{1} = \frac{\partial f}{\partial x}|_{^{x=a}_{y=b}}$$
- similarly, 
$$\frac{\partial f}{\partial y} = B_{1} + 2B_{2}(y-b) + C_{2}(x-a) +...$$
$$\implies B_{1}= \frac{\partial f}{\partial y}|_{^{x=a}_{y=b}}$$
- $f_{xx} \implies A_{2} = \frac{1}{2!}\frac{\partial^{2} f}{\partial x^{2}}|_{^{x=a}_{y=b}}$
- $f_{yy} \implies B_{2} = \frac{1}{2!}\frac{\partial^{2} f}{\partial y^{2}}|_{^{x=a}_{y=b}}$
- $f_{xy} = f_{yx} \implies C_{2} = \frac{\partial^{2} f}{\partial x \partial y}|_{^{x=a}_{y=b}}$
- this gives the expansion to second order, writing $(x-a)=\Delta x$, and $(y-b)=\Delta y$ : 
$$f(x,y) \approxeq f(a,b) + f_{x}\Delta x + f_{y}\Delta y + \frac{1}{2!} f_{xx} \Delta x^{2} + \frac{1}{2!} f_{yy} \Delta y^{2} + f_{xy} \Delta x \Delta y +...$$
- following a similar process, you can derive the full expression: 
$$f(x,y) = \sum\limits_{n=0}^{\infty} \frac{1}{n!} \left[\left (\Delta x \frac{\partial}{\partial x} + \Delta y \frac{\partial}{\partial y} \right)^{n} f(x,y) \right]$$
- eg: expand the function $f(x,y) = e^{xy}$ tp 2nd order about $x=1,y=2$
		$f(1,2) = e^{2}$
		$f_{x}(1,2) = ye^{xy}|_{1,2} = 2e^{2}$
		$f_{xx}(1,2) = y^{2}e^{xy}|_{1,2} = 4e^{2}$
		$f_{y}(1,2) = xe^{xy}|_{1,2} = e^{2}$
		$f_{yy}(1,2) = x^{2}e^{xy}|_{1,2} = e^{2}$
		$f_{xy}(1,2) = (xye^{xy}+e^{xy})|_{1,2} = 3e^{2}$
	- the taylor series is: 
$$\begin{align*}
f(x,y) \approxeq e^{2}(1 + 2(x-1)+ (y-2) + \frac{1}{2!} 4(x-1)^{2} \\ + \frac{1}{2!} (y-2)^{2} + 3(x-1)(y-2)+...)
\end{align*}$$
