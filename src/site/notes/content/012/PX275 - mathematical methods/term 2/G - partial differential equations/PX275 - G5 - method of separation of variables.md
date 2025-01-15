---
{"dg-publish":true,"permalink":"/content/012/px-275-mathematical-methods/term-2/g-partial-differential-equations/px-275-g5-method-of-separation-of-variables/","noteIcon":"1","created":"2025-01-09T12:50:46.338+00:00","updated":"2025-01-15T19:21:52.850+00:00"}
---

- assuming that solutions can be found of the form $u(x,t) = X(x) \, Y(t)$
- so, assuming that the dependence of individual variables can be separated
$$\begin{align*}
\frac{\partial^{2} {XY}}{\partial {t}^{2}} &= c^{2}\frac{\partial^{2} {XY}}{\partial {x}^{2}} \\
X \frac{d^{2} {Y}}{d {t}^{2}} &= c^{2} Y \frac{d^{2}X}{dx^{2}} \\
\underbrace{\frac{1}{c^{2}} \frac{1}{Y}\frac{d^{2} {Y}}{d {t}^{2}}}_\text{only dependent on $t$} &= \underbrace{\frac{1}{X} \frac{d^{2}X}{dx^{2}}}_\text{only dependent on $x$} = \alpha_{s}
\end{align*}
$$
	where, $\alpha_{s}$ is a constant of separation
- three cases to consider:
	- $\alpha_{s} = 0$
	- ${} \alpha_{s} > 0 {}$
	- $\alpha_{s} < 0$

## case 1: 
$$\alpha = 0$$
- looking at the $x$-dependent term:
$$\begin{gather*}
\frac{1}{X} \frac{d^{2}X}{dx^{2}} = 0 \;\forall x \\
\implies \frac{d^{2}X}{dx^{2}} = 0 \\
\implies X(x) =  A_{0} x + B_{0}
\end{gather*}$$
	where, $A_{0}$ and $B_{0}$ are constants of integration

- now, the $y$-dependent term:
$$\frac{1}{c^{2}Y} \frac{d^{2}Y}{dt^{2}}= 0 \implies Y = C_{0}t + D_{0}$$
  where, $C_0$ and $D_{0}$ are constants of integration

- therefore, for $\alpha_{s} = 0:$
$$u(x,t) =( A_{0}x + B_{0})(C_{0}t + D_{0})$$
- this is a 'steady state'

## case 2
$$\alpha>0$$
- trying $\alpha_{s} = k^{2}$
$$\frac{1}{c^{2}Y} \frac{d^{2}Y}{dt^{2}}= k^{2} \implies Y = k^{2}c^{2}Y$$
- the solutions to this are exponentials:
$$Y(t) = Ce^{-ckt} + De^{ikt}$$
- but these are divergent, and solutions are unphysical

## case 3
$$\alpha < 0$$
- trying $\alpha_{s} = -k^{2}$ 
- the $x$-dependent term:
$$\frac{1}{X} \frac{d^{2}X}{dx^{2}}= -k^{2} \implies X = -k^{2}X$$
- the solutions to this are sinusoidal:
$$X(x) = A \cos kx + B\sin kx$$
- now, the $y$-dependent term:
$$\frac{1}{c^{2}Y} \frac{d^{2}Y}{dt^{2}}= -k^{2} \implies Y = -  (kc)^{2}Y$$
$$Y(t) = C\cos kcx + D\sin kct$$

- the wavenumber:
$$k = 2\pi / \lambda $$

## conclusion
- combining the first and the third cases:
$$u(x,t) =( A_{0}x + B_{0})(C_{0}t + D_{0}) + (A \cos kx + B\sin kx)(C\cos kcx + D\sin kct)$$
