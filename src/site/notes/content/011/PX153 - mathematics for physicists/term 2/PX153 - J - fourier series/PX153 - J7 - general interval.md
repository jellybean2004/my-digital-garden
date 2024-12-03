---
{"dg-publish":true,"permalink":"/content/011/px-153-mathematics-for-physicists/term-2/px-153-j-fourier-series/px-153-j7-general-interval/","created":"2024-11-25T10:50:32.000+00:00","updated":"2024-12-03T17:15:38.893+00:00"}
---

- a [[content/011/PX153 - mathematics for physicists/term 2/PX153 - J - fourier series/PX153 - J1 - introduction\|fourier series]] is given by: 
$$f(x) = \frac{a_{0}}{2} + \sum\limits_{n=1}^{\infty}\left(a_{n}\cos\left(\frac{n\pi x}{L}\right) +b_{n}\sin\left(\frac{n\pi x}{L}\right) \right)$$ for $x \in [L,L)$
- from [[content/011/PX153 - mathematics for physicists/term 2/PX153 - J - fourier series/PX153 - J3 - proofs and derivations\|proofs and derivations]]: 
$$\begin{align*}
	a_{n} &= \frac{1}{L} \int_{-L}^{L} f(x) \cos\left(\frac{n\pi x}{L}\right)\,dx \\
	b_{n} &= \frac{1}{L}\int_{-L}^{L} f(x) \sin\left(\frac{n\pi x}{L}\right)\,dx \\
	a_{0} &= \frac{1}{L}\int_{-L}^{L} f(x)\,dx
\end{align*}$$

- for $a_{n}:$ 
$$\int_{-L}^{L} f(x)\cos \left[\frac{m\pi x}{L}\right] \,dx$$
![Pasted image 20240205140754.png](/img/user/pics/Pasted%20image%2020240205140754.png)
