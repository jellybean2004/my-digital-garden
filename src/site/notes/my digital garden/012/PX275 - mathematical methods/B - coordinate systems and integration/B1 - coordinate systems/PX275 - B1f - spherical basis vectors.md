---
{"dg-publish":true,"permalink":"/my-digital-garden/012/px-275-mathematical-methods/b-coordinate-systems-and-integration/b1-coordinate-systems/px-275-b1f-spherical-basis-vectors/","created":"2024-11-25T10:50:32.000+00:00","updated":"2024-11-26T10:04:36.485+00:00"}
---

![Pasted image 20241017122458.png](/img/user/pics/Pasted%20image%2020241017122458.png)
$$\vec r = r\sin\theta\cos\phi \, \hat i + r\sin\theta\sin\phi\,\hat j + r\cos\theta\,\hat k$$
$$\begin{align*}
	\frac{d\vec r}{dr}: \hat e_{r} &= \frac{\sin\theta\cos\phi \, \hat i + \sin\theta\sin\phi\,\hat j + \cos\theta\,\hat k}{\sqrt{\sin^{2}\theta\cos^{2}\phi + \sin^{2}\theta\sin^{2}\phi + \cos^{2}\theta}} \\
	&= \frac{\sin\theta\cos\phi \, \hat i + \sin\theta\sin\phi\,\hat j + \cos\theta\,\hat k}{\sqrt{1}}
\end{align*}$$
$$\therefore \hat e_{r}= \sin\theta\cos\phi \, \hat i + \sin\theta\sin\phi\,\hat j + \cos\theta\,\hat k$$
$$\begin{align*}
	\frac{d\vec r}{d\phi}: \hat e_{\phi} &= \frac{-r\sin\theta\sin\phi \, \hat i + r\sin\theta\cos\phi\,\hat j}{\sqrt{r^{2}\sin^{2}\theta\sin^{2}\phi + r^{2}\sin^{2}\theta\cos^{2}\phi}} \\
	&= \frac{-r\sin\theta\sin\phi \, \hat i + r\sin\theta\cos\phi\,\hat j}{r\sin\theta}
\end{align*}$$

$$\therefore \hat e_{\phi}= -\sin\phi \, \hat i + \cos\phi\,\hat j$$
$$\frac{d\vec r}{d\theta}: \hat e_{\theta} = \frac{r\cos\theta\cos\phi \, \hat i + r\cos\theta\sin\phi\,\hat j - r\sin\theta\,\hat k}{\sqrt{r^{2}\cos^{2}\theta\cos^{2}\phi + r^{2}\cos^{2}\theta\sin^{2}\phi - r^{2}\sin^{2}\theta}}$$
$$\therefore \hat e_{\theta} = \cos\theta\cos\phi \, \hat i + \cos\theta\sin\phi\,\hat j - \sin\theta\,\hat k$$
## notation
- for a point: 
$$\vec r = r\,\hat e_r$$
- for a vector field: 
$$\vec F = F_{r}\hat e_{r}+ F_{\phi} \hat e_{\phi} + F_{\theta} \hat e_\theta$$
