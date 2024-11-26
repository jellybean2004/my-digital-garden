---
{"dg-publish":true,"permalink":"/content/011/px-157-electricity-and-magnetism/px-157-c-magnetic-fields/px-157-c4c-magnetic-field-on-a-long-cylindrical-conductor/","created":"2024-10-01T18:27:10.202+01:00","updated":"2024-11-26T20:09:53.574+00:00"}
---

![Pasted image 20240219183417.png](/img/user/pics/Pasted%20image%2020240219183417.png)
- assuming current is uniform in the wire, the current density, $J = \frac{I}{\pi a^{2}} = constant$
- **step 1: symmetry**
	- $\vec B = B_{\phi}(R)\,\hat\phi$
- **step 2: path**
$$
\oint_{C} \vec B\cdot d\vec l = 2\pi R\, B_{\phi}
$$
- **step 3: enclosed current**
	- if $R>a: I_{encl.}= I$
	- if $R<a: I_{encl.} = J\pi R^{2} = I\left(\frac{R}{a}\right)^{2}$
- **step 4: summarize**
	$$\vec B = \begin{cases}
\frac{\mu_{0}I}{2\pi R}\hat\phi\;, & R\geq a \\
\frac{\mu_{0}I}{2\pi R} \left(\frac{R}{a}\right)^{2} \hat\phi = \frac{\mu_{0}I}{2\pi a^{2}} \hat\phi\;, & R<a 
\end{cases}$$
![Pasted image 20240219183444.png](/img/user/pics/Pasted%20image%2020240219183444.png)
