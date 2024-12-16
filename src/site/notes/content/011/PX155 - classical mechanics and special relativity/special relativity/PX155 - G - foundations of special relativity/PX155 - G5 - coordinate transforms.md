---
{"dg-publish":true,"permalink":"/content/011/px-155-classical-mechanics-and-special-relativity/special-relativity/px-155-g-foundations-of-special-relativity/px-155-g5-coordinate-transforms/","noteIcon":"1","created":"2024-10-01T18:27:09.756+01:00","updated":"2024-11-26T19:58:21.542+00:00"}
---

- $t \neq t'$, so, new transforms are needed
- **RP1** implies motion in a straight line in one frame must be motion in a straight line (or no motion at all) in another, otherwise [[content/011/PX155 - classical mechanics and special relativity/classical mechanics/PX155 - A - foundations of classical mechanics/PX155 - A1 - newton's first law\|PX155 - A1 - newton's first law]] would not hold
- need *linear* coordinate transformations
- most general linear transformation:
$$x'  = Ax + Bt \;,\; t' = Dx+Ct$$
- alternatively:
$$\begin{pmatrix} x'\\ t'\end{pmatrix}  =  \begin{pmatrix} A & B\\ D & C \end{pmatrix}\begin{pmatrix} x \\ y \end{pmatrix}$$
- galilean tranforms:
		$A = 1, B = 4$
		$D = 0, C = 1$

- in standard configuration, $x'=0$, corresponding to $x=ut$:  $0 = Aut + Bt \implies B = -uA$
	$$x' = A(x-ut) \; ...[1]$$
	- run time backwards, now $S$ moves at speed $+u$ in frame $S'$
		- if $t \to -t$, then swap identity of frames:
$$x = A(x' +ut') \; ...[2]$$
		- Putting [1] in [2] : 
			$x = A(A(x-ut) +ut')$
			$Aut' = x- A^{2}x +A^{2}ut$
			$Aut' = (1-A^{2})x+A^{2}ut$
			$t' = A[t+ ( \frac{1-A^{2}}{A^{2}}) \frac{x}{u}]$
		
$$\therefore t' = \gamma \left [t+ \left ( \frac{1-\gamma^{2}}{\gamma^{2}} \right) \frac{x}{u} \right] \; , \; and \;x' = \gamma(x-ut)$$
		- if $A \neq 1$, $t'$ depends on both $x$ , and $t$
		- so, $C=A$, $D = \frac{1-A^{2}}{Au}$
$$\begin{pmatrix} x'\\ t'\end{pmatrix} \begin{pmatrix} \gamma & -u \gamma\\ 1- \frac{\gamma^{2}}{\gamma u} & \gamma \end{pmatrix} = \begin{pmatrix} x \\ y \end{pmatrix}$$
- **further reading** **matrix transformations**: textbook by A.P. French (link on the Moodle page)