---
{"dg-publish":true,"permalink":"/content/011/px-155-classical-mechanics-and-special-relativity/classical-mechanics/px-155-e-circular-motion-rotation-of-bodies/px-155-e14-parallel-axis-theorem/","created":"2024-10-01T18:27:09.693+01:00","updated":"2024-11-26T19:57:20.067+00:00"}
---

- moment of inertia of an object of mass $m$ around an axis that lies at a perpendicular distance $d$ from the object's centre of mass equals the moment of inertia around a parallel axis through the centre of mass plus $md^{2}$:
$$I(any \; axis) = I_{cm}(||)+md^{2}$$
- avoids needing to recompute $I$
- eg: $I_{cm}$ for a long thin rod mass, $m$, length about an axis through the centre perpendicular to rod:
$$I_{cm}= \frac{1}{12}mL^{2}$$
	- what is $I$ for rotation about a parallel through one end? 
		- here,  $d=\frac{L}{2}$:
$$I = \frac{1}{12}mL^{2} + \frac{1}{4}mL^{2}= \frac{1}{3}mL^{2}$$
  ## justification of the theorem
![Pasted image 20231112151347.png](/img/user/pics/Pasted%20image%2020231112151347.png)
$$I_{A}= \int (r')^{2}.dm$$
- cosine rule:
$$(r')^{2}=r^{2} + d^{2} - 2dr\cos\theta$$
$$I_{A}= \int r^{2}.dm + d^{2}\int dm - 2d\int x.dm$$
\1\n\2\n