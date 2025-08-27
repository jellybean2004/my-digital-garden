---
{"dg-publish":true,"permalink":"/content/012/px-262-quantum-mechanics/term-2/m-basic-postulates-revisited/px-262-m3-dirac-notation/","noteIcon":"1","created":"2025-08-27T13:15:23.266+01:00","updated":"2025-06-12T18:11:20.000+01:00"}
---

- it is a very economical and powerful notation
- associated with each wavefunction, $\psi(x)$, is a state vector, $|\psi\rangle$, called a '**ket**'
- with each complex conjugate, there is an associated '**bra**', $\langle \psi|$
$$\begin{gather}
\int \phi^{*}(x') \psi('x)\,dx' = \langle{\phi|\psi}\rangle \\
 (\langle{\phi|\psi}\rangle)^{*} = \langle{\psi|\phi}\rangle
\end{gather}$$
- for an expression involving an operator, eg: an expectation value:
$$\int \psi^{*} (x') \hat A \psi(x') \, dx' = \langle{\psi | A | \psi}\rangle $$
- the eigenvalue equation is written as:
$$\hat A | a \rangle = \lambda_{a}| a \rangle$$
	where, state $|a\rangle$ is labelled by its eigenvalue

- orthonormality:
$$\langle{a_{1}|a_{2}\rangle}= \delta_{a_{1}, a_{2}}$$

- the expansion process:
$$\begin{gather}
|\psi\rangle = \sum\limits_{a}c_{a}|a\rangle \\
c_{a_{1}} = \langle{a_{1} | \psi}\rangle \\
|\psi\rangle = \sum\limits_{a} |a\rangle \langle{a | \psi}\rangle \\
\sum\limits_{a} |a\rangle \langle a| = 1
\end{gather}$$ 
- using this, a lot of quantum mechanical problems can be recast in the language of matrices
- this can be used to make approximations and models
- the schrödinger equation:
$$\hat H | \psi \rangle = i \hbar \frac{d}{dt} |\psi\rangle$$
	where, the representation has not yet been specified

- choosing some basis of states, $|a\rangle:$
$$|\psi\rangle = \sum\limits_{a} |a\rangle \langle{a|\psi}\rangle$$
$$\begin{gather}
\sum\limits_{a} \hat H |a\rangle \langle{a|\psi}\rangle = i\hbar \sum\limits_{a} |a \rangle \frac{d}{dt} \langle{a|\psi}\rangle \\ 
\sum\limits \langle{a_{1} | \hat H | a}\rangle \langle{a|\psi}\rangle = i\hbar \sum\limits_{a} \langle{a_{1}|a}\rangle \frac{d}{dt} \langle{a|\psi}\rangle
\end{gather}$$
- ie. multiplied the schrodinger equation on the left by $\langle a_{1}|$
$$\sum\limits_{a} H_{a,a} c_{a}(t) = i\hbar \frac{d}{dt}c_{a_{1}}(t)$$
$$\begin{pmatrix}H_{11} & H_{12}& \dots \\
H_{21} &\ddots & \\
\vdots & & \ddots\end{pmatrix}
\begin{pmatrix}c_{1}(t)  \\ c_{2}(t) \\ \vdots\end{pmatrix}
= i\hbar \frac{d}{dt} \begin{pmatrix}c_{1} \\ c_{2}\\ \vdots\end{pmatrix}$$
- $H_{a,a}$'s have the form of a square matrix
- to illustrate, considering the case of two base states forming a complete set, eg: spin
$$|\psi\rangle = c_{1}|\uparrow \rangle+ c_{2}|\downarrow\rangle$$
- eg:
$$\begin{gather}
\langle{\uparrow | \hat H | \uparrow}\rangle = E_{0} \\
H_{12} = \langle{\uparrow | \hat H | \downarrow}\rangle = A = H_{21} \\
H_{22}= \langle{\downarrow | \hat H | \downarrow}\rangle = E_{0} \\\\
\begin{pmatrix} E_{0} & A \\ A & E_{0}\end{pmatrix} \begin{pmatrix}c_{1}\\c_{2}\end{pmatrix} = i\hbar \frac{d}{dt} \begin{pmatrix}c_{1} \\ c_{2}\end{pmatrix} \\
E_{0}c_{1} + A c_{2}(t) = i\hbar \frac{dc_{1}}{dt} \\
A c_{1} + E_{0} c_{2}(t) = i\hbar \frac{dc_{2}}{dt}
\end{gather}$$
- it is useful to have a representation that diagonalizes the $H$-matrix
- to do this, the eigenstates and eigenvalues of the hamiltonian need to be found
$$\begin{gather}
\hat H | n \rangle = E_{n} | n \rangle \\
|\psi \rangle = \sum\limits_{n} c_{n}(t) | n \rangle \\
\text{and, } c_{n} (t) = \langle{ n_{1} | \psi}\rangle \\\\
|\psi\rangle = \sum\limits_{n}|n\rangle \langle{ n |\psi}\rangle \\
\sum\limits_{n} \hat H | n \rangle \langle{ n | \psi}\rangle = i \hbar  \sum\limits | n \rangle \frac{d}{dt} \langle{ n |\psi}\rangle \\
\sum\limits_{n} \hat H | n \rangle c_{n}(t) = i\hbar \sum\limits_{n} |n \rangle \frac{dc_{n}}{dt} \\
\end{gather}$$
- forming a matrix, $\langle n_{1} |:$
$$\begin{gather}
\sum\limits_{n} \langle{ n_{1} | \hat H | n}\rangle c_{n} (t) = i\hbar \sum\limits_{n} \langle{n_{1} | n}\rangle \frac{dc_{n}}{dt} \\
\hat H | n \rangle = E_{n} | n \rangle \\\\
\langle{n_{1} | \hat H | n}\rangle = E_{n} \langle{ n_{1} | n}\rangle = E_{n} \delta_{nn_{1}}  \\
E_{n_{1}} c_{n_{1}} = i\hbar \frac{dc_{n_{1}}}{dt}  \\
c_{n_{1}}(t) = c_{n_{1}}(0) \exp\left(- \frac{iE_{n_{1}}t}{\hbar}\right) \\
|\psi(t) \rangle = \sum\limits_{n} c_{n}(0) | n \rangle  \exp\left(- \frac{iE_{n_{1}}t}{\hbar}\right)
\end{gather}$$
- with the initial $| \psi(0) \rangle$ state known, $|\psi(t)\rangle$ can be found
