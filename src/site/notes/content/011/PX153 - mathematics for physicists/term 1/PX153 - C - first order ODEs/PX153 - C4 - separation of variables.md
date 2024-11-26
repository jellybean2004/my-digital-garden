---
dg-publish: true
---

- if an ODE can be written as $\frac{dy}{dx}=f(x)g(y)$, then solve by rearranging and integrating: 
$$\int \frac{1}{g(x)}.dy = \int f(x).dx$$
- eg: solve: $\frac{dN}{dt}=-\alpha N$
		$\int \frac{1}{N}.dN=\int -\alpha .dt$
			$\ln{N}=-\alpha t +c$
			$N = e^{-\alpha t + c}=e^{c}e^{-\alpha t}$
		$\therefore N=Ae^{-\alpha t}$
	 - equally valid approach as using a trial approach
- eg: solve the differential equation from the *[[content/011/PX153 - mathematics for physicists/term 1/PX153 - C - first order ODEs/PX153 - C2 - construction of ODEs#^a397d9\|height of water example ]]*
	- ![Pasted image 20231024162834.png](/img/user/pics/Pasted%20image%2020231024162834.png)
