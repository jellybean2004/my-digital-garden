---
dg-publish: true
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
		$x_{cm} = \frac{\int x.dm}{\int dm} \implies \int x.dm = x_{cm}\int dm = d.m$
$$I_{A}= I_{cm}(||)+md^{2}$$