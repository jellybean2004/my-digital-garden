---
dg-publish: true
---
 - only for square matrices
- some properties of a matrix can be characterized by a single number
## trace
$$Tr\,A = a_{11}+ a_{22}+\dots+a_{nn} = \sum\limits_{i=1}^{\infty} a_{ii}$$
$$Tr\,(A+B) = Tr\,A + Tr\,B$$
$$Tr(AB) = \sum\limits_{j,i} a_{ij} b_{ji} = \sum\limits_{j,i} b_{ji} a_{ij} = Tr(BA)$$
- eg: 
$$Tr\, \begin{bmatrix}1 & 0 \\0 & -1\end{bmatrix} = 1-1=0$$
## determinant
- let $A$ be a $n\times n$ matrix. the determinant of $A$, written as $|A|$ or $\det A$, is a number defined as: 
$$\det \begin{bmatrix}a_{11} & a_{12} \\ a_{21} & a_{22}\end{bmatrix} = a_{11}a_{22}-a_{12} a_{21}$$
$$\det \begin{bmatrix}a_{11} & a_{12} & a_{13} \\ a_{21} & a_{22} & a_{23} \\ a_{31} & a_{32} & a_{33}\end{bmatrix} =
a_{11}\det\begin{bmatrix}a_{22} & a_{23} \\ a_{32} & a_{33}\end{bmatrix}
-a_{12}\det\begin{bmatrix}a_{21} & a_{23} \\ a_{31} & a_{33}\end{bmatrix}
+ \det\begin{bmatrix}a_{21} & a_{22} \\ a_{31} & a_{32}\end{bmatrix}$$

- eg: 
$$\det \begin{bmatrix}1 & 0 & 2 \\ -1 & 1 & 3 \\ 0 & 2 & 1\end{bmatrix} = 1\times (-5)-0+2\times(-2) = -9$$
### cofactor
- more generally, for a $n\times n$ matrix, $A=(a_{ij})_{n\times n}$, the co-factor, $c_{ij}$, for $a_{ij}$ is defined to be $(-1)^{i+j}\times \det A_{(n-1)\times(n-1)}$ 
- the determinant can be written as: 
$$\det A = a_{11}c_{11}+a_{12}c_{12}+\dots +a_{1n}c_{1n}$$
- in 3D: 
$$\begin{align*}
	\det A &= a_{11}c_{11}+ a_{12}c_{12}+a_{13}c_{13} \\
	&= a_{11}(-1)^{1+1} \det\begin{bmatrix}a_{22} & a_{23} \\ a_{32} & a_{33}\end{bmatrix} + a_{12}(-1)^{1+2} \det\begin{bmatrix}a_{21} & a_{23} \\ a_{31} & a_{33}\end{bmatrix} + a_{13} \det\begin{bmatrix}a_{21} & a_{22} \\ a_{31} & a_{32}\end{bmatrix}
\end{align*}$$
- if $A$ is a $n\times n$ matrix, then $\det A$ contains of the order of $n!$ products of $n$ matrix elements that are in different rows and columns
### connection between determinant and cross product
[[content/011/PX153 - mathematics for physicists/term 1/PX153 - A - vectors/PX153 - A6 - advanced vector operations#scalar triple product\|PX153 - A6 - advanced vector operations#scalar triple product]]
- consider 3 vectors:
	 $\vec e = (e_{1},e_{2}, e_{3})$
	 ${} \vec f = (f_{1},f_{2}, f_{3}) {}$
	 $\vec g = (g_{1},g_{2}, g_{3})$
- the cross product: 
$$\vec f\times \vec g = (f_{2}g_{3}-g_{2}f_{3}, g_{1}f_{3}-g_{3}f_{1}, f_{1}g_{2}-g_{1}f_{2})$$
$$\begin{align*}
	\vec e\cdot (\vec f\times\vec g) &= (e_{1}(f_{2}g_{3} - g_{2}f_{3}), e_{2}(g_{1}f_{3}-g_{3}f_{1}), e_{3}(f_{1}g_{2}-g_{1}f_{2})) \\
	&= e_{1}c_{11}+e_{2}c_{12}+e_{3}c_{13} \\
	&= \det \begin{bmatrix}e_{1} & e_{2} & e_{3} \\ f_{1} & f_{2} & f_{3} \\ g_{1} & g_{2} & g_{3}\end{bmatrix}
\end{align*}$$
- this gives the volume of the parallelepiped, the base area, $|\vec f\times \vec g|$, times height, $|\vec e|\cos\theta$: 
$$\vec e \cdot (\vec f\cdot \vec g) = |\vec f\times \vec g| |\vec e|\cos\theta
$$
