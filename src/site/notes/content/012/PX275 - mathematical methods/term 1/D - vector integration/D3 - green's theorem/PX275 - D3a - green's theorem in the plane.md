---
{"dg-publish":true,"permalink":"/content/012/px-275-mathematical-methods/term-1/d-vector-integration/d3-green-s-theorem/px-275-d3a-green-s-theorem-in-the-plane/","noteIcon":"1","created":"2025-08-27T13:14:15.958+01:00","updated":"2024-11-26T10:05:42.000+00:00"}
---

![Pasted image 20241111120746.png](/img/user/pics/Pasted%20image%2020241111120746.png)
- green's theorem relates an integral around a closed loop to an integral over the area of the region enclosed by the loop
- this is a two dimensional theorem, but it underpins the divergence and stokes' theorems
- considering a vector field in 2D: 
$$\vec F = P(x,y) \, \hat i + Q(x,y) \, \hat j$$
	where, $P$ and $Q$ are scalar functions of $(x,y)$
- taking a path from $A$ to $B$ in the $x-y$ plane: 
$$\int_{A}^{B }\vec F \cdot d\vec r = \int_{A}^{B} (P\hat i + Q \hat j) \cdot (dx\,\hat i + dy \,\hat j) = \int_{A}^{B} P\,dx + Q\,dy$$
- considering a closed loop: 
$$\oint_{C}\vec F \cdot d\vec r = \oint_{C}P\,dx + Q\,dy$$
![Pasted image 20241111121528.png](/img/user/pics/Pasted%20image%2020241111121528.png)
- green's theorem relates the integral of a vector field around a loop to the integral of the differentiated components of that field over the area enclosed by the loop: 
$$\oint_{C}\vec F \cdot d\vec r = \oint_{C}P\,dx + Q\,dy = \iint_{R} \left(\frac{\partial Q}{\partial x} - \frac{\partial P}{\partial y}\right) \, dA $$
- for a conservative field, the loop integral will be zero, and hence, so is the $RHS$ of green's theorem: 
$$\frac{\partial Q}{\partial x} - \frac{\partial P}{\partial y} = 0$$
$$\iint_{R} \left(\frac{\partial Q}{\partial x} - \frac{\partial P}{\partial y}\right) = \iint_{R} (\vec\nabla \times \vec F)_{z}\,dA$$
- extending it to three dimensions gives *stokes' theorem*: 
$$\oint_{C}\vec F \cdot d\vec r = \iint_R (\vec\nabla \times \vec F) \cdot d\vec A$$
	where, $dA$ is a vector element, normal to the plane where $\left(\frac{\partial Q}{\partial x} - \frac{\partial P}{\partial y}\right)$ is being calculated
