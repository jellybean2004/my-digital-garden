---
{"dg-publish":true,"permalink":"/content/011/px-157-electricity-and-magnetism/px-157-c-magnetic-fields/px-157-c3d-forces-between-two-current-loops/","created":"2024-10-01T18:27:10.193+01:00","updated":"2024-11-26T20:09:28.648+00:00"}
---

- two parallel straight wires, each carrying a current in the positive $z$-direction:
	- wire 1 is centred at $x=y=0$
	- wire 2 is centred at $y=a,\, x=0$
- the magnetic field generated by wire 1:
$$
\vec B_{1}(\vec r) = \frac{\mu_{0}I_{1}}{2\pi R} \hat\phi
$$
	- at wire 2:
$$
\vec B_{1}(at\;2) = -\frac{\mu_{0}I_{1}}{2\pi a} \hat x
$$
- the magnetic field generated by wire 2:
$$
\vec B_{2}(\vec r) = \frac{\mu_{0}I_{1}}{2\pi |\vec r - a\,\hat y|} \hat\phi_{2}
$$
	- at wire 1:
$$
\vec B_{2}(at\;1) = \frac{\mu_{0}I_{2}}{2\pi a} \hat x
$$
- force per unit length on wire 1 due to $\vec B_{2}(at\;1):$
$$
\vec F_{1}= I_{1}\,\hat z \times \vec B_{2}(at\;1) = I_{1} \frac{\mu_{0}I_{2}}{2\pi a} \hat z \times \hat x = \frac{\mu_{0}I_{1}I_{2}}{2\pi a}\hat y
$$
- force per unit length on wire 2 due to $\vec B_{1}(at\;2):$
$$
\vec F_{2}= I_{2}\,\hat z \times \vec B_{1}(at\;2) = I_{2} \frac{-\mu_{0}I_{1}}{2\pi a} \hat z \times \hat x = -\frac{\mu_{0}I_{1}I_{2}}{2\pi a}\hat y
$$
- **currents in the same direction attract each other and in the opposite directions repel each other**