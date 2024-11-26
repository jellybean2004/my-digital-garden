---
dg-publish: true
---
![Pasted image 20240117160005.png](/img/user/pics/Pasted%20image%2020240117160005.png)
$$
\sigma = \frac{\Delta Q}{\Delta S}
$$
- **step 1: symmetry**
	- $\vec E$ points vertically away from the sheet
	- $|\vec E|$ is constant for a constant distance, $z$, above or below the sheet
- **step 2: gaussian surface**
	- cylinder with axis in the z-direction, intersecting the sheet
	$$\begin{align*}
	\oiint \vec E \, d\vec S &=  \iint_{top} \vec E \, d\vec S + \iint_{bottom}\vec E \, d\vec S + \iint _{curled} \vec E \, d\vec S \\
	&= \iint E \, dS + \iint E \, dS + 0 \\
	&= 2E \iint dS \\
	&= 2E A
	\end{align*}$$
- **step 3:**
$$
Q_{encl.} = \sigma A
$$
- **step 4:**
$$\begin{align*}
2EA = \frac{\sigma A}{\epsilon_{0}} &\implies E  = \frac{\sigma}{2\epsilon_{0}} \\
\therefore \vec E &= \begin{cases}
	\frac{\sigma}{2\epsilon_{0}} \hat z  & z>0 \\
	-\frac{\sigma}{2\epsilon_{0}}  & z<0
	\end{cases}
\end{align*}$$
