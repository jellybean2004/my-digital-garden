---
{"dg-publish":true,"permalink":"/content/011/px-153-mathematics-for-physicists/term-1/px-153-c-first-order-od-es/px-153-c4-separation-of-variables/","noteIcon":"1","created":"2024-11-25T10:50:32.000+00:00","updated":"2024-11-26T19:36:54.762+00:00"}
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
