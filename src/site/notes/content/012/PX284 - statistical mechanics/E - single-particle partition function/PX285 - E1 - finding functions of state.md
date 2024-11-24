---
dg-publish: true
---
## internal energy
$$\begin{align*}
	U &= \langle{E}\rangle \\
	&= \sum\limits_{i}E_{i}P_{i} \\
	&= \sum\limits_{i} \frac{E_{i}\exp(-\beta E_{i})}{Z} \\
	&= - \frac{1}{Z} \frac{dZ}{d\beta}
\end{align*}$$
$$\boxed{\therefore U = - \frac{d \ln Z}{d\beta}}$$
## entropy
$$S = - k_{B} \sum\limits_{i}P_{i} \ln P_{i}$$
- but: 
$$\begin{align*}
	P_{i} &= \frac{\exp(-\beta E_{i})}{Z} \\
\therefore \ln P_{i} &= - \beta E_{i} - \ln Z
\end{align*}$$
$$\implies S = k_{B} \sum_{i} P-i (\beta E_{i} + \ln Z) = k_{B}(\beta U + \ln Z)$$
**note:** $U = \sum\limits_{i} E_{i}P_{i}$ and $\sum\limits_{i} P_{i} =1$
## helmholtz free energy
$$\boxed{F = U - TS}$$
### aside on thermodyanamics
- but $dU = T\,dS - p\,dV$
$$dF = T\,dS - p\,dV - T\,dS - S\,dT = -S\,d - p\,dV$$
$$\begin{align*}
	\left(\frac{\partial F}{\partial T}\right)_{V} &=  -S \\
	\left(\frac{\partial F}{\partial V}\right)_{T } &= -p
\end{align*}$$
###
- in terms of $Z_{i}:$ 
$$F = U - k_{B}T (\beta U + \ln Z)$$
$$\boxed{ F = - k_{B}T\ln Z}$$
- **note:** $Z = \exp(-\beta F)$
## others
- similarly, expressions for other thermodynamic potentials
- enthalpy: 
$$H = U + pV$$
- gibb's free energy: 
$$G = H - TS$$
- $Z$ can be used to find $U$ and $F$, and hence find ${} S:$ 
$$ S= \frac{U-F}{T}$$
- also, heat capacity: 
$$C_{V} = \left(\frac{\partial U}{\partial T}\right)_{V}$$
