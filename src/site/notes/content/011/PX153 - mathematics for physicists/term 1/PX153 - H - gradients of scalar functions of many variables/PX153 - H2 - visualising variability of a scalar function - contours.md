---
dg-publish: true
---

- **contours** - eg think of height, $z$, as a function of position int he $x,y$ plane, ie: $z(x,y)$
- contour lines mark out lines of constant height, ie: defined by $z(x,y) = k$ , where $k$ is a constant
- we will show that the direction of greatest rate of change is perpendicular to the contour

- consider two contour lines that are close together, ie: $f(x,y) =\kappa_{1}$ , and $f(x,y) =\kappa_{2}$ , where $\kappa_{2} = \kappa_{1} + \delta\kappa$ , and $\delta\kappa$ is small
- consider the rate of change along $A\to B$, where $A \to B$ is perpendicular to the contour, compared to the rate of change along $A \to C$ 
	$\Delta n = AB$ , and $\Delta r = AC$
	$\Delta n = \Delta r \cos\theta$
- for infinitesimally small changes: 
$$\frac{\partial f}{\partial r} =  \frac{\partial f}{\partial n}  \frac{\partial n}{\partial r} = \cos\theta  \frac{\partial f}{\partial n}$$
- the change in $f$, $\Delta f$, between $A$ and $B$ is the same as between $A$ and $C$. so, the rate is determined just by the length
- thus, the directional derivative, given by $\vec\nabla f =  \frac{\partial f}{\partial n} \hat n$ , gives the highest change of $f$ and is always perpendicular to the contour of constant $f$. this gives a geometrical definition of $\vec \nabla f$
- we would show shortly that this is equivalent to our previous definition: 
$$\vec \nabla f = \left( \hat{i} \frac{\partial}{\partial x} + \hat{j} \frac{\partial }{\partial y} \right) f$$

- eg: for $f(x,y)$, find $\vec\nabla f$, evaluate the gradient at $(\frac{1}{2} , \frac{1}{2})$ , and hence find the direction of the fastest change in $f$ at that point
	- for gradient: 
	$$\vec \nabla f = \left( \hat{i} \frac{\partial}{\partial x} + \hat{j} \frac{\partial }{\partial y} \right) f = \hat{\vec i} - \hat{\vec j}$$
	- at all points, gradient is $(1,-1)$, magnitude $\sqrt 2$, and direction $\frac{1}{\sqrt{2}} (1,-1)$
	- the contour lines are: 
	$$f(x,y) = \kappa = x-y \implies y = x- \kappa$$
	![Pasted image 20231127145005.png](/img/user/pics/Pasted%20image%2020231127145005.png)

- eg: at $(1,2)$ find the direction along which $f(x,y) = x^{2}y + xy$ changes most rapidly
	- taking the directional derivative: 
	$$\vec \nabla f = (2xy+y)\hat{\vec i} + (x^{2}+x)\hat{\vec j}$$
	- at $(1,2)$: $\vec\nabla f(1,2) = 6\hat{\vec i} + 2 \hat{\vec j}$
	- the direction is given by 
	$$\hat{\vec u} = \frac{\vec\nabla f}{|\vec\nabla f|} = \frac{3}{\sqrt{10}}\hat{\vec i} + \frac{1}{\sqrt{10}}\hat{\vec j}$$
- we now show that $\vec\nabla f = ( \frac{\partial }{\partial x}\hat{\vec i} + r \hat{\vec j}  \frac{\partial }{\partial y})f$ is perpendicular to the tangent of the contour line of $f$, consistent with our geometrical definition
- let $f(x,y)=\kappa$ define a contour, which is parameterized by $q$, ie: all points on this contour are given by $\vec r(q) = [x(q),y(q)]$
- varying $q$ takes us aroufd this contour, on which the function assumes an arbitrary constant value $\kappa$, thus: 
$$\frac{df}{dq}=0$$
	- this derivative can be rewritten as:  
	$$df =  \frac{\partial f}{\partial x} dx + \frac{\partial f}{\partial y} dy \implies \frac{df}{dq} =  \frac{\partial f}{\partial x} \frac{dx}{dq} + \frac{\partial f}{\partial y} \frac{dy}{dq}$$
	- can write this as a scalar product: 
	$$\frac{df}{dq}=  (\frac{\partial f}{\partial x},\frac{\partial f}{\partial y})\cdot ( \frac{dx}{dq}, \frac{dy}{dq})$$
- the vector $\vec t = ( \frac{dx}{dq}, \frac{dy}{dq})= \frac{d}{dq}\vec r$ is the direction of the tangent to the contour: 
$$\frac{df}{dq} = \vec\nabla f\cdot t = 0$$
$$\therefore\vec\nabla f \perp \vec t$$

- eg: what are the shapes of the contour lines of the function, $f(x,y) = e^{-(x^{2}+y^{2})}$? find the general expression for the gradient
	- contour lines are defined by $f(x,y)=\kappa = e^{-(x^{2}+y^{2})}$
		$\implies x^{2}+y^{2}= \ln(\frac{1}{\kappa})$
		- ie: circles of radius $\sqrt{\ln{\frac{1}{\kappa}}}$ centred on the origin
	- the gradient is given by: 
	$$\vec\nabla f = (-2xe^{-(x^{2}+y^{2})})\hat{\vec i} + (-2ye^{-(x^{2}+y^{2})})\hat{\vec j}$$
		- in circular polar coordinates, this is 
		$$\vec\nabla f = -2e^{-r^{2}}\vec r$$