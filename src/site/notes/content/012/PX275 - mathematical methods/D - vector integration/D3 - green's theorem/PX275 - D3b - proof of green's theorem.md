---
{"dg-publish":true,"permalink":"/content/012/px-275-mathematical-methods/d-vector-integration/d3-green-s-theorem/px-275-d3b-proof-of-green-s-theorem/","noteIcon":"1","created":"2024-11-25T10:50:32.000+00:00","updated":"2024-11-26T10:05:44.009+00:00"}
---

- **this is non examinable**
- considering a rectangle with vertices $(x_{1}, y_{1})$, $(x_{2},y_{1})$, $(x_{2},y_{2})$, $(x_{1,}y_{2})$
- taking a term from the theorem: 
$$\begin{align*}
	-\iint \frac{\partial P}{\partial y} \,dy\,dx &= - \int_{x_{1}}^{x_{2}} \int_{y_{1}}^{y_{2}}  \frac{\partial P}{\partial y}\,dy\,dx \\
	&= - \int_{x_{1}}^{x_{2}} \big[ P(x,y_{2}) - P(x,y_{1}) \big] \,dx \\
	&= \int_{x_{1}}^{x_{2}} P(x,y_{1})\,dx + \int_{x_{2}}^{x_{1}} P(x,y_{2})\,dx \\
\end{align*}$$
	- this gives the integrals of the top and the bottom sections
- similarly: 
$$\iint \frac{\partial Q}{\partial x} = \int_{y_{1}}^{y_{2}} Q(x_{2},y)\,dy + \int_{y_{2}}^{y_{1}} Q(x_{1},y)\,dy $$
	- this gives the integrals of the sides
- combining the terms give the integral around the perimeter of the rectangle

- for a field $\vec F$ in the $x-y$ plane: 
$$\vec\nabla \times \vec F = \left(\frac{\partial F_y}{\partial x} + \frac{\partial F_x}{\partial y}\right) \hat k$$
$$\iint \vec\nabla \times \vec F \cdot d\vec A = \oint \vec F \cdot d\vec r$$
- eg: 
$$\vec\nabla\times \vec E = - \frac{\partial B}{\partial t}$$
$$\iint \vec\nabla\times \vec E \cdot d\vec A = \oint_{loop} \vec E \cdot d\vec l - \int \frac{\partial B}{\partial t}\cdot d\vec A$$
