---
dg-publish: true
---
- eg: a spherical conductor with charge, $Q$
	- outside the sphere: 
	![Pasted image 20240125101101.png](/img/user/pics/Pasted%20image%2020240125101101.png)
	$$\oiint \vec E\,d\vec S = \frac{Q_{encl.}}{\epsilon_{0}} \implies \vec E = \frac{Q}{4\pi\epsilon_{0}r^{2}}\hat r$$
	- inside the sphere: 
	![Pasted image 20240125101028.png](/img/user/pics/Pasted%20image%2020240125101028.png)
	$$\vec E = \vec 0$$
	- surface charge density, $\sigma= \frac{Q}{4\pi a^{2}}$, outside:
$$ \vec E = \frac{\sigma}{\epsilon_{0}}\left(\frac{a}{r}\right)^{2}\hat r
$$
	![Pasted image 20240125101202.png](/img/user/pics/Pasted%20image%2020240125101202.png)
![Pasted image 20240125101214.png](/img/user/pics/Pasted%20image%2020240125101214.png)

- eg: a conducting infinite plane with a finite width
	![Pasted image 20240125101239.png](/img/user/pics/Pasted%20image%2020240125101239.png)
	- the excess charges will be on the top and the bottom planes, each with a charge density, $\frac{\sigma}{2}$
	- the gaussian surface is a cylinder that dissects one face of the plane:
$$
\oiint \vec E\,d\vec S = \iint_{top} \vec E\,d\vec S + \iint_{bottom} \vec E\,d\vec S + \iint_{curved} \vec E\,d\vec S
$$
		- $\iint_{curved} \vec E\,d\vec S = 0$ as $\vec E \parallel d\vec S$
		- $\iint_{bottom} \vec E\,d\vec S = 0$ as it is inside the conductor
	$$\oiint \vec E\,d\vec S = \iint E \hat z \cdot \hat z \, dS  = E\iint dS = EA$$
	- for enclosed charge, $Q_{encl.}=\frac{\sigma}{2}A$:
$$
E = \frac{\sigma}{2\epsilon_{0}}
$$
	$$\vec E = \begin{cases}
		  & \frac{\sigma}{2\epsilon_{0}}\hat z & above\;conductor \\
		  & \vec 0 & inside\;conductor \\
		  & -\frac{\sigma}{2\epsilon_{0}}\hat z & below\;conductor
	 \end{cases}$$
