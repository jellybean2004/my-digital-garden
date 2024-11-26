---
dg-publish: true
---

$$P(E) \sim \exp(-\beta E)$$
	where, $\beta = \frac{1}{k_{B}T}$
$$P(nhf) = \frac{\exp(-\beta\,nhf)}{\sum\limits_{n}^{\infty} \exp(-\beta\,nhf)}$$
- for $y\to0: (1-y)^{-1}=1+y+y^{2}+y^{3}+\dots:$ 
$$(1-e^{-x})^{-1} = 1+e^{-x}+e^{-2x}+e^{-3x}+\dots = \sum\limits_{n=0}^{\infty}e^{-nx}$$
$$P(nhf) = e^{-\beta\,nhf} (1-e^{-\beta \,hf})$$
$$\langle{E}\rangle = \sum\limits_{n}^{\infty}P(E_{n})E_{n} = \sum\limits_{n=0}^{\infty}nhf\, e^{-\beta\,nhf}(1-e^{-\beta\,hf})$$
$$\begin{align*}
	\sum\limits_{n=0}^{\infty} \frac{d}{d\beta} e^{-\beta nhf} &= \sum\limits_{m=0}^{\infty}-nhf \,e^{-\beta nhf} \\
	&= \frac{d}{d\beta} \frac{1}{1-e^{-\beta hf}} \\
	&= \frac{-e^{-\beta hf}hf}{(1-e^{-\beta hf})^{2}} \\
	&= \frac{-e^{-\beta hf}hf}{(1-e^{-\beta hf})^{2}}
\end{align*}$$
$$\boxed{\langle E \rangle = \frac{hf}{e^{\beta hf}-1}}$$

- high $T$ limit: $k_{B}T>>hf\implies \beta hf <<1:$ 
$$e^{\beta hf} -1 \approx  \beta hf +  \frac{(\beta hf)^{2}}{2}+ \dots \implies \langle E\rangle= \frac{hf}{\beta hf} = k_{B}T$$
- low $T$ limit $k_{B}T << hf \implies \beta hf >> 1 :$ 
$$\langle E\rangle = \frac{hf}{\beta hf} = hf e^{- \frac{hf}{k_{B}T}} \implies small$$
$$I(\lambda) = \frac{2\pi c}{\lambda^{4}} k_{B}T = \frac{2\pi c}{\lambda^{4}} \frac{hf}{e^{\frac{hf}{k_{B}T}}-1} = \frac{2\pi c^{2}h}{\lambda^{5}} \frac{1}{e^{\frac{hf}{k_{B}T}}-1}$$
- taking $T=10^{4}\,K$, $\lambda=5\times10^{-7}\,m$: 
$$\exp\left(\frac{hc}{\lambda k_{B}T}\right) \approx 18$$
- comparable to 
$$I(\lambda,T) = \frac{a\exp\left(\frac{-b}{\lambda T}\right)}{\lambda^{5}}$$
- to find $\lambda_{max}: \frac{dI}{d\lambda}=0$
- to find $I$, integrate $I(\lambda):$ 
$$I = \frac{2\pi^{5}k_{B}^{4}}{15h^{3}c^{2}} T^{4}$$
