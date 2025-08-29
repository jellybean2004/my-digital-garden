---
{"dg-publish":true,"permalink":"/content/012/px-275-mathematical-methods/term-2/h-fourier-series-and-transforms/px-275-h9-ft-and-differential-equations/","noteIcon":"1","created":"2025-08-27T13:15:23.812+01:00","updated":"2025-02-13T12:23:40.000+00:00"}
---

-  considering a function, $f(x)$, and its (partial) derivatives
- the fourier transform:
$$\begin{align*}
\mathcal F \left(\frac{df}{dx}\right) &= \int_{-\infty}^{\infty} e^{-ikx} \frac{df}{dx} \, dx \\
&= [ e^{-ikx} f(x)]_{-\infty}^{+\infty} + ik \int_{-\infty}^{\infty}  e^{-ikx} f(x)\, dx 
\end{align*}$$
- **note:** $f(x)$ needs to be well-behaved and integrable so that $\mathcal F(f(x))$ can sensibly be considered
- if $\lim_{x\to\pm\infty} f(x) = 0$, so the first term is zero
$$\mathcal F\left(\frac{df}{dx}\right) = ik \int_{-\infty}^{\infty}  e^{-ikx} f(x)\, dx  = ik \tilde f(k)$$

- similarly, for the second derivative:
$$\begin{align*}
\mathcal F \left(\frac{d^{2}f}{dx^{2} }\right) &= \int_{-\infty}^{\infty} e^{-ikx} \frac{d^{2}f}{dx^{2}} \, dx \\
&= \underbrace{\left[ e^{-ikx} \frac{df}{dx}\right]_{-\infty}^{+\infty}}_{0} + \underbrace{ik \int_{-\infty}^{\infty}  e^{-ikx} \frac{df}{dx}\, dx }_{ik\,\mathcal F(f'(x))= ik(ik\tilde f(k))}  \\
&= -k^{2} \tilde f(k)
\end{align*}$$

>[!info] general formula for the FT of the $n^{th}$ derivative
$$\mathcal F\left(\frac{d^{n}f}{dx^{n}}\right) = (ik)^{n} \tilde f(k)$$

- this proves to be a power tool for handling differential equations
- the derivatives of a function can be converted into the FT of the function
- the original PDE can be turned into an algebraic expression involving $\tilde f(k)$, which tends to be easier to solve
- the solution for $\tilde f(k)$ can be transformed back into $f(x)$

## example
- considering a differential equation:
$$\frac{d^{2}f}{dx^{2}} + \alpha \frac{df}{dx} + \beta f(x) = g(x)$$
- taking the FT of both sides:
$$\begin{gather}
-k^{2} \tilde f(k) + \alpha ik \tilde f(k) + \beta \tilde f(k) = \tilde g(k) \\
(-k^{2} + \alpha ik \ + \beta) \tilde f(k) = \tilde g(k)
\end{gather}$$
- the second order ODE has been turned into an algebraic expression for $\tilde f(k)$, and:
$$f(x) = \mathcal F^{-1} (\tilde f(k))$$
