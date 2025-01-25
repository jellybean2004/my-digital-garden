---
{"dg-publish":true,"permalink":"/content/012/px-275-mathematical-methods/term-2/g-partial-differential-equations/px-275-g9-orthogonality-relations/","noteIcon":"1","created":"2025-01-23T10:38:25.675+00:00","updated":"2025-01-23T18:40:58.753+00:00"}
---

$$\begin{align*}
\int_{-L}^{L }\cos\left(\frac{n\pi x}{L}\right) \cos\left(\frac{m\pi x}{L}\right) \, dx &= \begin{cases} L &\text{if } n=m, \\ 0 &\text{if } n \neq m \end{cases} \\
\int_{-L}^{L }\sin\left(\frac{n\pi x}{L}\right) \sin\left(\frac{m\pi x}{L}\right) \, dx &= \begin{cases} L &\text{if } n=m, \\ 0 &\text{if } n\neq m \end{cases} \\
\int_{-L}^{L }\sin\left(\frac{n\pi x}{L}\right) \cos\left(\frac{m\pi x}{L}\right) \, dx &= 0
\end{align*}$$

## kronecker delta
- the kronecker delta is defined as:
$$\delta_{nm} = \begin{cases} 1 & \text{if } n = m, \\ 0 & \text{if } n \neq m \end{cases}$$

## application on the string
- the [[content/012/PX275 - mathematical methods/term 2/G - partial differential equations/PX275 - G6 - boundary and initial conditions\|PX275 - G6 - boundary and initial conditions]]:
$$\begin{gather}
	u(x,0) = \sum\limits_{n}\sin\left( \frac{n\pi x}{L}\right) C_{n} = f(x) \tag{1} \\
	\frac{\partial u(x,0)}{\partial t} = \sum\limits_{n}\cos\left( \frac{n\pi x}{L}\right) D_{n} \frac{n\pi x}{L} = V_{0} \delta(x-x_{0}) \tag{2}
\end{gather}$$

- from equation $(1):$
$$\begin{align*}
\int_{0}^{L} f(x) \sin\left( \frac{m\pi x}{L}\right) \, dx &= \sum\limits_{n} C_{n} \int_{0}^{L}\sin\left( \frac{n\pi x}{L}\right) \sin\left( \frac{m\pi x}{L}\right) \, dx \\
\int_{0}^{L} f(x) \sin\left( \frac{m\pi x}{L}\right) \, dx &= \sum\limits_{n}C_{n}\delta_{nm} \frac{L}{2}  \\
\frac{2}{L}\int_{0}^{L} f(x) \sin\left( \frac{m\pi x}{L}\right) \, dx  &= C_{m} \\
\end{align*}$$

- the initial shape of the string sets $C_{n}$ set of coefficients

- eg: consider the function as:
$$f(x) = \begin{cases} \cfrac{2\epsilon}{L}x & \text{for } 0 \le x \le \cfrac{L}{2}, \\ \cfrac{2\epsilon}{L}(L-x) & \text{for } \frac{L}{2} \le x \le L\end{cases}$$

- integrating the equation for $C_n:$
$$\begin{align*}
C_{n} &= \frac{4\epsilon}{L^{2}} \int_{0}^{L/2}x \sin \left(\frac{n\pi x}{L}\right) \, dx + \frac{4\epsilon}{L^{2}} \int_{L/2}^{L} (L-x) \sin\left(\frac{n\pi x}{L}\right)\,dx \\
&=\dots \\
&= \frac{8\epsilon\sin(n\pi/2)}{n^{2}\pi^{2}}
\end{align*}$$

$$\therefore u(x,t) = \sum\limits_{n} \frac{8\epsilon\sin(n\pi/2)}{n^{2}\pi^{2}} 
\sin\left(\frac{n\pi x}{L}\right) \cos\left(\frac{n\pi ct}{L}\right)  + D_{n} \sin \left(\frac{n\pi x}{L}\right)  \sin \left(\frac{n\pi ct}{L}\right) $$

- eg: if the string is released from an initial stationary state
$$\begin{gather}
\frac{\partial u}{\partial t}(x,0) = 0 \; \forall x \\
\frac{\partial u}{\partial t}(x,0) = \sum\limits \sin\left(\frac{n\pi x}{L}\right)  D_{n} \frac{n\pi c}{L} \\
\implies D_{n} = 0
\end{gather}$$
