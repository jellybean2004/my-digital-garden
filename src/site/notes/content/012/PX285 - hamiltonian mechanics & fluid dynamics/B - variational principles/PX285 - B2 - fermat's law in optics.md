---
{"dg-publish":true,"permalink":"/content/012/px-285-hamiltonian-mechanics-and-fluid-dynamics/b-variational-principles/px-285-b2-fermat-s-law-in-optics/","created":"2024-11-25T10:50:32.000+00:00","updated":"2024-12-09T10:31:59.518+00:00"}
---

- light rays trace paths that extremize the *optical path length*: 
$$l = \int ds\, n(\vec r(s))$$

![Pasted image 20241209103134.png|500](/img/user/pics/Pasted%20image%2020241209103134.png)

-  consider light travelling though layers of air $(n_1)$ and water $(n_2)$
- it travels a distance, $d_{1}$, in air, and $d_{2}$ in water
$$\begin{align*}
	l &= \int n(\vec r)\,ds\\
	&= \int_{0}^{d_{1}}ds\, n_{1} + \int_{d_{1}}^{d_{1}+d_{2}}ds\, n_{2} \\
	&= n_{1}d_{1}+ n_{2}d_{2} \\
	&= n_{1}\sqrt{h_{1}^{2}+x^{2}} + n_{2}\sqrt{h_{2}^{2}+(R-x)^{2}}
\end{align*}$$
- $\frac{dl}{dx}=0 \implies l$ is the minimum wrt variation of $x:$ 
$$\begin{align*}
	\frac{dl}{dx} &= \frac{n_{1}x}{\sqrt{h_{1}^{2}+x^{2}}} + \frac{-n_{2}(R-x)}{\sqrt{h_{2}^{2}+ (R-x)^{2}}} = 0 \\
	 0 &= n_{1}\frac{x}{d_{1}} + n_{2}\frac{x-R}{d_{2}}
\end{align*}$$
- $\theta_1$ and $\theta_2$ are angles of incidence in air and water, respectively
	$d_{1}\sin\theta_{1}=x$
	$d_{2}\sin\theta_{2}=(R-x)$ 
$$\begin{gather*}
	n_{1} \frac{d_{1}\sin\theta_{1}}{d_{1}} - n_{2} \frac{d_{2}\sin\theta_{2}}{d_{2}} = 0 \\
	n_{1}\sin\theta_{1}=n_{2}\sin\theta_{2}
	\end{gather*}$$
- the above relation is *snell's law*!

- considering neighbouring paths, ie. $x_{min}\pm \delta x$, 
- the taylor expansion of $l$ at the minimum:
$$l(x)|_{x=x_{min}} = l_{min} + \underbrace{\frac{dl}{dx} \bigg|_{x=x_{min}}}_{=0} (x-x_{min}) + \frac{d^{2}l}{dx^{2}} \bigg|_{x=x_{min}}(x-x_{min})^{2} + \dots$$
- there is no difference (at lowest order) in optical path length, $l(x)$, near $x=x_{min}$
- the neighbouring paths have almost exactly the same optical path lengths, hence they interfere constructively

- considering the phase of the light wave: $\phi = (2\pi \frac{l}{\lambda}-\omega t)$, so, $\frac{d\phi}{dx} = 0 \Leftrightarrow \frac{df}{dx}=0$

 - the light 'seen' is therefore the rays passing through $x_{min}$ 
- the **realized path** is the one where the path length, $l$, is stationary with respect to varying paths, ie: have varying $x$
