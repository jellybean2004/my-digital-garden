---
{"dg-publish":true,"permalink":"/my-digital-garden/012/px-275-mathematical-methods/b-coordinate-systems-and-integration/b2-4-integration/px-275-b3a-hyperbolic-coordinates/","created":"2024-11-25T10:50:32.000+00:00","updated":"2024-11-26T10:04:53.108+00:00"}
---

- consider the thermodynamics of an ideal gas: $pV = nRT$
![Pasted image 20241021124456.png](/img/user/pics/Pasted%20image%2020241021124456.png)
- whilst, it can be integrated over the area, $\Omega$, it would be better to find another region
- the problem is simplified with hyperbolic coordinates: 
$$pV = R \;;\;\frac{p}{V}= s$$
- in $(r,s)$ space, the problem is:
![Pasted image 20241021125012.png](/img/user/pics/Pasted%20image%2020241021125012.png)
- going from $A$ to $B: \frac{P}{V}= c_{1} = \text{constant} \implies s$ is constant
- going from ${} B$ to $C: pV = nRT_{2} = \text{constant} \implies r$ is constant 
- going from ${} C$ to $D: \frac{P}{V}= c_{2} = \text{constant} \implies s$ is constant 
- going from ${} D$ to $A: pV = nRT_{1} = \text{constant} \implies r$ is constant

- to undertake this transformation: 
$$J = \frac{\partial (p,V)}{\partial (r,s)}$$
$$I_{\Omega}= \int_{s_{1}}^{s_{2}} \int_{r_{1}}^{r_{2}} |J|\,dr\,ds$$
