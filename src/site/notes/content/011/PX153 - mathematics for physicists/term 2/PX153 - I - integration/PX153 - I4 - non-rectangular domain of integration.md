---
dg-publish: true
---

- so far, the integration domain has been rectangular, but if the integration region isn't rectangular, then the following approach must be taken
![Pasted image 20240110184011.png](/img/user/pics/Pasted%20image%2020240110184011.png)
- domain, $R$, is given by $y_{1}(x) \leq y \leq y_{2}(x)$ for all $a \leq x \leq b$
- the function is integrated over $y$ from $y_{1}(x)$ to $y_{2(x)}$ , and then integrated over $x$ from $a$ to $b$
- can alternatively be thought as: 
![Pasted image 20240110184039.png](/img/user/pics/Pasted%20image%2020240110184039.png)
- the function is first integrated over $x$ from $x_{1}(y)$ to $x_{2}(y)$, and then over $y$ from $c$ to $d$
- first way: 
$$I = \iint_{R}f(x,y).dx.dy = \int_{a}^{b}\left( \int_{y_{1}(x)}^{y_{2}(x)} f(x,y).dy \right).dx$$
- eg: $y_{1}=x$ , $y_{2}=\sqrt{x}$ , and $f=xy^{2}$. evaluate: 
$$I= \int_{0}^{1}\left( \int_{y_{1}=x}^{y_{2}=\sqrt{x}} xy^{2}.dy \right).dx$$
	![Pasted image 20240110184057.png](/img/user/pics/Pasted%20image%2020240110184057.png)
	$$I = \int_{0}^{1} \left[ \frac{xy^{3}}{3} \right]_{x}^{\sqrt{x}.dx}= \int_{0}^{1}(\frac{x^{\frac{5}{2}}}{3}- \frac{x^{4}}{3}).dx =...=\frac{1}{35}$$
	- change the order of integration? 
	$$I= \int_{0}^{1}\left( \int_{x_{1}}^{x_{2}} xy^{2}.dx \right).dy = ... = \frac{1}{35}$$
- eg: find $I = \iint_{R} (x+y)^{2}.dx.dy$ , where $R$ is the domain of integration where the area is enclosed by triangle: $(0,-1)$, $(1,1)$, $(-1,1)$
	- first, integrate over $x$ : 
$$\begin{align}
	I &= \int \left(\int_{x_{1} - \frac{y+1}{2}}^{x_{2}=\frac{y+1}{2}} (x+y)^{2}.dx \right).dy \\
	& = \int_{-1}^{1} \left( \frac{(\frac{3y}{2}+ \frac{1}{2})^{3}}{3} - \frac{(\frac{y}{2}- \frac{1}{2})^{3}}{3}\right).dy \\
	&= 1
\end{align}$$
	- can be verified by swapping the order of integration: 
	![Pasted image 20240118155029.png](/img/user/pics/Pasted%20image%2020240118155029.png)
	$$I = \int_{-1}^{0} \left( \int_{y_{1}=-2x-1}^{1} (x+y)^{2}.dy \right).dx + \int_{0}^{1} \left( \int_{y_{1}=2x-1}^{1} (x+y)^{2}.dy \right).dx$$
		- the result must be $1$

- eg: what is the volume of a sphere of radius, $a$?
	- every point at the surface of a sphere: $x^{2} + y^{2} +z^{2} = a^{2}$
	- $f(x,y)= z = \pm\sqrt{a^{2}-x^{2}-y^{2}}$
	![Pasted image 20240118155055.png](/img/user/pics/Pasted%20image%2020240118155055.png)
	$$V = 8 \int_{0}^{a} \int_{0}^{\sqrt{a^{2}-x^{2}}} \sqrt{a^{2}-x^{2}-y^{2}}.dy.dx$$
	- let, $y=A\sin t$ ,  $A=\sqrt{a^{2}-x^{2}}$ , $dy = A\cos t \, dt$ , $y=\sqrt{a^{2}-x^{2}} \implies t = \frac{\pi}{2}$
$$\begin{align}
	V &= 8 \int_{0}^{a} \int_{0}^{\frac{\pi}{2}} \sqrt{A^{2}-A^{2}\sin^{2}t} A\cos t.dt.dx\\
	&= 8 \int_{0}^{a} \int_{0}^{\frac{\pi}{2}} A^{2}\cos^{2} t.dt.dx\\
	&= 8 \int_{0}^{a} \int_{0}^{\frac{\pi}{2}} \frac{A^{2}}{2}(\cos 2t+1).dt.dx\\
	&= 8 \int_{0}^{a} \frac{A^{2}}{2} [\frac{1}{2}\sin 2t + t]_{0}^{\frac{\pi}{2}}.dx\\
	&= 8 \int_{0}^{a} \frac{A^{2}}{2} \frac{\pi}{2}.dx\\
	&= 2\pi \int_{0}^{a} (a^{2} -x^{2}).dx \\
	\therefore V&= \frac{4\pi}{3}a^{3}
\end{align}$$
	