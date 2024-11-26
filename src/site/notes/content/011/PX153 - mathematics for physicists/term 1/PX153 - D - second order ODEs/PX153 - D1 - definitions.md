---
{"dg-publish":true,"permalink":"/content/011/px-153-mathematics-for-physicists/term-1/px-153-d-second-order-od-es/px-153-d1-definitions/","created":"2024-11-25T10:50:32.000+00:00","updated":"2024-11-26T19:37:03.766+00:00"}
---

- a linear ODE can be written  in the form: 
$$a_{n}(x) \frac{d^{n}y}{dx^{n}}+ a_{n-1}(x)\frac{d^{n-1}y}{dx^{n-1}}+...a_{1} \frac{dy}{dx}+ a_{0}(x)y = f(x)$$
	- dependent variable and its derivatives are only present to first order (no $y^2$, etc)
	- no non-linear functions of the dependent variable (no sin(y), etc)
	- no products of the dependent variable and its derivatives (no $y\frac{dy}{dx}$, etc)

- a linear ODE is homogeneous if $f(x)=0$
	- then, if $y$ is a solution, so is $Ay$, or if $y_1$ and $y_2$ are both solutions, so is $Ay_{1}+By_2$ 
	- if $f(x) \neq 0$ and the ODE is linear, then it is inhomogeneous
	- eg: 
		- $\sin x \frac{dy}{dx}=x-y$ - 1st order, linear, inhomogeneous
		- $\ddot x + \gamma \dot x + \omega_{0}^{2}x = 0$ - 2nd order, linear, homogeneous
		- $\ddot x + \gamma \dot x + \omega_{0}^{2}x = b \cos \omega t$ - 2nd order, linear, inhomogeneous
		-  $\ddot x + \gamma \dot x + x(x^{2}-1) = b \cos \omega t$ - forced Duffing's equation - 2nd order, non-linear

- the solution of an ODE is the relationship between the independent and dependent variable over a specified domain
- the general solution contains all solutions of the ODE 
- for a linear homogeneous ODE, if $y_1(x)$ and $y_2(x)$ are solutions, so is $y(x)= Ay_1(x)+By_2(x)$
- eg: for $\ddot x + \omega_{0}^{2}x =0$
	- solutions: $x_{1}=Ae^{i\omega_{0}t}, x_{2}=Be^{-i\omega_{0}t}$
	- consider a constant times $x_{1}$, ie: $x=Cx$ : 
	$$\ddot x +\omega_{0}^{2} = C\ddot x_{1} + C \omega_{0}^{2} x_{1} = C(\ddot x_{1}+ \omega_{0}^{2}x_{1})=0$$
	- for $x=Cx_{1}+Dx_{2}$: 
	$$\begin{align}
	  \ddot x + \omega_{0}^{2}x &= \frac{d^{2}}{dt^{2}} (Cx_{1}+Dx_{2}) + \omega_{0}^{2}(Cx_{1}+Dx_{2})\\
	  &= C(\ddot x_{1} + \omega_{0}^{2} x_{1}) + D(\ddot x_{2}+\omega_{0}^{2}x_{2}) \\
	  &=0
	  \end{align}$$
	  - so, $x$ is a solution
	  - **note**: not true for inhomogeneous or non-linear
- for a second order ODE, expect two constants of integration
- the particular solution satisfies a given set of boundary conditions