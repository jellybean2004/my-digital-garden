---
dg-publish: true
---
![Pasted image 20240311183335.png](/img/user/pics/Pasted%20image%2020240311183335.png)
- **step 1:**
$$
\tilde Z_{eq}= R + j\omega L
$$
- **step 2:**
$$
\tilde I = \frac{\tilde V_{in}}{\tilde Z_{eq}} = \frac{\tilde V_{in}}{R+j\omega L}
$$
- **step 3:**
$$
\tilde V_{out} = \tilde Z_{L}\tilde I = j\omega L \frac{\tilde V_{in}}{R+j\omega L}
$$
- **step 4:**
$$
\frac{|\tilde V_{out}|}{|\tilde V_{in}|} = \frac{\omega L}{\sqrt{R^{2}+\omega^{2}L^{2}}}
$$
- **step 5:**
$$
\phi = \arctan\left(\frac{\omega L}{R}\right)
$$
	- ${} \tilde V_{in} {}$ leads $\tilde I$ by $\phi$
![Pasted image 20240311183822.png](/img/user/pics/Pasted%20image%2020240311183822.png)
- typical frequency: $\omega=\frac{R}{L}$
- this circuit acts as a *high-pass filter*
