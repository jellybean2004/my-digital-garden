---
{"dg-publish":true,"permalink":"/content/011/px-157-electricity-and-magnetism/px-157-b-electric-fields/i-field/px-157-b2a-electric-field-from-a-continuous-distribution/","created":"2024-10-01T18:27:10.053+01:00","updated":"2024-11-26T20:07:13.980+00:00"}
---

## method
- divide the distribution into small elements at $\vec r'$
- find $d\vec E$ at position, $\vec r$, for each element
- vector sum all contributions: $\vec E(\vec r) = \int d\vec E$
## linear charge density, $\lambda$
![Pasted image 20240115121159.png](/img/user/pics/Pasted%20image%2020240115121159.png)
$$
\lambda = \frac{dq}{dl}
$$
$$\begin{align} 
d \vec E &= \frac{dq}{4\pi\epsilon_{0}} \frac{\vec r - \vec r'}{|\vec r - \vec r'|^{3}} \\
&= \frac{\lambda dl}{4\pi\epsilon_{0}} \frac{\vec r - \vec r'}{|\vec r - \vec r'|^{3}} \\
\vec E &= \frac{1}{4\pi\epsilon_{0}} \int \lambda.dl \; \frac{\vec r - \vec r'}{|\vec r - \vec r'|^{3}}
\end{align}$$
## surface charge density, $\sigma$
![Pasted image 20240115121216.png](/img/user/pics/Pasted%20image%2020240115121216.png)
$$
\sigma = \frac{dq}{dS}
$$
$$\begin{align} 
d \vec E &= \frac{\sigma dS}{4\pi\epsilon_{0}} \frac{\vec r - \vec r'}{|\vec r - \vec r'|^{3}} \\
\vec E &= \frac{1}{4\pi\epsilon_{0}} \iint \sigma.dS \; \frac{\vec r - \vec r'}{|\vec r - \vec r'|^{3}}
\end{align}$$
## volume charge density, $\rho$
![Pasted image 20240115121235.png](/img/user/pics/Pasted%20image%2020240115121235.png) 
$$
\rho = \frac{dq}{d\tau}
$$
$$\begin{align} 
d \vec E &= \frac{\rho d\tau}{4\pi\epsilon_{0}} \frac{\vec r - \vec r'}{|\vec r - \vec r'|^{3}} \\
\vec E &= \frac{1}{4\pi\epsilon_{0}} \iiint \rho.d\tau \; \frac{\vec r - \vec r'}{|\vec r - \vec r'|^{3}}
\end{align}$$
- eg: a uniformly distributed charged circle, centred at the origin along the $y-z$ plane, with total charge, $Q$ ![Pasted image 20240115121253.png](/img/user/pics/Pasted%20image%2020240115121253.png)
	$$d\vec E (x,0,0) = \frac{dQ}{4 \pi \epsilon_{0}} \frac{x \hat x - \vec r'}{|x \hat x - \vec r'|^{3}}$$
	$$\vec E (x,0,0) = \int \frac{dQ}{4 \pi \epsilon_{0}} \frac{x \hat x - \vec r'}{|x \hat x - \vec r'|^{3}}$$
	
$$\begin{align*}
		E_{x}(x,0,0) &=  (\vec E \cdot \hat x) \\
		&= \int \frac{x}{4\pi\epsilon_{0}r} dQ \\
		&= \frac{x}{4\pi\epsilon_{0}r} \int dQ \\
		&= \frac{xQ}{4\pi\epsilon_{0}r} \\
		&= \frac{xQ}{4\pi\epsilon_{0}(x^{2}+a^{2})^\frac{3}{2}}
		\end{align*}$$
- also, $E_{x}(0,0,0) = 0$ , and $\lim_{x\to\pm\infty} E_{x}=0$
![Pasted image 20240115121439.png](/img/user/pics/Pasted%20image%2020240115121439.png)
