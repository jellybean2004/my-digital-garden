---
{"dg-publish":true,"permalink":"/content/012/px-284-smeto/part-1-statistical-mechanics/e-single-particle-partition-function/px-284-e1a-internal-energy/","noteIcon":"1","created":"2024-12-23T21:55:45.679+00:00","updated":"2024-12-23T22:04:28.851+00:00"}
---

- the internal energy is the total expected energy:
$$\begin{align*}
	U &=\sum\limits_{i}E_{i}P_{i} \\
	&= \sum\limits_{i} \frac{E_{i}\exp(-\beta E_{i})}{Z} 
\end{align*}$$
- the partition function:
$$Z = \sum\limits_{i}\exp(-\beta E_{i}) \implies \frac{dZ}{d\beta} = -E_{i}  \sum\limits_{i}\exp(-\beta E_{i})$$
$$\boxed{\therefore U = - \frac{d \ln Z}{d\beta}}$$
