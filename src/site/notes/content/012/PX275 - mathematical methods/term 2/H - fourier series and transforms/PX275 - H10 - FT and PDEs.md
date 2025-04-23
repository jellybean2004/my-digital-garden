---
{"dg-publish":true,"permalink":"/content/012/px-275-mathematical-methods/term-2/h-fourier-series-and-transforms/px-275-h10-ft-and-pd-es/","noteIcon":"1","created":"2025-02-13T12:24:10.594+00:00","updated":"2025-03-27T12:17:19.493+00:00"}
---

## the wave equation
- for a multivariable function, $u(x,t)$, FT can be done with respect to $x$, $t$ or both
- considering the wave equation:
$$\frac{\partial^{2} {u}}{\partial {x}^{2}} = \frac{1}{c^{2}}\frac{\partial^{2} {u}}{\partial {t}^{2}}$$

$$\begin{align*}
\tilde u(k) &= \int_{-\infty}^{\infty} e^{ikx} u(x)\,dx \\
\tilde u(\omega) &= \int_{-\infty}^{\infty} e^{i\omega t} u(t)\,dt
\end{align*}$$

- these can be combined to form a 2D FT:
$$\tilde u(k,\omega) = \tilde u(k) = \iint_{-\infty}^{\infty} e^{i(kx+\omega t)} u(x,t)\,dx\,dt$$
- using the formula for the FT of the $n^{th}$ derivative:
$$\begin{gather}
\mathcal F \left(\frac{\partial^{n} {f}}{\partial {x}^{n}}\right) = (ik)^{n} \tilde f(k) \\
\mathcal F \left(\frac{\partial^{n} {f}}{\partial {t}^{n}}\right) = (ik)^{n} \tilde f(\omega) 
\end{gather}$$

- taking the FT of both sides of the wave equation:
$$(ik)^{2} \tilde u(k,\omega) = \frac{1}{c^{2}} (i\omega)^{2} \tilde u(k,\omega) \implies \left(\frac{\omega^{2}}{c^{2}}- k^{2}\right)  \tilde u(k,\omega) = 0$$
- this yields the dispersion relation:
$$\omega^{2} = k^{2}c^{2}$$
## the diffusion relation
$$\frac{\partial  u}{\partial t} = D \frac{\partial^{2} {u}}{\partial {x}^{2}}$$
- taking the FT of both sides:
$$\begin{gather}
\int_{-\infty}^{\infty} e^{-ikx} \frac{\partial u}{\partial t}\,dx = D \int_{-\infty}^{\infty} e^{-ikx} \frac{\partial^{2} {u}}{\partial {x}^{2}}\,dx \\
\frac{\partial}{\partial t}\int_{-\infty}^{\infty} e^{-ikx} u\,dx = -Dk^{2}\tilde u \\
\frac{\partial \tilde u}{\partial t} = - Dk^{2} \tilde u
\end{gather}$$
- this turned it into a first order PDE
- the solutions for $\tilde u$ will have the form:
$$\tilde u(k,t) = \tilde A (k) e^{-Dk^{2}t}$$
	where, $\tilde A(k)$ is an undetermined function of only $k$

- to find the solutions for $u$, taking the inverse FT:
$$u = \frac{1}{2\pi} \int_{-\infty}^{\infty} e^{ikx} \tilde A(k) e^{-Dk^{2}t} ,dx$$

- considering a special case of $\tilde A(k) = 1:$
$$u = \frac{1}{2\pi} \int_{-\infty}^{\infty} e^{ikx} e^{-Dk^{2}t} \,dx$$
- this is the FT of a gaussian:
$$\begin{gather} 
f(x) = \sqrt{\frac{\alpha}{\pi}} e^{-\alpha x^{2}} \\
\tilde f(k) = e^{-k^{2}/4\alpha}
\end{gather}$$
$$\therefore u(x,t) = \frac{1}{\sqrt{4\pi D t}} \exp\left(\frac{-x^{2}}{4Dt}\right)$$

- for the general case, including $\tilde A(k)$, this is a product of two functions, $\tilde A(k)$ and $\tilde G(k,t) = \exp(-Dk^{2}t)$
$$u = \mathcal F^{-1} (\tilde A(k) \, \tilde G(k,t)) = A * G(x,t)$$
- so, it is a convolution between $A(x)$ and $G(x,t)$ 
- since $\tilde G = \exp(-Dk^{2}t):$
$$G = \frac{1}{\sqrt{4\pi Dt}} \exp\left(- \frac{x^{2}}{4Dt}\right)$$
- therefore, the solution:
$$u = A * G = \int_{-\infty}^{\infty} A(y) G(x-y, t)\,dy$$

-  considering an initial condition: $u(x,t=0)$
- recalling the definition of a $\delta$ function: $$\lim_{\text{width}\to 0} G(x-y) = \delta(x-y)$$
- it can be considered a 'local injection' at $x=y$
- if $G$ is a $\delta$-function at$t=0:$
$$u(x,0) = \int_{-\infty} ^{\infty} A(y) \, \delta(x-y)\, dy = A(x)$$
- so, it can be seen how the initial condition settles $A(x)$, and this $\tilde A(k)$
- $\tilde A(k) = 1$ is the case where $u(x,0) = \delta(x)$
- for $t>0:$
$$u(x,t) = \int_{-\infty}^{\infty} A(y)\, G(x-y, t) \, dy = \int_{-\infty}^{\infty} u(y,0) \, G(x-y, t) \, dy$$

- as seen before, convolutions with gaussians broaden and smear them
- similarly, the initial condition is broadened over time as the particles diffuse