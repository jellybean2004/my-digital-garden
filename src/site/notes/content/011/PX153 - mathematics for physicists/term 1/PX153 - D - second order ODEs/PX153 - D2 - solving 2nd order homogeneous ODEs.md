---
{"dg-publish":true,"permalink":"/content/011/px-153-mathematics-for-physicists/term-1/px-153-d-second-order-od-es/px-153-d2-solving-2nd-order-homogeneous-od-es/","noteIcon":"1","created":"2025-08-27T13:14:08.677+01:00","updated":"2024-11-26T19:37:06.000+00:00"}
---

## derivation
- consider 
$$\frac{d^{2}y}{dx^{2}}+ \frac{dy}{dx} + 2y = 0$$
- we postulate the solution: 
$$y=Ae^{\lambda x}$$
		$$\lambda^{2}Ae^{\lambda x} + \lambda Ae^{\lambda x} + 2 Ae^{\lambda x} = 0$$ $$\lambda^{2}y + \lambda y + 2y = 0$$
- looking for a solution across a range of y: 
$$\implies \lambda ^{2}+\lambda+2=0$$
	- this is the auxiliary equation, an algebraic equation that can be solved to find $\lambda$, which has 2 solutions: 
		$$\lambda_{1}=- \frac{1}{2}(1+\sqrt 7 i)$$$$\lambda_{2}= - \frac{1}{2}(1-\sqrt 7 i)$$
- the general solution contains all possible solutions:
		$$y(x)= e^{\lambda_{1}x}+e^{\lambda_{2}x}$$
- for a particular solution, we have to apply boundary conditions
	- eg: if $y(x=0)=0$ and $\frac{dy}{dx}|_{x=0}=1$
		$y(x)= Ce^{\lambda_{1}x}+De^{\lambda_{2}x}$
		$y(0)=C+D=0 \implies C = -D$
		$\frac{dy}{dx}= \lambda_{1}Ce^{\lambda_{1}x} + \lambda_{2}De^{\lambda_{2}x}$
		at $x=0: \frac{dy}{dx} = \lambda_{1}C + \lambda_{2}D = 1$
		$\implies (\lambda_{1}-\lambda_{2})C = 1$
		$\lambda_{1} = - \frac{1}{2}(1+\sqrt7 i); \lambda_{2} = - \frac{1}{2}(1-\sqrt7 i)$ 
		$\implies \sqrt 7 i C = 1$
		$\implies C = -D = \frac{-1}{\sqrt7i}$
		$\therefore y(x) = \frac{-1}{\sqrt7i} e^{-\frac{x}{2}}(e^{i\frac{\sqrt7i}{2}} + e^{-i\frac{\sqrt7i}{2}})$
			$= \frac{-2}{\sqrt7} e^{-\frac{x}{2}}(\sin\frac{\sqrt 7}{2}x)$
	
- for an nth order ODE, the auxiliary equation will be an nth order polynomial. we need to find n linearly independent solutions, but we can have repeated roots 
	- eg: for $\frac{d^{2}y}{dx^{2}}+ 2 \frac{dy}{dx}+ y = 0$
		- the auxiliary equation: $l^{2}+2l+1-0$
			$(l+1)^2=0$
			$l=-1$
		- we only found one solution: $y(x) = Ae^{lx}=Ae^{-x}$
		- in the case of repeated roots, if we have one solution, $y_{1}=Ae^{lx}$, then try $y_{2}=Bxe^{lx}$ (multiply by the independent variable)
		- working through this: 
				$\frac{dy_{2}}{dx} = Be^{lx}+lBxe^{lx}$
				$\frac{d^{2}y_{2}}{dx^{2}} = Ble^{lx}+Ble^{lx}+Bl^{2}xe^{lx}=2Ble^{lx}+Bl^{2}xe^{lx}$
		- show that this satisfies $\frac{d^{2}y}{dx^{2}}+ 2 \frac{dy}{dx}+ y = 0$
				$-2Be^{-x}+Bxe^{-x}+2Be^{-x}-2Bxe^{-x}+Bxe^{-x}=0$
## summary
- for a 2nd order linear homogeneous ODE:
	- try solution of the form $Ae^{\lambda x}$
	- find the auxiliary equation (quadratic in $\lambda$)
	- if there are two distinct roots, GS: $y=Ae^{\lambda_{1}x} + Be^{\lambda_{2} x}$
	- if there are repeated roots, GS: $y=Ae^{\lambda x} + Bxe^{\lambda x}$
\1\n\2\n