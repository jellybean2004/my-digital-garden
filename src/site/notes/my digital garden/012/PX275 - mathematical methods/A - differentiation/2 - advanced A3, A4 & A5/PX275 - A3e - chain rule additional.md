---
{"dg-publish":true,"permalink":"/my-digital-garden/012/px-275-mathematical-methods/a-differentiation/2-advanced-a3-a4-and-a5/px-275-a3e-chain-rule-additional/","created":"2024-11-25T10:50:32.000+00:00","updated":"2024-11-26T10:04:08.091+00:00"}
---

## comments
- more generally: 
	- $x_{1},x_{2}, x_{3},\dots x_{i}$ are used rather than $x,y,t$
	- $u_{1}, u_{2}, u_{3},\dots u_{j}$ are used rather than $\rho,\theta\,\phi$
	- for functions, $f,g$, just $f$ is used
- a more compact notation: 
$$\frac{\partial f}{\partial u_{j}} = \sum\limits_{i} \frac{\partial f}{\partial x_{i}} \frac{\partial x_{i}}{\partial u_{j}}$$
- in operator form: 
$$\frac{\partial }{\partial u_{j}} = \sum\limits_{i}\frac{\partial x_{i}}{\partial u_{j}} \frac{\partial }{\partial x_{i}}$$
## warning
$$\begin{gather}
x=\rho\cos\theta \\
\implies \frac{\partial x}{\partial \rho}=\cos\theta \\\\
\rho^{2}=x^{2}+y^{2} \\
\text{or, }\rho=(x^{2}+y^{2})^{\frac{1}{2}}\\\\
\implies \frac{\partial \rho}{\partial x} = \frac{x}{(x^{2}+y^{2})^{\frac{1}{2}}} = \frac{x}{\rho} \\
\frac{\partial \rho}{\partial x} =\cos\theta
\end{gather}$$
- expected: 
$$\frac{\partial x}{\partial \rho} = \left(\frac{\partial \rho}{\partial x}\right)^{-1}$$
- the reason: 
$$\left(\frac{\partial x}{\partial \rho}\right)_{\theta} \text{and } \left(\frac{\partial \rho}{\partial x}\right)_{y}$$ 
	- different variables are being held constant

### what does '*holding variables constant*' mean?
- consider $(\frac{\partial x}{\partial \rho})_{\theta} \text{ and }(\frac{\partial \rho}{\partial x})_{y}=\cos\theta$
- holding $\theta$ constant: $x\to x+dx$; $y\to y+dy$
![Pasted image 20241004173034.png](/img/user/pics/Pasted%20image%2020241004173034.png)
- holding $y$ constant $x\to x+dx$; $\theta\to\theta-d\theta$
![Pasted image 20241004173047.png](/img/user/pics/Pasted%20image%2020241004173047.png)

- **in general**: 'reciprocity relationship' will only hold if the variable being held constant is the same in both sides, ie: $\left(\frac{dy}{dx}\right)_{z} = \left(\frac{dx}{dy}\right)^{-1}_{z}$
