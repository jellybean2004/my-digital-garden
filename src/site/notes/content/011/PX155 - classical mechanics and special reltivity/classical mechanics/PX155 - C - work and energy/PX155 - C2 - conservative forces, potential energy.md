---
{"dg-publish":true,"permalink":"/content/011/px-155-classical-mechanics-and-special-reltivity/classical-mechanics/px-155-c-work-and-energy/px-155-c2-conservative-forces-potential-energy/","created":"2024-10-01T18:27:09.516+01:00","updated":"2024-11-26T19:55:23.428+00:00"}
---

## conservative forces
- work done is independent of the path
	- 'conservative' as in energy conserving
![Pasted image 20231018080503.png](/img/user/pics/Pasted%20image%2020231018080503.png)
- conservative if
$$\int_A^B \vec F d\vec r \;|_P=\int_A^B \vec F d\vec r\;|_{P'}$$
- here,
$$\int_A^B \vec F d\vec r\;|_P+\int_B^A \vec F d\vec r\;|_{P'}=0$$
- this can be written as,
$$\oint \vec F d\vec r = 0$$
	- means that the path is a closed loop
- work done in reaching any point $P$ from an origin $O$ depends only on the position of $P$
- define a function $U=-W(O \to P)$ and set $U(0)=0$, where $U$ is the potential energy
	- $W(A\to B)=W(A\to 0)+W(0\to B)= U(A)-U(B)$
		$=-[U(B)-U(A)]$
		$=-\Delta U$
	- $W(A\to B)$ is also $\Delta T$
		$\Delta T=-\Delta U$
		$\Delta T + \Delta U = 0$
			$\therefore T+U$, AKA total mechanical energy, is constant/conserved provided that forces act as conservative
## deriving a force from a potential
- since $dW=F(x)dx=-dU$
	- in 1D:
$$F(x)=-\frac{dU}{dx}$$
	- in 3D:
$$\vec F=-\nabla U=-\frac{\delta U}{\delta x}\vec i-\frac{\delta U}{\delta y}\vec j-\frac{\delta U}{\delta x}\vec k$$
![Pasted image 20240218110334.png](/img/user/pics/Pasted%20image%2020240218110334.png)
- consider $U=mgh$ 
	- $F(h)= -\frac{dU}{dh}=-mg$
		- acts downwards
		- increases $T$, decreases $U$
- consider $U=\frac{1}{2}kx^2$
	- $F(x)=- \frac{dU}{dx}=-kx$
		- opposes displacement from $x=0$, *restoring force*
## the work that *you* do
- if *you* apply an equal and opposite force to a conservative force, you are pushing against the conservative force and you increase the potential energy
	- eg: raising a mass against gravity
		- you do positive work on the mass
		- gravity does negative work on the mass
	