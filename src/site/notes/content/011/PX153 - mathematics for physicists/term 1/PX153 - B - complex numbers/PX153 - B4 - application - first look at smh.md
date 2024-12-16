---
{"dg-publish":true,"permalink":"/content/011/px-153-mathematics-for-physicists/term-1/px-153-b-complex-numbers/px-153-b4-application-first-look-at-smh/","noteIcon":"1","created":"2024-11-25T10:50:32.000+00:00","updated":"2024-11-26T19:36:35.525+00:00"}
---

- as an example, let's look at a mass on a spring
- the force on the mass $\vec F=-kx\hat{\vec{x}}$
- using [[content/011/PX155 - classical mechanics and special relativity/classical mechanics/PX155 - A - foundations of classical mechanics/PX155 - A2 - newton's second law\|PX155 - A2 - newton's second law]], we can derive the equation of motion: 
$$m \frac{d^2x}{dt^2}=-kx$$
or, 
$$\frac{d^2x}{dt^2}= - \frac{k}{m}x$$
- let $\omega_0=\sqrt{\frac{k}{m}}$
- now we need to solve the 2nd order differential equation:$$\frac{d^2x}{dt^2}=-\omega_0^2x$$
- try solution: $x(t)=Ae^{\lambda t}$
	$$\frac{dx}{dt}= A\lambda e^{\lambda t}=\lambda x$$
	$$\frac{d^2x}{dt^2}=A\lambda^{2}e^{\lambda t} =\lambda^2 x$$
- from this, 
$$-\omega_0^2x=\lambda^2x$$
	- for this to be generally true, $-\omega_0^2=\lambda^{2}\implies \lambda=\pm i\omega_0$
	- both roots are equally valid, hence the general solution is the sum of both:
	$$x(t)=Ce^{i\omega_0t}+De^{-i\omega_0t}$$
- aside: helpful to consider dimensions
- eg: what are the dimensions of $\omega_0$? 
	- $e^{-i\omega_0t}$ so, $\omega_{0}t$ must be dimensionless
	- $[\omega_0]=s^{-1}$

- suppose the initial condition are $x(0)=x_0$ and the value of $v(0)= \frac{dx(0)}{dt}=0$
	- we then have: 
	$$x(0)=Ce^0+De^0=C+D=x_0$$
	- and:
		$v(0)= \frac{dx}{dt}=i\omega_0Ce^0-i\omega_0De^0=0$
		$\implies C-D=0$
		$\therefore C=D=\frac{1}{2}x_0$
		$\implies x(t)=\frac{1}{2}x_0(e^{i\omega_0t}+e^{-i\omega_0t})$
- if instead, the initial conditions are $x(0)=0$ and $v(0)=v_0$
	$$x(t)=Ce^{i\omega_0t}+De^{-i\omega_0t}$$
	$\implies 0 = Ce^0+De^0\implies 0=C+D$
	and $v= \frac{dx}{dt}=i\omega_0 Ce^0-i\omega_0 De^0=v_0$
	$\implies C-D= \frac{v_{0}}{i\omega_{0}}$
	$\implies 2C=\frac{v_{0}}{i\omega_{0}} \implies C=\frac{v_{0}}{2i\omega_{0}}$
	$\implies D=-C=-\frac{v_{0}}{2i\omega_{0}}$
	giving, 
\1\n\2\n