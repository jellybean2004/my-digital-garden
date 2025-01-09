---
{"dg-publish":true,"permalink":"/content/012/px-275-mathematical-methods/term-2/g-partial-differential-equations/px-275-g5-method-of-separation-of-variables/","noteIcon":"1","created":"2025-01-09T12:50:46.338+00:00","updated":"2025-01-09T12:56:54.130+00:00"}
---

- assuming that solutions can be found of the form $u(x,t) = X(x) \, Y(t)$
- so, assuming that the dependence of individual variables can be separated
$$\begin{align*}
\frac{\partial^{2} {XY}}{\partial {t}^{2}} &= c^{2}\frac{\partial^{2} {XY}}{\partial {x}^{2}} \\
X \frac{d^{2} {Y}}{d {t}^{2}} &= c^{2} Y \frac{d^{2}X}{dx^{2}} \\
\underbrace{\frac{1}{c^{2}} \frac{1}{Y}\frac{d^{2} {Y}}{d {t}^{2}}}_\text{only dependent on $t$} &= \underbrace{\frac{1}{X} \frac{d^{2}X}{dx^{2}}}_\text{only dependent on $x$}
\end{align*}
$$
