---
{"dg-publish":true,"permalink":"/content/012/px-275-mathematical-methods/term-2/h-fourier-series-and-transforms/px-275-h2-calculating-coefficients/","noteIcon":"1","created":"2025-01-29T13:40:23.624+00:00","updated":"2025-01-29T13:56:48.953+00:00"}
---

- orthogonality relation:
$$\frac{1}{L} \int_{-L/2}^{L/2}\exp(\pm2\pi i (n-m)x/L)\,dx =\delta_{nm}$$
- multiplying the complex fourier series by $\exp(-i2\pi mx/L)$ and integrating:
$$\begin{align}
\int_{-L/2}^{L/2}f(x)\exp(-i2\pi mx/L)\,dx&=\int_{-L/2}^{L/2}\sum\limits_{n=-\infty}^{\infty}C_{n} \exp(-i2\pi (n-m)x/L)\,dx\\\\
&= LC_m
\end{align}$$
$$\therefore C_{m} = \frac{1}{L} \int_{-L/2}^{L/2}f(x)\exp(-2i\pi m/L)\,dx$$

- this can be used as two-directional transformation:
	- **forward:** coefficients from a function
	- **backward:** function from coefficients
