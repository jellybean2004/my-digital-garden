---
{"dg-publish":true,"permalink":"/content/011/px-153-mathematics-for-physicists/term-1/px-153-h-gradients-of-scalar-functions-of-many-variables/px-153-h6-gradient-operator/","created":"2024-11-25T10:50:32.000+00:00","updated":"2024-11-26T19:37:56.097+00:00"}
---

- from [[content/011/PX153 - mathematics for physicists/term 1/PX153 - H - gradients of scalar functions of many variables/PX153 - H3 - gradients of functions of three variables\|PX153 - H3 - gradients of functions of three variables]]:  
$$\vec\nabla f =\left( \hat{\vec e}_{x} \frac{\partial }{\partial x} + \hat{\vec e}_{y} \frac{\partial }{\partial y} \right)f$$
- we have, 
$$\hat{\vec e}_{x} = \cos\theta \;\hat{\vec e}_{r} - \sin\theta\; \hat{\vec e}_{\theta} \; , \; \hat{\vec e}_{y} = \sin\theta \;\hat{\vec e}_{r} + \cos\theta\; \hat{\vec e}_{\theta} $$
- to find: $\hat{\vec e}_{x}  \frac{\partial f}{\partial r}$ in terms of $r, \theta$:
	- using chain rule: 
	$$\frac{\partial f}{\partial x} =  \frac{\partial f}{\partial r}  \frac{\partial r}{\partial x} +  \frac{\partial f}{\partial \theta}  \frac{\partial \theta}{\partial x}$$
	- from $r = \sqrt{x^{2}+y^{2}}$ : 
	$$ \frac{\partial r}{\partial x} = \frac{2x}{2\sqrt{x^{2}+y^{2}}}= \frac{r\cos\theta}{r} = \cos\theta$$
	- from $\theta = \arctan(\frac{y}{x})$ : 
	$$\frac{\partial \theta}{\partial x} = \frac{1}{1+ (\frac{y}{x})^{2}} \cdot \frac{-y}{x^{2}}= \frac{-r\sin\theta}{r^{2}} = - \frac{\sin\theta}{r}$$
	- we get: 
	$$\hat{\vec e}_{x} \ \frac{\partial f}{\partial y} = (\cos\theta \; \hat{\vec e}_{r} - \sin\theta\; \hat{\vec e}_{\theta}) (\cos\theta  \frac{\partial f}{\partial r} + \frac{\sin\theta}{r}\ \frac{\partial f}{\partial \theta})$$
- similarly, wrt $y$: 
$$\frac{\partial r}{\partial y} = \sin\theta \;, and \; \frac{\partial \theta}{\partial y} = \frac{\cos\theta}{r}$$
	- we get: 
	$$\hat{\vec e}_{y} \ \frac{\partial f}{\partial y} = (\sin\theta \; \hat{\vec e}_{r} + \cos\theta\; \hat{\vec e}_{\theta}) (\sin\theta  \frac{\partial f}{\partial r} + \frac{\cos\theta}{r}\ \frac{\partial f}{\partial \theta})$$
- combine and simplify to get: 
$$\vec\nabla f(r,\theta) = \left( \hat{\vec e}_{r}  \frac{\partial }{\partial r} + \hat{\vec e}_{\theta} \frac{1}{r} \frac{\partial }{\partial \theta} \right)f$$

- eg: for $U(r) = \frac{q_{1}q_{2}}{4\pi\epsilon_{0}r}$
\1\n\2\n