---
{"dg-publish":true,"permalink":"/content/013/c-error-statistics/c2-reduced-chi-squared/","noteIcon":"1","created":"2025-08-21T10:21:20.269+01:00","updated":"2025-08-21T10:34:43.398+01:00"}
---

- models are fitted by minimising the $\chi^{2}$ statistic
$$\begin{align*} 
\chi^{2} &= \sum\limits_{i} \frac{(y_{i} - y)^{2}}{\alpha_{i}^{2}} \\
\chi^{2} &= \sum\limits_{i} \frac{(O_{i} - E_{i})^{2}}{\alpha_{i}^{2}} 
\end{align*}$$
- the **null hypothesis** being tested is that the obtained sample distribution can be described by a particular parent distribution
- ie: the data, $(x_{i}, y_{i})$, are well modelled by a particular function, $y(x_{i})$

- the two-thirds rule implies that a good fit will have 2/3 of the data points within 1 error bar
- $95\%$ should be between 2 error bars

| $\pm\sigma$ | $\pm 2 \sigma$ | $\pm  3 \sigma$ |
| ----------- | -------------- | --------------- |
| $68\%$      | $95\%$         | $99.7\%$        |

- furthermore, the normalised residuals should have a mean of $0$ and a standard deviation of $1$

- the degrees of freedom, $\nu$, is the number of unconstrained parameters:
$$\nu = N - \mathscr{N}$$
	where $N$ and $\mathscr{N}$ are the numbers of data points and fit parameters, respectively

- eg: when trying to fit 10 data points:
	- in a straight line ($y = mx + c$) : $\nu = 8$
	- in a parabola ($y = ax^{2}+ bx + c$) : $\nu = 7$

- so, the more datapoints are unconstrained, the more robust an estimation is

- **reduced chi-squared** statistic:
$$\chi^{2}_{\nu} = \frac{\chi^{2}_{min}}{\nu} $$
- for a good fit, $\chi^{2}_{min} \simeq \nu$, so $\chi^{2}_{\nu} \simeq 1$

