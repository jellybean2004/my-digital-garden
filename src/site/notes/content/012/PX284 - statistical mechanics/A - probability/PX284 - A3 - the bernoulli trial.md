---
{"dg-publish":true,"permalink":"/content/012/px-284-statistical-mechanics/a-probability/px-284-a3-the-bernoulli-trial/","noteIcon":"1","created":"2024-11-25T10:50:32.000+00:00","updated":"2024-11-26T13:01:17.253+00:00"}
---

- an *independent* experiment with two outcomes with the probabilities: 
$$P_{i}(x) = \begin{cases} p & x_{i}=1 & '\text{success}' \\ 1-p & x_{i}=0 & '\text{failure}' \end{cases}$$
- eg: tossing a coin
- the mean is given by: 
$$\langle{x}\rangle = \sum\limits x_{i}P_{i} = 1\times p + 0 \times (1-p) = p$$
 - the mean of $x^{2}:$ 
 $$\langle{x^{2}}\rangle = \sum\limits x_{i}^{2} P_{i} = 1^{2}\times p + 0^{2}\times(1-p)=  p$$
- the standard deviation: 
$$\sigma_{x} = \sqrt {\langle{x^{2}}\rangle - \langle{x}\rangle^{2}} = \sqrt{p - p^{2}} = \sqrt{p(1-p)}$$
- if the same experiment is performed $n$ times, the probability of getting $k$ successes and $n-k$ failures is given by the **binomial distribution**: 
$$P(n,k) =  {}^{n}C_{k} \,p^{k}(1-p)^{n-k}$$
	where, $^{n}C_{k} = {n \choose k} =  \frac{n!}{k!(n-k)!}$ 
- the expected value and the standard deviation are: 
$$\begin{gather*}
	\langle{k}\rangle = np \\
	\sigma_{k} = \sqrt{np(1-p)}
\end{gather*}$$
- the **fractional width** is given by: 
$$\frac{\sigma_{k}}{\langle{k}\rangle} = \sqrt{\frac{1-p}{np}}$$
- the fractional width $\to 0 \;\text{as } n\to\infty$

![Pasted image 20241107154115.png](/img/user/pics/Pasted%20image%2020241107154115.png)
### stirling's formula
- it is an approximation that allows factorial calculations in the limit of large ${} n:$
$$\ln n! \approx n\ln n - n$$
