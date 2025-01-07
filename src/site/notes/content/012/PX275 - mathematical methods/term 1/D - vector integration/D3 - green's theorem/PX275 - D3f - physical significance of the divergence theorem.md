---
{"dg-publish":true,"permalink":"/content/012/px-275-mathematical-methods/term-1/d-vector-integration/d3-green-s-theorem/px-275-d3f-physical-significance-of-the-divergence-theorem/","noteIcon":"1","created":"2024-11-25T10:50:32.000+00:00","updated":"2024-11-26T10:05:51.118+00:00"}
---

## example 1 
![Pasted image 20241114123030.png](/img/user/pics/Pasted%20image%2020241114123030.png)
- looking at the velocity field of a flow of water, $\vec F$, which is uniform
- at a point, $A$, $\vec F \cdot d\vec n \sim+ve$, and at a point, ${} B$, $\vec F \cdot d\vec n \sim-ve$, but they have the same magnitude
- therefore, the contributions cancel each other out: 
$$(\vec F \cdot d\vec n)_{A} + (\vec F \cdot d\vec n)_B = 0$$
- this happens for all points on the loop, and therefore: 
$$\oint_{C}\vec F  \cdot d\vec n  = 0 \implies \iint_{R}\vec\nabla \cdot \vec F \,dA =0$$
- therefore, this is a *divergence free field*
## example 2
![Pasted image 20241114123720.png](/img/user/pics/Pasted%20image%2020241114123720.png)
- at any point on the curve, $\vec F$ and $d\vec n$ are parallel to each other, and $\vec F\cdot d\vec n$ is always positive: 
$$\oint_{C} \vec F \cdot d\vec n > 0$$
- therefore, $\vec F$ is not a *divergence free field*
