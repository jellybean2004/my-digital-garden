---
{"dg-publish":true,"permalink":"/content/012/px-275-mathematical-methods/a-differentiation/2-advanced-a3-a4-and-a5/px-275-a5b-definition-using-gradient/","created":"2024-11-25T10:50:32.000+00:00","updated":"2024-11-26T10:04:14.454+00:00"}
---

$$\boxed{\vec\nabla f + \lambda \vec\nabla g =0}$$
## example
$$\begin{gather}
	f(x,y) = 1+xy \\
	g(x,y) = x^{2} + y^{2} =1 \\\\
	\vec\nabla f = y\,\hat{i}+x\,\hat{j} \\
	\vec\nabla g = 2x\,\hat{i}+ 2y\,\hat{j} \\
\end{gather}$$
- it is known that the maxima of the function with respect to the constraint lies at $x=y=\frac{1}{\sqrt 2}$, and $\lambda = - \frac{1}{2}:$ 
$$\vec\nabla f = \frac{1}{\sqrt 2} (\hat i + \hat j)\,;\, \vec\nabla g= \frac{2}{\sqrt{2}}(\hat i + \hat j)$$
- it can be seen that: 
$$\vec\nabla f = \frac{1}{2}\vec\nabla g$$
- this means that the vectors, $\vec\nabla f$ and $\vec\nabla g$ point in the same direction, but have different magnitudes: 
$$\vec\nabla f - \frac{1}{2}\vec\nabla g = 0$$
- the following condition can be identified: 
$$\vec\nabla f  + \lambda \vec\nabla g = 0$$
