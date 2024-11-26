---
dg-publish: true
---
![Pasted image 20240123182243.png](/img/user/pics/Pasted%20image%2020240123182243.png)
- a charge, $q$, placed at the origin
- here, the path is radial: $d\vec l = dr\,\hat r$
- apply $V_{a}-V_{b} = \int_{a}^{b}\vec E \cdot d\vec l$ :
$$\begin{align*}
V_{a}- V_{b} &= \int_{a}^{b} \frac{q}{4\pi\epsilon_{0}r^{2}}\hat r \cdot \hat r\,dr \\
&= \frac{q}{4\pi\epsilon_{0}} \int_{r_{a}}^{r_{b}} \frac{1}{r^{2}}dr \\
&= \frac{q}{4\pi\epsilon_{0}}(\frac{1}{r_{a}}- \frac{1}{r_{b}})
\end{align*}$$
{ #163087}

- choose to put zero potential for $r_{b}\to \infty$:
$$
V_{a}-V(r\to\infty) = \frac{q}{4\pi\epsilon_{0}r_{a}}
$$
- this is true for any value of $r_{a}$:
$$
V(r) = \frac{q}{4\pi\epsilon_{0}r}
$$
```functionplot
dg-publish: true
---
title: 
xLabel: r
yLabel: V(r)
bounds: [0,5,0,5]
disableZoom: true
grid: true
---
f(x)=1/x
```
