---
{"dg-publish":true,"permalink":"/content/012/px-275-mathematical-methods/b-coordinate-systems-and-integration/b2-4-integration/px-275-b2b-simple-examples-of-line-integrals/","noteIcon":"1","created":"2024-11-25T10:50:32.000+00:00","updated":"2024-11-26T10:04:48.690+00:00"}
---

## length of a line
![Pasted image 20241021122320.png](/img/user/pics/Pasted%20image%2020241021122320.png)
- a length, $s:$ 
$$s = \int_{s_{1}}^{s_{2}} ds$$
$$\begin{align*}
	ds &= dx\sqrt{1+ \left(\frac{dy}{dx}\right)^{2}} \\
	&= dx\sqrt{1+m^{2}} \\
	\implies s &= \int_{x_{1}}^{x_{2}} \sqrt{1+m^{2}} \,dx
\end{align*}$$
## length of a curve
![Pasted image 20241021122256.png](/img/user/pics/Pasted%20image%2020241021122256.png)
$$ds^{2}= \delta\rho^{2}+ (\rho \, \delta\phi)^{2}$$
- in the arc of a circle: $\delta \rho =0 \implies ds = \rho d\phi$
$$s = \int_{\phi_{1}}^{\phi_{2}} \rho\,d\phi$$
