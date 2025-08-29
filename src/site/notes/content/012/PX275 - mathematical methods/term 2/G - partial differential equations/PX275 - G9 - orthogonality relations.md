---
{"dg-publish":true,"permalink":"/content/012/px-275-mathematical-methods/term-2/g-partial-differential-equations/px-275-g9-orthogonality-relations/","noteIcon":"1","created":"2025-08-27T13:15:23.685+01:00","updated":"2025-04-29T18:40:54.000+01:00"}
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
	\frac{\partial u(x,0)}{\partial t} = \sum\limits_{n}\sin\left( \frac{n\pi x}{L}\right) D_{n} \frac{n\pi x}{L} = V_{0} \delta(x-x_{0}) \tag{2}
\end{gather}$$

- from equation $(1):$
$$\begin{align*}
\int_{0}^{L} f(x) \sin\left( \frac{m\pi x}{L}\right) \, dx &= \sum\limits_{n} C_{n} \int_{0}^{L}\sin\left( \frac{n\pi x}{L}\right) \sin\left( \frac{m\pi x}{L}\right) \, dx \\
\int_{0}^{L} f(x) \sin\left( \frac{m\pi x}{L}\right) \, dx &= \sum\limits_{n}C_{n}\delta_{nm} \frac{L}{2}  \\
\frac{2}{L}\int_{0}^{L} f(x) \sin\left( \frac{m\pi x}{L}\right) \, dx  &= C_{m} \\
\end{align*}$$

- the initial shape of the string sets $C_{n}$ set of coefficients

## initial velocity example 1
- consider the function as:
$$f(x) = \begin{cases} \cfrac{2\epsilon}{L}x & \text{for } 0 \le x \le \cfrac{L}{2}, \\ \cfrac{2\epsilon}{L}(L-x) & \text{for } \frac{L}{2} \le x \le L\end{cases}$$

![PX275 - G9 - orthogonality relations-4.png|500](/img/user/pics/PX275%20-%20G9%20-%20orthogonality%20relations-4.png)

- integrating the equation for $C_n:$
$$\begin{align*}
C_{n} &= \frac{4\epsilon}{L^{2}} \int_{0}^{L/2}x \sin \left(\frac{n\pi x}{L}\right) \, dx + \frac{4\epsilon}{L^{2}} \int_{L/2}^{L} (L-x) \sin\left(\frac{n\pi x}{L}\right)\,dx \\
&=\dots \\
&= \frac{8\epsilon\sin(n\pi/2)}{n^{2}\pi^{2}}
\end{align*}$$

$$\therefore u(x,t) = \sum\limits_{n} \left[ \frac{8\epsilon\sin(n\pi/2)}{n^{2}\pi^{2}} 
\sin\left(\frac{n\pi x}{L}\right) \cos\left(\frac{n\pi ct}{L}\right)  + D_{n} \sin \left(\frac{n\pi x}{L}\right)  \sin \left(\frac{n\pi ct}{L}\right) \right]$$

- eg: if the string is released from an initial stationary state
$$\begin{gather}
\frac{\partial u}{\partial t}(x,0) = 0 \; \forall x \\
\frac{\partial u}{\partial t}(x,0) = \sum\limits \sin\left(\frac{n\pi x}{L}\right)  D_{n} \frac{n\pi c}{L} \\
\implies D_{n} = 0
\end{gather}$$
$$\therefore u(x,t) = \sum\limits_{n} \left[ \frac{8\epsilon\sin(n\pi/2)}{n^{2}\pi^{2}} 
\sin\left(\frac{n\pi x}{L}\right) \cos\left(\frac{n\pi ct}{L}\right) \right] \propto \epsilon/n^{2}$$
- since $\sin\frac{n\pi}{2}= 0$ for $n\in$ even, only odd harmonics exist

![PX275 - G9 - orthogonality relations.png|250](/img/user/pics/PX275%20-%20G9%20-%20orthogonality%20relations.png) ![PX275 - G9 - orthogonality relations-1.png|250](/img/user/pics/PX275%20-%20G9%20-%20orthogonality%20relations-1.png)
*image: A-M Broomhall, lecture notes*

## initial velocity example 2

$$\begin{gather}
\frac{\partial u}{\partial t}(x,0) = \sum\limits_{n}\sin\left(\frac{n\pi x}{L}\right) D_{n} \frac{n\pi c}{L} = V_{0} \delta(x - x_{0}) \\
\int_{0}^{L} \sum\limits_{n}\sin\left(\frac{n\pi x}{L}\right) \sin \left(\frac{m\pi x}{L}\right) D_{n} \frac{n\pi c}{L} \, dx=  \int_{0}^{L} V_{0} \delta(x - x_{0}) \sin \left(\frac{m\pi x}{L}\right) \, dx \\
\sum\limits_{n} D_{n}  \frac{n\pi c}{L} \delta_{nm} \frac{L}{2} = V_{0} \sin\left(\frac{m\pi x_{0}}{L}\right) \\
\therefore D_{m} = \frac{2V_{0}}{cm\pi}  \sin\left(\frac{m\pi x_{0}}{L}\right)
\end{gather}$$

![PX275 - G9 - orthogonality relations-2.png|250](/img/user/pics/PX275%20-%20G9%20-%20orthogonality%20relations-2.png) ![PX275 - G9 - orthogonality relations-3.png|250](/img/user/pics/PX275%20-%20G9%20-%20orthogonality%20relations-3.png) 
*image: A-M Broomhall, lecture notes*

