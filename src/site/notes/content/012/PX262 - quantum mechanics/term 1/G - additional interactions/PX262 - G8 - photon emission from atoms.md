---
{"dg-publish":true,"permalink":"/content/012/px-262-quantum-mechanics/term-1/g-additional-interactions/px-262-g8-photon-emission-from-atoms/","noteIcon":"1","created":"2025-08-27T13:14:32.595+01:00","updated":"2024-12-23T10:57:59.000+00:00"}
---

- light emitted from atoms can be understood as emissions from electron deexcitation
- photons can be seen as a **periodic perturbation** of the electromagnetic field
## light polarized in $z$
- electromagnetic field in the form of a plane wave, aligned along the $z$-axis can be described as:
$$\varepsilon = \varepsilon_{0}z\cos(\vec k \cdot \vec r -\omega t ) \approx \varepsilon_{0}\,z\cos\omega t$$
	where, $\vec k \cdot \vec r$ is small in terms of atomic size
- the wavelength is much lager than the atom, so the field can be considered to be uniform across the atom
- the perturbation hamiltonian can be written as:
$$\hat H' = e\,\varepsilon_{0}z\cos\omega t = e\varepsilon z$$
	- this changes the state of the electron
- the variations are slow, so it can be treated as time-independent: 
$$\hat H'' = e \, \varepsilon_{0}z$$
- the probability of electron transition between two states in the hydrogen atom is given by the overlap integral:
$$\begin{align*}
H''_{12} &= e\, \varepsilon_{0}\int \phi_{n_{1}l_{1}m_{1}}^{*} \,z\, \phi_{n_{2}l_{2}m_{2}}\,d\tau \\\\
& \begin{multlined} = e\,\varepsilon \int_{0}^{2\pi}\int_{0}^{\pi} \int_{0}^{\infty}R_{n_{1}l_{1}}^{*}(r) P_{l_{1}}^{|m_{1}|} (\cos\theta) e^{-im_{1}\varphi} \\ 
r \cos\theta \, R_{n_{2}l_{2}}(r) P_{l_{2}}^{|m_{2}|} (\cos\theta) e^{im_{2}\varphi}\, r^{2} \sin\theta \, dr\, d\theta\, d\varphi \end{multlined} \\\\
& \begin{multlined} =e\,\varepsilon \int_{0}^{2\pi}
 e^{i(m_{2}-m_{1})\varphi}\, d\varphi  \\ \int_{0}^{\pi} P_{l_{1}}^{|m_{1}|}(\cos\theta) P_{l_{2}}^{|m_{2}|}(\cos\theta) \cos\theta\sin\theta\,d\theta \\ \shoveleft \int_{0}^{\infty}R_{n_{1}l_{1}}^{*}(r) \, R_{n_{2}l_{2}}(r) \, dr \end{multlined} 
\end{align*} $$
- the integral must be non-zero for transmissions to occur
- the integral cannot be fully evaluated generically, but the quantum numbers can be worked out

- considering the integral over $\varphi$, there is the product of two eigenfunctions of $\hat L_{z}$, which will be non-zero only if $m_{1} = m_{2}$

- considering the integral over $\theta$, the relationships between legendre polynomials:
$$(2l + 1)\cos\theta \,P_{l}^{|m|} = (l-|m|+1) P_{l+1}^{|m|} + (l + |m|) P_{l-1}^{|m|}$$
- using this relation for $P_{2}^{|m_{2}|}$, the integral can be rewritten as: 
$$A\int_{0}^{\pi} P_{l_{1}}^{|m_{1}|} P_{l_{2+1}}^{|m_{2}|} \sin\theta\,d\theta + B\int_{0}^{\pi} P_{l_{1}}^{|m_{1}|} P_{l_{2-1}}^{|m_{2}|} \sin\theta\,d\theta$$
	where, $A$ and $B$ contain constants that can be supressed for simplification
- using the orthogonality of the legendre polynomials, the integral will be non-zero only if: $l_{1} = l_{2}+1$ or $l_{1}= l_{2}-1$ 

- therefore, it can be concluded that the electron in a hydrogen atom can move between two states for which $l_{1} = l_{2} \pm 1$ and $m_{1} = m_{2}$
## light polarized in ${} x$

- the above discussion is only for light polarized in the $z$-direction, but light can be polarized in all directions
- considering light polarized in the $x$-direction:
$$\hat H '' = e\,\varepsilon_{0}r \sin\theta \cos\varphi$$
	where, $x = r\sin\theta\cos\varphi$

- considering the integral over $\varphi:$
$$\frac{1}{2} \int_{0}^{2\pi} \big[ e^{i(m_{2}-m_{1}+1)\varphi} + e^{i(m_{2}-m_{1}-1)\varphi} \big] \, d\varphi$$
	where, $\cos\varphi = \frac{1}{2} (e^{i\varphi} + e^{-i\varphi})$
- for this to be non-zero: $m_{1} = m_{2} \pm 1$

- considering the integral over $\theta:$ similar to above, this will only be non-zero if $l_{1} = l_{2} \pm 1$
## summary
- transitions are only possible between states which differ in orbital quantum number by $1$ $(\Delta l = \pm 1)$, and the magnetic quantum number remains the same or changes by $1$ $(\Delta m = 0,\pm1)$
- these transitions are called **electric dipole transitions**
- at this approximation, all other possibilities are forbidden
- such conditions are called **selection rules**