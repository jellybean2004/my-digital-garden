---
{"dg-publish":true,"permalink":"/content/012/px-275-mathematical-methods/term-2/h-fourier-series-and-transforms/px-275-h7b-examples-of-convolutions/","noteIcon":"1","created":"2025-08-27T13:15:23.797+01:00","updated":"2025-02-12T16:06:22.000+00:00"}
---

## convolution with a $\delta$ function
$$\begin{align*}
f*g(x') &= \int_{-\infty}^{\infty} f(y')\, g(x'-y')\, dy' \\
f*\delta(x-y)&= \int_{-\infty}^{\infty} f(z) \delta(x-y-z) \, dz \\
&= \int_{-\infty}^{\infty} f(z) \delta(z - (x-y)) \, dz \\
&= f(x-y)
\end{align*}$$
- this shows that convolutions with $\delta(x-y)$ shifts the function by $x=y$

$$\begin{align*}
f * \delta(x-y) &= \mathcal F^{-1} (\tilde f(k) \, \tilde g (k)) \\
&= \frac{1}{2\pi} \int_{-\infty}^{\infty} e^{ikx} \tilde f(k) \mathcal(\delta(x-y))\,dk \\
&= \frac{1}{2\pi} \int_{-\infty}^{\infty} e^{ik(x-y)} \tilde f(k) \, dk \\
&= f(x-y) 
\end{align*}$$

## convolve with a set of $\delta$ functions

$$\begin{gather}
g(x) = \sum\limits_{i= 1}^{N }\delta(x - y_{i}) \\
f * g(x) = \sum\limits_{i=1}^{N }f(x - y_{i})
\end{gather}$$
- the convolution is a sum of the function shifted to each $y_{i}$

![PX275 - H7b - examples of convolutions.png|500](/img/user/pics/PX275%20-%20H7b%20-%20examples%20of%20convolutions.png)
## convolution of two gaussians

$$\begin{gather}
f(x) = \sqrt{\frac{1}{2\pi\sigma_{1}^{2}}}\exp(- x^{2}/2\sigma_{1}^{2}) \\
g(x) = \sqrt{\frac{1}{2\pi\sigma_{2}^{2}}}\exp(- x^{2}/2\sigma_{2}^{2}) \\\\

\tilde f(k) = \exp(- k^{2}\sigma_{1}^{2}/2) \\\\

f*g(x) = \int_{-\infty}^{\infty}e^{ikx} \exp (- x^{2}/2\sigma_{1}^{2})  \exp (- x^{2}/2\sigma_{2}^{2}) \\
= \int_{-\infty}^{\infty}e^{ikx} \underbrace{\exp \left(\frac{1}{2}(\sigma_{1}^{2}+\sigma_{2}^{2})k^{2}\right)}_\text{gaussian with varaince added}\,dk \\
= \frac{1}{\sqrt{2\pi (\sigma_{1}^{2}+ \sigma_{2}^{2})}} \exp\left(- \frac{x^{2}}{2(\sigma_{1}^{2}+\sigma_{2}^{2})}\right)
\end{gather}$$
- therefore, gaussian convolutions broadens/smears the function, with the result having combined variance
- this is called **gaussian blurring**
