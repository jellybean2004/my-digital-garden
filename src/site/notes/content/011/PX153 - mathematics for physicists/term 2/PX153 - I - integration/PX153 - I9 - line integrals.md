---
{"dg-publish":true,"permalink":"/content/011/px-153-mathematics-for-physicists/term-2/px-153-i-integration/px-153-i9-line-integrals/","noteIcon":"1","created":"2024-11-25T10:50:32.000+00:00","updated":"2024-11-26T19:38:16.085+00:00"}
---

- split curve $C$ in $n$ sections, each with displacement vector: 
$$\Delta\vec l_{r} = \Delta l_{r,x} \,\hat i + \Delta l_{r,y} \,\hat j - \Delta l_{r,z}\,\hat k$$
$$\lim_{n\to\infty} \sum\limits_{r=1}^{n} F_{x}(\bar x_{r} , \bar y_{r} , \bar z_{r})\Delta l_{r,x} + F_{y}(\bar x_{r} , \bar y_{r} , \bar z_{r})\Delta l_{r,y} + F_{z}(\bar x_{r} , \bar y_{r} , \bar z_{r})\Delta l_{r,z}$$
$$= \int_{C} \vec F(\vec r) \cdot d\vec l$$
- [guide](https://tutorial.math.lamar.edu/classes/calciii/lineintegralsintro.aspx)

- eg: the integral could be the work down, $W$, when moving a particle along a path, $C$, when subjected to a force, $\vec F$, that may be position dependent along path $C:$ 
$$W = \int_{C}\vec F \cdot d\vec l$$
- eg: $I = \int_{C}\vec P \cdot d\vec l$ , where, $\vec P = 5y^{2}\hat i + 2xy \hat j$, along $C_{1}:$ a straight line joining the origin and $(1,1)$
	- parameterizing the path: 
	$$\vec l = x \vec i + y \hat j$$ with $C_{1}: y=x$
	- can be simplified by using $x$ as the integration variable: $y=x \implies dy = dx$ along $C_{1}$, and $x$ goes from $0\to1$
	$$d \vec l = \frac{d}{dx}(x,y) = (1,1)dx = (\hat i + \hat j)dx$$
$$\begin{align*}
	\int_{C} \vec P \cdot d\vec l &= \int_{x=0}^{x=1} (5y^{2}\hat i + 2xy\hat j)\cdot (dx \hat i + dx \hat j)\\
	&= \int_{0}^{1} 7x^{2} \, dx \\
	&= \frac{7}{3}
\end{align*}$$

- eg: $I = \int_{C_{2}} \vec P \cdot d\vec l$ , where $C_{2}:$ two straight lines, one with $x$ from $0\to1$, other with $y$ from $0\to1$
$$\begin{align*}
	I &= \int_{x=0,y=0}^{x=1} (5y^{2}\hat i + 2xy\hat j)\cdot (dx \hat i + dy \hat j) + \int_{y=0,x=1}^{y=1} (5y^{2}\hat i + 2xy\hat j)\cdot (dx \hat i + dy \hat j) \\
	&= \int_{0}^{1} 0 \, dx + \int_{0}^{1}2y \, dy \\
	&= 1
\end{align*}$$
- this shows that the result depends on the path taken
