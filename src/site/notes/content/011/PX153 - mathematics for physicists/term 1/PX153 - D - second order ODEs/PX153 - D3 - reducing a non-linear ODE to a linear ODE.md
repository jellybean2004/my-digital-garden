---
{"dg-publish":true,"permalink":"/content/011/px-153-mathematics-for-physicists/term-1/px-153-d-second-order-od-es/px-153-d3-reducing-a-non-linear-ode-to-a-linear-ode/","noteIcon":"1","created":"2025-08-27T13:14:08.759+01:00","updated":"2024-11-26T19:37:07.000+00:00"}
---

- non-linear ODEs are usually very difficult or impossible to solve, so, we try to make assumptions to simplify them
- here, we give the example of a pendulum
![Pasted image 20231031162134.png](/img/user/pics/Pasted%20image%2020231031162134.png)
- the length of arc $ds$ travelled in $dt$ is related to the change in the angle $d\theta$: $ds = ld\theta$
- so the acceleration is $\frac{d^{2}s}{dt^{2}} = l \frac{d^{2}\theta}{dt^{2}}$
- this must be equal to the component of the gravity tangential to the trajectory $-mg\sin\theta$
- giving: $ml \frac{d^{2}\theta}{dt^{2}} = -mg\sin\theta$
		$$\frac{d^{2}\theta}{dt^{2}} = - \frac{g}{l}\sin\theta$$
	- this is non-linear and very tough to solve
- to simplify the differential, we make a small angle approximation, such that $\sin\theta \approx \theta$: $$\frac{d^{2}\theta}{dt^{2}} \simeq - \frac{g}{l}\theta$$
