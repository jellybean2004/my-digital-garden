---
dg-publish: true
---

#publish
## 1D blackbody
- a box of length, $L$
- the electric field: 
$$\vec E (0,t) = \vec E(L,t) = 0$$
```functionplot
---
title: 
xLabel: x
yLabel: E
bounds: [0,6.28,-2,2]
disableZoom: true
grid: true
---
f(x)  = sin(x)
g(x) = sin(2x)
h(x) = sin(3x)
```
$$E_{n} \sim \sin\left(\frac{n\pi}{L}\right)\sin(\omega_{n}t) \;,\; n=1,2,3$$
- allowed standing waves, "modes": 
$$\lambda_{n}= \frac{2L}{n}\implies \lambda_{n}<<2L\;for\; n>>1$$
$$\delta n = \frac{dn}{d\lambda}(-\delta\lambda) = \frac{2L}{\lambda^{2}}\delta\lambda$$
- energy in modes with wavelengths between $\lambda\to\lambda-\delta\lambda:$ 
$$e(\lambda,T) = \frac{2L}{\lambda^{2}}k_{B}\,T\,\delta\lambda$$
## 3D blackbody
- a cube of length, $L$
$$e(\lambda,T) = \frac{8\,\pi\,L^{3}}{\lambda^{4}}k_{B}\,T\,\delta\lambda$$
- converting $e(\lambda,T)$ to $I(\lambda)$ gives the *rayleigh-jeans law*: 
$$I(\lambda) = \frac{2\,\pi\,c\,k_{B}\,T}{\lambda^{4}}$$
![Pasted image 20240213114920.png](/img/user/pics/Pasted%20image%2020240213114920.png)
- not found experimentally, as it lead to the '*ultraviolet catastrophe*'
