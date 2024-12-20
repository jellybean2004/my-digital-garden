---
{"dg-publish":true,"permalink":"/content/011/px-157-electricity-and-magnetism/px-157-d-induction/px-157-d1e-a-rotating-conducting-rod-in-a-magnetic-field/","noteIcon":"1","created":"2024-10-01T18:27:10.231+01:00","updated":"2024-11-26T20:10:34.890+00:00"}
---

![Pasted image 20240229165601.png](/img/user/pics/Pasted%20image%2020240229165601.png)
- using cylindrical coordinates, $(R,\phi,z)$
	$\vec B = -B\,\hat z$
	$\vec v = v_{\phi}\,\hat\phi = R\omega\,\hat \phi$
	$\omega$ is constant
- choose path $C$, radially outwards along the rod
$$\begin{align*}
	\vec v\times\vec B \cdot d\vec l &= R\omega\,\hat\phi \times (-B)\,\hat z \cdot dR\,\hat R \\
	&= -RB\omega\,dR
\end{align*}$$
$$\begin{align*}
	\epsilon &= \oint_{C}(\vec v\times\vec B )\cdot d\vec l \\
	&= -B\omega \int_{0}^{L}R\,dR \\
	&= -\frac{1}{2} B\omega L^{2}
\end{align*}$$
- **alternatively**, rod sweeps an area as a function of time:
$$
A(t) = \frac{1}{2}L^{2}\phi(t)
$$
- from [[content/011/PX157 - electricity and magnetism/PX157 - D - induction/PX157 - D1a - faraday's law\|faraday's law]]:
$$\begin{align*}
	\epsilon &= - \frac{d}{dt}(BA) \\
	&= -B \frac{dA}{dt} \\
	&= -\frac{1}{2}B\omega L^{2}
\end{align*}$$
