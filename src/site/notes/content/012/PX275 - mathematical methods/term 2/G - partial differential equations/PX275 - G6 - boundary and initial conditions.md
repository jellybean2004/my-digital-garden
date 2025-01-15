---
{"dg-publish":true,"permalink":"/content/012/px-275-mathematical-methods/term-2/g-partial-differential-equations/px-275-g6-boundary-and-initial-conditions/","noteIcon":"1","created":"2025-01-15T17:40:16.042+00:00","updated":"2025-01-15T18:52:15.200+00:00"}
---

## initial conditions
- the value of the solution at time, $t = t_{0}$, or its derivative
- eg: initial shape and/or velocity
## boundary conditions
- physics problems usually directly look at finite domain

- **dirichlet boundary conditions:** values solutions take along boundaries; eg: $u(0,t) = u(L,t)$
- **neumann boundary conditions:** values of derivatives at boundaries; eg: string clamped at both ends

- previously:
$$u(x,t) =( A_{0}x + B_{0})(C_{0}t + D_{0}) + (A \cos kx + B\sin kx)(C\cos kcx + D\sin kct)$$
- defining a coordinate frame where the constants of integration vanish
- eg: aligning the string with the $x$-axis, $A_{0}= B_{0} = 0:$
$$u(x,t) = (A \cos kx + B\sin kx)(C\cos kcx + D\sin kct)$$
- taking the boundary condition of string clamped at both ends: 
$$u(0,t) = u(L,t) = 0 \; \forall t$$
$$\begin{gather}
u = A \cos 0 + B \sin  0 = 0 \implies A = 0 \\
u = A\cos kL + B\sin kL = 0 \implies B \sin kL = 0
\end{gather}$$
- for this to be true, $kL = n \pi$, where $n\in \mathbb{Z}$
- the solution now reduces to a [[content/011/PX153 - mathematics for physicists/term 2/PX153 - J - fourier series/J - fourier series\|fourier series]]:
$$u(x,t) = \sum\limits_{n}B_{n} \sin kx(C_{n} \cos \omega t + D_{n} \sin \omega t)$$
	where, $k = n\pi / L$ and $\omega = kc = n\pi c / L$

___
## recap on fourier series
- any function, $f(x)$, periodic over an interval, $2L$, can be described by a fourier series:
$$f(x) = \frac{a_{0}}{2} + \sum\limits_{n=1}^{\infty}\left(a_{n}\cos\left(\frac{n\pi x}{L}\right) +b_{n}\sin\left(\frac{n\pi x}{L}\right) \right)$$
- the average value of the function:
$$\langle{f(x)}\rangle = \frac{1}{2L} \int_{-L}^{L} f(x) \, dx = \frac{a_{0}}{2}$$
- if only interested in the value of the function over  a finite domain $(0 \leq x \leq L)$, it can be periodically extended
![PX275 - G6a - boundary and initial conditions.png|500](/img/user/pics/PX275%20-%20G6a%20-%20boundary%20and%20initial%20conditions.png)

- fourier series can thus be used to described non-periodic functions
___

- any solution over a finite domain, eg: $x \in [0,L]$, can be periodically extended outside of this domain, and thus, a fourier series a a full description of this solution
- here, the boundary conditions directly demanded $k = n\pi/L$, but the solution can always be written as a fourier series

- defining two independent constants:
$$\begin{gather}
C_{n}' = B_{n}C_{n} \\ 
D_{n}' = B_{n}D_{n}
\end{gather}$$

$$u(x,t) = \sum\limits_{n} \sin\left(\frac{n\pi x}{L}\right) \left( C_{n}' \cos\left(\frac{n\pi x}{L}\right)+ D_{n}' \sin\left(\frac{n\pi x}{L}\right)\right)$$

![PX275 - G6a - boundary and initial conditions-1.png|500](/img/user/pics/PX275%20-%20G6a%20-%20boundary%20and%20initial%20conditions-1.png)

- the lowest $n$ corresponds to the longest wavelength and the smallest wavenumber, $k$

- initial conditions can describe:
	- the shape of the string at $t=0:$ $u(x,0) = f(x)$
	- the string is released at $t=0$, ie. fully at rest at $t=0:$ $\cfrac{\partial u(x,t)}{\partial t} \bigg|_{t=0}  =0$

