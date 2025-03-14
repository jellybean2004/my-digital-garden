---
{"dg-publish":true,"permalink":"/content/012/px-262-quantum-mechanics/term-2/k-crystalline-solids/px-262-k5-block-wavefunctions-electronic-energy-bands-and-gaps/","noteIcon":"1","created":"2025-02-10T16:32:33.010+00:00","updated":"2025-02-10T16:45:46.565+00:00"}
---

- considering a 1D lattice

![PX262 - H18 - block wavefunctions, electronic energy bands and gaps}.png|500](/img/user/pics/PX262%20-%20H18%20-%20block%20wavefunctions,%20electronic%20energy%20bands%20and%20gaps%7D.png)

- attaching a potential to the lattice:
$$V(x) = V(x + R_{n}) = \sum\limits_{h} V_{h}\exp(iG_{h}x)$$
- since $\exp(iG_{h}x)=1$
- for an electron moving in such a periodic potential, the wavefunction must have a form: 
$$\phi_{n,k} = e^{ikx} u_{n,k}(x)$$
	where, $u_{n,k}(x) = u_{n,k}(x + R_{n})$, ie. it is periodic
	
- the probability will also be periodic: 
$$\phi_{n,k}^{*}(x) \phi(x) = e^{-ikx} u^{*}_{n,k} (x)\, e^{ikx} u_{n,k}(x) = u^{*}_{n,k}(x) u_{n,k}(x)$$
- this is **bloch's theorem**

- similarly, for 3D, the crystal lattice with $\vec R_{n_{1},n_{2},n_{3}}$ and $\vec G_{h,k,l}$
- the potential: 
$$V(\vec r) = V(\vec r + \vec R_{n_{1},n_{2},n_{3}}) = \sum\limits_{h,k,l} V_{h,k,l} \exp(i \vec G_{h,k,l} \cdot \vec r)$$
- since $\vec \exp(i\vec G_{h,k,l}\cdot \vec r) = 1$
- bloch's theorem:
$$\phi_{h,k}(\vec r) = e^{i\vec k \cdot \vec r} u_{n,k} (\vec r)$$

- $u_{h,k}$ and $\phi_{h,k}\phi^{*}_{h,k}$ are periodic
- $n$ is a band index and $\vec k$ is the wavevector
