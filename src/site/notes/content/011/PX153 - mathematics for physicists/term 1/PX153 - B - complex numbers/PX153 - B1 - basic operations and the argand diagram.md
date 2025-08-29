---
{"dg-publish":true,"permalink":"/content/011/px-153-mathematics-for-physicists/term-1/px-153-b-complex-numbers/px-153-b1-basic-operations-and-the-argand-diagram/","noteIcon":"1","created":"2025-08-27T13:14:08.640+01:00","updated":"2024-11-26T19:36:29.000+00:00"}
---

## complex numbers
- a complex number can be written in the form $z=x+iy$
		$Re(z)=x$
		$Im(z)=y$
			 $x,y \in \mathbb{R}$
			 $i^2=-1$
	- the set of real numbers $\mathbb Re$ is a subset of the set of complex numbers $\mathbb{C}$
	- the modulus $|z|=\sqrt{x^2+y^2}$
	- the argument $arg(z)=\theta=\arctan{ \frac{y}{x}}$
	- we use the convention $0\leq\theta< 2\pi$ ; $arg(z)\in[0,2\pi)$
## argand diagram
![Pasted image 20231016140614.png](/img/user/pics/Pasted%20image%2020231016140614.png)
## complex conjugate
- $z^*=x-iy$
- $|{z}|=\sqrt{z.z^*}$
## standard operations
- $z_1=x_1+iy_1$
- $z_2=x_2+iy_2$
### addition and subtraction
$$z_1\pm z_2=(x_1\pm iy_1)+(x_2\pm iy_2)$$
### multiplication
$$z_1z_2=(x_1+iy_1)(x_2+iy_2)=(x_1x_2-y_1y_2)+i(x_2y_1+x_1y_2)$$
### division
$$\frac{1}{z}=\frac{1}{x+iy}= \frac{x-iy}{(x+iy)(x-iy)}= \frac{x-iy}{x^2+y^2}$$
$$\frac{z_1}{z_{2}}=z_1z_2^{-1}=(x_1+iy_{1}) \frac{(x_2-iy_{2})}{x_2^2+y_{2}^2}= \frac{(x_1x_2-y_1y_2)+i(x_2y_1+x_1y_2)}{x_2^2+y_2^2}$$
$$\frac{z_{1}}{z_{2}} = \frac{z_{1}z_{2}^{*}}{z_{2}z_{2}^{*}}$$
## powers of i
$$i^n=i^r$$
where, $r=$ remainder from division by 4
- note: added during tutorial