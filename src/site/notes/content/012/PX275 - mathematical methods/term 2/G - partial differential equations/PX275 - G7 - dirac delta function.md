---
{"dg-publish":true,"permalink":"/content/012/px-275-mathematical-methods/term-2/g-partial-differential-equations/px-275-g7-dirac-delta-function/","noteIcon":"1","created":"2025-08-27T13:15:23.669+01:00","updated":"2025-01-29T13:01:10.000+00:00"}
---

[[content/012/PX275 - mathematical methods/term 1/E - stoke's theorem and the divergence theorem/PX275 - E2b - dirac delta\|PX275 - E2b - dirac delta]]

- the motivation is to explore another condition
- for a vibrating string, governed by the wave PDE, considering injecting a local impulse near $x = x_0$, ie. hitting it with a hammer of width, $w$
- so, the impulse acts on a range: $x_{0} - w/2$ to $x_{0} + w/2$

$$\frac{\partial u(x,0)}{\partial t} = \begin{cases}
0 & x < x_{0}- w/2 ,\\
V_{0} & x_{0} - \frac{w}{2}<x<x_{0} + w/2 ,\\
0 & x > x_{0}+ w/2
\end{cases}$$

- making the hammer narrower and narrower, ie: $w\to 0$, for a constant ${} V_0: {}$
$$\int \frac{\partial u(x,0)}{\partial t}\,dx \to 0$$

![PX275 - G7 - dirac delta function.png|500](/img/user/pics/PX275%20-%20G7%20-%20dirac%20delta%20function.png)

- but if $V_{0} \propto 1/w$, ${} \lim_{w\to0} V_{0} \to \infty: {}$
$$\int \frac{\partial u(x,0)}{\partial t}\,dx = \text{const}$$

![PX275 - G7 - dirac delta function-1.png|500](/img/user/pics/PX275%20-%20G7%20-%20dirac%20delta%20function-1.png)

- the limit of a step function is the **dirac delta function**, $\delta(x)$
- it is normalized, ie:
$$\int_{-\infty}^{\infty} \delta(x )\,dx = 1$$
- in the limit, the function has **zero width**, and **infinite height**
- the function is non-zero only at a single $x$ value
## definition 1
- only non-zero at a single $x$
$$\delta(x) = \begin{cases} 0 & |x|>w/2, \\ 1/w & |x|\leq w/2\end{cases}$$

## definition 2
- the limit of a gaussian:
$$\lim_{w\to0} \delta(x) = N\exp\left(- \frac{x^{2}}{w^{2}}\right)$$
- this can be normalized
- it is arbitrarily narrow
$$\delta(x-x_{0}) =  \begin{cases} 0 & x\neq x_{0} \\ \infty & x = x_{0} \end{cases}$$
$$\int\delta(x-x_{0}) = \begin{cases}
1 & \text{if integration range includes $x_0$},\\
0 & \text{otherwise}
\end{cases}$$
- this can be used for:
$$\int f(x)\delta(x-x_{0}) = \begin{cases}
f(x_0) & \text{if integration range includes $x_0$},\\
0 & \text{otherwise}
\end{cases}$$

## implementation
- using the dirac delta function for the local injection of pulse
$$\begin{gather}
	u(x,0) = 0 & 0<x<L \\
		\frac{\partial u(x,0)}{\partial t} &= V_{0} \, \delta(x-x_{0})
\end{gather}$$

- for a clamped string:
$$u(x,t) = \sum\limits_{n} \sin\left(\frac{n\pi x}{L}\right) \left( C_{n}' \cos\left(\frac{n\pi t}{L}\right)+ D_{n}' \sin\left(\frac{n\pi t}{L}\right)\right)$$
$$u(x,0) = \sum \sin \left(\frac{n\pi x}{L}\right) C'_{n} \; \forall x$$
$$\implies C'_{n} = 0 \; \forall n$$
$$\frac{\partial u(x,t)}{\partial t} = \sum\limits_{n} \sin\left(\frac{n\pi x}{L}\right) D_{n}'  \frac{n\pi c}{L}\cos\left(\frac{n\pi ct}{L}\right)$$
- at $t = 0:$
$$\sum\limits_{n} \sin\left(\frac{n\pi x}{L}\right) D_{n}'  \frac{n\pi c}{L} = V_{0} \; \delta(x-x_{0})$$
