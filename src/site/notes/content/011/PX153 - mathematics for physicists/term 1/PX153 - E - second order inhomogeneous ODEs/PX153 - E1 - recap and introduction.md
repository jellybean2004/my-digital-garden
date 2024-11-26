---
{"dg-publish":true,"permalink":"/content/011/px-153-mathematics-for-physicists/term-1/px-153-e-second-order-inhomogeneous-od-es/px-153-e1-recap-and-introduction/","created":"2024-11-25T10:50:32.000+00:00","updated":"2024-11-26T19:37:14.389+00:00"}
---

- a second order, linear, inhomogeneous ODE: 
$$a_{2}(x) \frac{d^{2}y}{dx^{2}} + a_{1}(x) \frac{dy}{dx}+ a_{0}(x)y(x)=f(x)$$
- *GS* will have 2 constants of integration, so, we will need 2 boundary conditions
- two steps: 
	- *step 1:* find the *GS* to the *complementary equation* - the homogenous version with $f(x)=0$
		- this gives $y_c(x)$ the complementary function: 
		$$a_{2}(x) \frac{d^{2}y_{c}}{dx^{2}} + a_{1}(x) \frac{dy_{c}}{dx}+ a_{0}(x)y_{c}=0$$ which will have 2 constant s of integration
	- *step 2:* find the *particular integral* - any solution to the full ODE - ie: any $y_{p}(x)$: 
	$$a_{2}(x) \frac{d^{2}y_{p}}{dx^{2}} + a_{1}(x) \frac{dy_{p}}{dx}+ a_{0}(x)y_{p}=f(x)$$ with no arbitrary constants
	- the *GS* is $y(x)=y_{c}(x)+y_{p}(x)$
$$\begin{multline} a_{2}(x) \frac{d^{2}y}{dx^{2}} + a_{1}(x) \frac{dy}{dx}+ a_{0}(x)y(x) = (a_{2}(x) \frac{d^{2}y_{c}}{dx^{2}} + a_{1}(x) \frac{dy_{c}}{dx}+ a_{0}(x)y_{c}) \\
	+ \left(a_{2}(x) \frac{d^{2}y_{p}}{dx^{2}} + a_{1}(x) \frac{dy_{p}}{dx}+ a_{0}(x)y_{p}\right)
	= 0 + f(x) \end{multline}$$
	