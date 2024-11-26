---
{"dg-publish":true,"permalink":"/content/011/px-153-mathematics-for-physicists/term-1/px-153-h-gradients-of-scalar-functions-of-many-variables/px-153-h3-gradients-of-functions-of-three-variables/","created":"2024-11-25T10:50:32.000+00:00","updated":"2024-11-26T19:37:50.204+00:00"}
---

- $f(x,y,z)= \kappa$ represents contours as planes of constant value
- gradient vector: 
$$\vec \nabla f = \left( \hat{i} \frac{\partial}{\partial x} + \hat{j} \frac{\partial }{\partial y} + \hat{k} \frac{\partial }{\partial z} \right) f$$
	- perpendicular to the planes of constant value
- this gives us a convenient way of finding a vector perpendicular to a surface: 
$$\hat{\vec n} = \frac{\vec\nabla f}{|\vec\nabla f|} = \frac{1}{\sqrt{x^{2}+y^{2}+z^{2}}}(x \hat{\vec i} + y \hat{\vec j} + z \hat{\vec k})$$
- eg: $f(x,y,z) = x^{2}+y^{2}+z^{2}$
	- surfaces of constant value are spheres
	$$f(x,y,z) = \kappa = x^{2}+y^{2}+z^{2}$$ 
	- sphere of radius $\sqrt{\kappa}$ centred on $x=y=z=0$
	$$\vec\nabla f = 2x\hat{\vec i} + 2y\hat{\vec j} + 2z\hat{\vec k} = \vec r$$
	$$\hat {\vec n} =  \frac{\vec r}{|\vec r|}$$
		- in spherical polar coordinates

- eg: find the vector normal to the surface of a torus
![Pasted image 20231128164420.png](/img/user/pics/Pasted%20image%2020231128164420.png)
	$R=$ major radius, $r=$ minor radius
	$\theta =$ toroidal angle ($R$), $\phi =$ poloidal angle ($r$)
	$x= (R + r\cos\phi)\cos\theta$
	$y=(R+r\cos\phi)\sin\theta$
	$z = R\sin\phi$
need to eliminate $\theta, \phi$: 
$$x^{2}+y^{2} = (R+r\cos\phi)^{2} \implies r\cos\phi = \sqrt{x^{2}+y^{2}}-R$$
$$r^{2}\cos^{2}\phi + r^{2}\sin^{2}\phi = r^{2}$$
$$\sqrt{x^{2}+ y^{2}}- R^{2}+z^{2}=r^2$$
$$f(x,y,z) = \sqrt{x^{2}+ y^{2}}- R^{2}+z^{2} - r^{2} =0$$
- describes the surface of the torus i cartesian coordinates

- now, find the normal to vector from $\vec\nabla f$: 
		$$ \frac{\partial f}{\partial x} = 2(\sqrt{x^{2}+ x^{2}}- R^{2}) \frac{x}{\sqrt{x^{2}+y^{2}}}$$
		$$ \frac{\partial f}{\partial x} = 2(\sqrt{x^{2}+ y^{2}}- R^{2}) \frac{y}{\sqrt{x^{2}+y^{2}}}$$
		$$ \frac{\partial f}{\partial z} = 2z$$
		$$\vec\nabla f = 2x \frac{(\sqrt{x^{2}+ x^{2}}- R^{2})}{\sqrt{x^{2}+y^{2}}} \hat{\vec i} + 2y \frac{(\sqrt{x^{2}+ x^{2}}- R^{2})}{\sqrt{x^{2}+y^{2}}} \hat{\vec k} + 2z \hat{\vec k}$$
