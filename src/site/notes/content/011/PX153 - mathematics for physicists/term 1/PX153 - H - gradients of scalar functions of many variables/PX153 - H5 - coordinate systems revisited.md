---
{"dg-publish":true,"permalink":"/content/011/px-153-mathematics-for-physicists/term-1/px-153-h-gradients-of-scalar-functions-of-many-variables/px-153-h5-coordinate-systems-revisited/","noteIcon":"1","created":"2024-11-25T10:50:32.000+00:00","updated":"2024-11-26T19:37:53.394+00:00"}
---

- extension for *[[content/011/PX153 - mathematics for physicists/term 1/PX153 - A - vectors/PX153 - A5 - coordinate systems#circular polar coordinates\|circular polar coordinates]]*

- in general, in 3D, a coordinate system is defined by specifying 3 basis vectors at each point in space
- usually orthonormal basis vectors 
$$\hat{\vec e_{i}} \cdot \hat{\vec e_{j}} = \delta_{ij}$$
![Pasted image 20231205120403.png](/img/user/pics/Pasted%20image%2020231205120403.png)
- for polar coordinates: $\vec r (r, \theta)$ , where $r=$ magnitude of the vector, and $\theta =$ angle to the x-axis
		$x=r\cos\theta$
		$y = r\sin\theta$
		$r = \sqrt{x^{2}+y^{2}}$
		$\theta = \arctan(\frac{x}{y})$
- from figure above, and trigonometry: 
$$\hat{\vec e}_{r} = \cos\theta \; \hat{\vec e}_{x} + \sin\theta \; \hat{\vec e}_{y}$$
$$\hat{\vec e}_{\theta} = -\sin\theta \; \hat{\vec e}_{x} + \cos\theta \; \hat{\vec e}_{y}$$
- in cartesian coordinates: 
$$\vec r = x \hat{\vec e}_{x} + y \hat{\vec e}_{y}$$
- also, 
$$\vec e_{x} = \left(\frac{\partial \vec r}{\partial r}\right)_{y} = \hat{\vec e}_{x}$$
	- ie: basis vectors are in direction of increasing coordinate
$$\vec e_{r} = \left( \frac{\partial \vec r}{\partial r} \right)_{\theta}$$
$$\vec e_{\theta} = \left( \frac{\partial \vec r}{\partial \theta}\right)_{r}$$
- again, 
$$\vec r = x \vec e_{x} + y \vec e_{y}$$
	- rewriting $x$ and $y$ : 
	$$\vec r = r \cos\theta \; \vec e_{x} + r\sin\theta \; \vec e_{y}$$
- we have, 
$$\vec e_{r} = \left( \frac{\partial \vec r}{\partial r} \right)_{\theta} = \cos\theta \; \vec e_{x} + \sin\theta \; \vec e_{y}$$
	- and, 
	$$\vec e_{\theta} = \left( \frac{\partial \vec r}{\partial \theta}\right)_{r} = -r \sin\theta \; \vec e_{x} + r \cos\theta \; \vec e_{y}$$
- note: 
	- $|\vec e_{r}| = 1 \implies \hat{\vec e}_{r} = \vec e_{r}$ : $$\hat {\vec e}_{r} = \vec e_r$$
	- $|\vec e_{\theta}| = r$ :
$$\therefore \hat{\vec e}_{\theta} =  \frac{\vec e_{\theta}}{r} = -\sin\theta \hat{\vec e}_{x} + \cos\theta \hat{\vec e}_y$$
- both are functions of $\theta$ only: 
$$\frac{d\hat{\vec e}_{r}}{d\theta} = -\sin\theta \; \hat{\vec e}_{x} + \cos\theta \; \hat{\vec e}_{y} = \hat{\vec e}_{\theta}$$
$$\frac{d\hat{\vec e}_{\theta}}{d\theta} = -\cos\theta \; \hat{\vec e}_{x} - \sin\theta \; \hat{\vec e}_{y} = -\hat{\vec e}_{r}$$
- the position vector in cartesian coordinates is $\vec r = x\hat{\vec e}_{x} + y \hat{\vec e}_{y}$ , but in polar, it is $\vec r = r \hat{\vec e}_{r}$

- eg: circular motion of an object with radius, $r$, constant angular velocity, $\omega \,rad \, s^{-1}$
	- the linear velocity: 
	$$\vec v = \frac{d\vec r}{dt} = \frac{d}{dt}(r\hat{\vec e}_{r}) = \dot r \hat{\vec e}_{r} + r \dot{\hat{\vec e}}_{r}$$
		- $\theta$ is a function of time: 
		$$\dot{\hat{\vec e}}_{r} = \frac{d\hat{\vec e}_r}{d\theta} \cdot \frac{d\theta}{dt} = \omega \hat{\vec e}_{\theta}$$
		- we know $\dot r = 0$ : 
		$$\vec v = \omega r \hat{\vec e}_{\theta}$$
		- this is a well known result, $v=\omega r$, and direction is tangential

	- similarly, acceleration: 
	$$\vec a = \frac{d\vec v}{dt} = \frac{d}{dt}(\omega r \hat{\vec e}_{\theta}) = r\omega \frac{d}{dt}\hat{\vec e}_{\theta}$$
	- we know $\theta$ is a function of time: 
	$$\frac{d}{dt}\hat{\vec e}_{\theta} = \frac{d \hat{\vec e}_{\theta}}{d\theta} \cdot \frac{d\theta}{dt} = -\omega\hat{\vec e}_r$$
	$$\therefore \vec a = -r\omega^{2}\hat{\vec e}_r$$


