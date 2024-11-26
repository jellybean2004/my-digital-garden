---
{"dg-publish":true,"permalink":"/content/011/px-153-mathematics-for-physicists/term-1/px-153-e-second-order-inhomogeneous-od-es/px-153-e2-method-of-undetermined-coefficients/","created":"2024-11-25T10:50:32.000+00:00","updated":"2024-11-26T19:37:15.454+00:00"}
---

- just a posh way of saying [[content/011/PX153 - mathematics for physicists/term 1/PX153 - E - second order inhomogeneous ODEs/PX153 - E1 - recap and introduction\|PX153 - E1 - recap and introduction]]
- method of finding the particular integral
	- essentially "guess" a trial solution based on the form of $f(x)$
	- substitute it into the ODE and find the undetermined coefficients

| $f(x)$                                     | trial solution                                                                    |
| ---------------------------------------- | --------------------------------------------------------------------------------- |
| polynomial of degree $n$, eg: $x^3+2x+1$ | polynomial of degree $n$, eg: $y_{p}= \alpha x^{3}+\beta x^{2}+\gamma x + \delta$ |
| $\cos qx or \sin qx$                     | $y_{p}=\alpha \cos qx + \beta \sin qx$                                            |
| $pe^qx$                                  | $y_{p}(x)=\alpha e^{qx}$                                                          |

- similarly, in the case of a *repeated root in the auxiliary equation*, we can have a problem if the usual trial function is already in the complementary function. as with the repeated root, our solution is to multiply by the independent variable.
	- eg: find the general solution to: 
	$$y''-y'-6y = e^{3x}$$
		- complementary function from before
		$$y_{c}(x) = Ce^{3x}+De^{2x}$$
		- trial function for $e^{3x}$ will not work
		- instead, we try $y_{p}(x) = \alpha x e^{3x}$
		$$y_{p}' = \alpha e^{3x}+3\alpha xe^{3x}$$
		$$y_{p}'' = 6 \alpha e^{3x}+ 9\alpha xe^{3x}$$
		$$(6 \alpha e^{3x}+ 9\alpha xe^{3x})-(\alpha e^{3x}+ 3\alpha xe^{3x})-6\alpha x e^{3x}=e^{3x}$$
		- terms in $xe^{3x}: 9\alpha-3\alpha-6\alpha = 0$
		- terms in $x^{0}e^{3x}: 6\alpha-\alpha = 1 \implies \alpha = \frac{1}{5}$
		$$\therefore G.S. : y(x) = y_{c}+ y_{p} = Ce^{3x}+De^{2x} + \frac{1}{5} e^{3x}$$
- if $f(x)$ contains a *sum of functions*, then our trial function will also be the sum of the functions
	- eg: for $ay''+by'+cy = 3\sin(2x) +1+x^{2}$
		- try: $\alpha \sin(2x) +\beta\cos(2x)+(\gamma+\delta x + \epsilon x^{2})$
- ***note***: the trial functions we gave assumed an ODE of the form $ay''+by'+cy = f(x)$
	- if this is not the case, think more carefully
	- eg: solve $y'' - 2y' = -5\cos(x)-2$
		- no term in $y$
		- first, solve complementary equation:
			- auxiliary equation: $l^{2}-2l = 0$
				$l_{1}=0, \; l_{2}=2$
			$$y_{c}= A+Be^{2x}$$
		- particular solution: $y_{p}(x) = C \cos(x)+D\sin(x)+Ex$
			- sub into ODE: $-C\cos(x)-D\sin(x)+2C\sin(x)-2D\cos(x)-2E = -5\cos(x)-2$
			- constant term: $-2E = -2 \implies E=1$
			- $\cos(x)$ term: $-C-2D = -5$
			- $\sin(x)$ term: $-D+2C=0 \implies D=2C$ 
				$\therefore C=1, \; D=2$
			- hence, 
			$$\therefore G.S.: y(x) = A + Be^{2x} + \cos(x) + 2\sin(x) + x$$
