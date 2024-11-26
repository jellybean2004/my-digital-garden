---
{"dg-publish":true,"permalink":"/my-digital-garden/012/px-262-quantum-mechanics/c-the-basic-postulates/px-262-c7a-the-uncertainty-principle/","created":"2024-11-25T10:50:32.000+00:00","updated":"2024-11-26T01:07:28.999+00:00"}
---

## derivation
- if $\hat  Q$ and $\hat  R$ are hermitian, then $(\hat Q \hat R + \hat R\hat Q)$ and $i(\hat Q \hat R - \hat R\hat Q)$ are also hermitian
- this means that $\hat Q^{2}$ is also hermitian
- the mean: 
  $$\langle{\hat Q}\rangle = \int \psi^{*} \hat Q \psi\,d\tau$$
- the 'spread', or the standard deviation is: 
  $$\Delta q^{2}= \int \psi^{*}(\hat Q - \langle{\hat Q}\rangle)^{2}\psi \,d\tau = \int \psi^{*}\hat Q'\hat Q' \psi \, d\tau$$
	where, $\hat Q' = \hat Q - \langle{\hat Q}\rangle$
- using the definition of hermitian operators:
   $$\Delta q^{2}=  \int (\hat Q' \psi) (\hat Q'^{*}\psi^{*}) \, d\tau = \int |\hat Q' \psi|^{2}\,d\tau$$
- similarly, for $\hat R:$  
  $$\Delta r^{2} = \int |\hat R' \psi|^{2}\,d\tau$$
	where, $\hat R' = \hat R - \langle{\hat R}\rangle$
- multiplying the two spreads, and using *schwarz's inequality:* 
  $$\Delta q^{2} \Delta r^{2} = \int |\hat Q' \psi|^{2}\,d\tau \int |\hat R' \psi|^{2}\,d\tau \geq \left|\int (\hat Q'\psi^{*}) (\hat R' \psi)\,d\tau \right|^{2} $$
$$\begin{align*}
	\int (\hat Q'\psi^{*}) (\hat R' \psi)\,d\tau  &= \int \psi^{*} \hat Q' \hat R' \psi\,d\tau \\
	&= \frac{1}{2}\int \psi^{*} (\hat Q' \hat R' - \hat R'\hat Q') \psi \,d\tau + \frac{1}{2}\int \psi^{*} (\hat Q' \hat R' + \hat R'\hat Q') \psi \,d\tau \\
\end{align*}$$
- the first integral is the imaginary part, and the second integral is the real part of the product
$$\Delta q^{2} \Delta r^{2} \geq \left(\frac{1}{4} \left|\int \psi^{*} [\hat Q' , \hat R'] \psi \,d\tau \right|^{2} + \left|\int \psi^{*} (\hat Q' \hat R' + \hat R'\hat Q') \psi \,d\tau\right|^{2}\right)$$
- the second integral, which is real, will have a positive value for square, so: 
  $$\Delta q^{2} \Delta r^{2}\geq \frac{1}{4} \left|\int \psi^{*} [\hat Q' , \hat R'] \psi \,d\tau \right|^{2}$$
- it can be shown that $[\hat Q', \hat R'] = [\hat Q, \hat R]$, so: 
  $$\Delta q \Delta r \geq \frac{1}{2} \left| \langle{[\hat Q , \hat R]}\rangle \right|$$
- this is generalized heisenberg's uncertainty principle
- for position and momentum operators, $[\hat X, \hat P_{x}] = i\hbar:$ 
  $$\Delta x \Delta p_{x} = \frac{\hbar}{2}$$
## interpretation
- the two quantities are measured on different copies of the QM system
- HUP does not tell how one variable is affected by the measurement of another
- it tells how well given quantities can be measured or predicted