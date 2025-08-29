---
{"dg-publish":true,"permalink":"/content/011/px-153-mathematics-for-physicists/term-1/px-153-b-complex-numbers/px-153-b5-application-describing-damped-smh/","noteIcon":"1","created":"2025-08-27T13:14:08.631+01:00","updated":"2024-11-26T19:36:38.000+00:00"}
---

## general solution
- conder mass on a spring on a surface to give a friction force proportional to the speed of the mass
- the equation of motion becomes: 
$$m \frac{d^{2}x}{dt^{2}}=-kx-\gamma \frac{dx}{dt}$$
- rearrange: 
$$\frac{d^{2}x}{dt^{2}}+ \frac{\gamma}{m} \frac{dx}{dt}+ \frac{k}{m}x=0$$
- rewrite: 
$$ \frac{d^{2}x}{dt^{2}} + 2\alpha \frac{dx}{dt} + \omega_{0}^{2}x =0$$
		where, $\alpha = \frac{\gamma}{2m}$ , $\omega_{0}= \sqrt{\frac{k}{m}}$ 
{ #efbd92}

- try $x(t)=Ae^{\lambda t}$: 
$$\lambda^{2}+ 2\alpha \lambda + \omega_{0}^{2}=0$$
	- quadratic equation, two solutions: 
	$$\lambda_{1}=-\alpha+\sqrt{\alpha^{2}-\omega_{0}^{2}} \, ,\, and \, \, \lambda_{2}=-\alpha-\sqrt{\alpha^{2}-\omega_{0}^{2}}$$
	- the general solution: 
	$$x(t)=Ce^{\lambda_{1}t}+De^{\lambda_{2}t}$$
	$$x(t)= e^{-\alpha t}(Ce^{t\sqrt{\alpha^{2}-\omega_{0}^{2}}}+De^{-t\sqrt{\alpha^{2}-\omega_{0}^{2}}})$$
		- first, the damping/dissipative force acts to make the displacement decay over time ($e^{-\alpha t}$, $\alpha\in \mathbb R$)
		- three cases:
			- **case 1**: $\alpha^2<\omega_{0}^{2}$ - [[content/011/PX153 - mathematics for physicists/term 1/PX153 - B - complex numbers/PX153 - B5.1 - underdamping\|PX153 - B5.1 - underdamping]]
			- **case 2**: $\alpha^{2}>\omega_{0}^{2}$ - [[content/011/PX153 - mathematics for physicists/term 1/PX153 - B - complex numbers/PX153 - B5.2 - overdamping\|PX153 - B5.2 - overdamping]]
			- **case 3**: $\alpha^{2}=\omega_{0}^{2}$ - [[content/011/PX153 - mathematics for physicists/term 1/PX153 - B - complex numbers/PX153 - B5.3 - critical damping\|PX153 - B5.3 - critical damping]]

![Pasted image 20240105114744.png](/img/user/pics/Pasted%20image%2020240105114744.png)
