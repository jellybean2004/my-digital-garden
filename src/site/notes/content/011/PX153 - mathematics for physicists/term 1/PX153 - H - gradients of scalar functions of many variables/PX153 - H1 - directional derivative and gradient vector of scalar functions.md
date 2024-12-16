---
{"dg-publish":true,"permalink":"/content/011/px-153-mathematics-for-physicists/term-1/px-153-h-gradients-of-scalar-functions-of-many-variables/px-153-h1-directional-derivative-and-gradient-vector-of-scalar-functions/","noteIcon":"1","created":"2024-11-25T10:50:32.000+00:00","updated":"2024-11-26T19:37:47.013+00:00"}
---

- consider a continuous differentiable function, $f(x,y,z)$. we want to estimate the change of $f$ between two points in space
- let $\vec a = (x_{a}, y_{a}, z_{a})$ be the position vector to point $A$
- let $B$ be a vector $\vec u$ from $A$
- any point on the line from $A$ to $B$ can be written as $\vec r = \vec a + t\cdot\vec u$ , for $t \in [0,1]$
- we can use a taylor expansion to evaluate the values of $f$ close to $A$: 
$$f(\vec r) = f(\vec a) + \frac{\partial f}{\partial \vec r}|_{a} (\vec r-\vec a) + ...$$
$$f(x,y,z) = f(x_{a},y_{a}, z_{a}) + \frac{\partial f}{\partial x} (x-x_{a}) + \frac{\partial f}{\partial y} (y-y_{a}) + \frac{\partial f}{\partial z} (z-z_{a})$$
	$\vec r = \vec a + t \cdot \vec u$
	$\implies x = x_{a}+ t u_{x}$
		$y = y_{a}+ t u_{y}$
		$z = z_{a}+ t u_{z}$
$$\Delta f = \frac{\partial f}{\partial x}tu_{x} + \frac{\partial f}{\partial y}tu_{y} + \frac{\partial f}{\partial z}tu_{z}$$
- we can write this as a scalar product: 
$$\Delta f = \left( \frac{\partial f}{\partial x}\hat{\vec i} + \frac{\partial f}{\partial y}\hat{\vec j} + \frac{\partial f}{\partial z}\hat{\vec k} \right)|_{\vec a} \cdot t\vec u$$
- we this define the gradient operator (vector): 
$$\vec \nabla f = \frac{\partial f}{\partial x}\hat{i} + \frac{\partial f}{\partial y}\hat{j} + \frac{\partial f}{\partial z}\hat{k} = \left( \hat{i} \frac{\partial}{\partial x} + \hat{j} \frac{\partial }{\partial y}+ \hat{k} \frac{\partial}{\partial z} \right) f$$
- and we find that: 
$$\Delta f = \vec \nabla f \cdot (t \vec u)$$
- the directional derivative is defined as: 
$$D_{u}f = \lim_{t\to0} \frac{f(\vec r)-f(s)}{t} = \lim_{t\to0} \frac{\Delta f}{t} = \vec \nabla f \cdot \vec u$$
- this gives the rate of change of function in the direction of $\vec u$
	- magnitude of $\vec u$ should use $\hat{\vec u}$
