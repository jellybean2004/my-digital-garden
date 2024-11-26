---
dg-publish: true
---

![Pasted image 20241114121449.png](/img/user/pics/Pasted%20image%2020241114121449.png)
- $d\vec n$ is normal, and $d\vec r$ is tangent to the curve: 
$$\begin{align*}
	d\vec r &= dx\,\hat i + dy\,\hat j \\
	d\vec n &= dy\,\hat i + dx\,\hat j
\end{align*}$$
![Pasted image 20241114121940.png](/img/user/pics/Pasted%20image%2020241114121940.png)
- for the vectors: 
$$\vec F = F_{x}\,\hat i + F_{y}\,\hat j$$
- then: 
$$\oint_{C} \vec F \cdot d\vec n = \oint F_{x}\,dy - F_{y}\,dx$$
- this is the $LHS$ of [[content/012/PX275 - mathematical methods/D - vector integration/D3 - green's theorem/PX275 - D3a - green's theorem in the plane\|green's theorem]]: 
$$\begin{align*}
	P &= - F_{y} \\
	Q &= F_{x}
\end{align*}$$
- green's theorem: 
$$\oint P\,dx + Q\,dy = \iint_{R }\left(\frac{\partial Q}{\partial x}- \frac{\partial P}{\partial y}\right)\,dA$$
- using the comparison with green's theorem: 
$$\oint F_{x}\,dx - F_{y}\,dy =\iint_{R} \underbrace{\left(\frac{\partial F_{x}}{\partial x} + \frac{\partial F_{y}}{\partial y}\right)}_{\vec\nabla\cdot F} \,dA$$
- therefore, **the divergence theorem in 2D** (AKA integral form of the divergence): 
$$\oint_{C} \vec F \cdot d\vec n = \iint_{R }\vec\nabla\cdot \vec F \,dA$$
