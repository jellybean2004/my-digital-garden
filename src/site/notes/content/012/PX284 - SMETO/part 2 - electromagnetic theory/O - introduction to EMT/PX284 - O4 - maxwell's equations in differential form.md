---
{"dg-publish":true,"permalink":"/content/012/px-284-smeto/part-2-electromagnetic-theory/o-introduction-to-emt/px-284-o4-maxwell-s-equations-in-differential-form/","noteIcon":"1","created":"2025-08-27T13:15:25.107+01:00","updated":"2025-02-13T17:22:22.000+00:00"}
---

## gauss' law
$\newcommand{\oiint}{\subset\!\supset \!\!\!\!\!\!\!\!\!\!\iint}\newcommand{\oiint}{\subset\!\supset \!\!\!\!\!\!\!\!\!\!\iint}$
$$\begin{gather}
\oiint_{S} \vec E \cdot d\vec S = = \iiint_{V}\vec\nabla\cdot\vec E\, dV = \iiint_{V} \frac{\rho}{\epsilon_{0}}\, dV \\
\iiint_{V} \left(\vec\nabla\cdot \vec E - \frac{\rho}{\varepsilon_{0}}\right) \, dV = 0 \\
\therefore \vec\nabla\cdot\vec E = \frac{\rho}{\varepsilon_{0}} \tag{1}
\end{gather}$$

## solenoidal condition
$$\begin{gather}
\oiint_{S} \vec B \cdot d\vec S = \iiint_{V} (\vec\nabla\cdot\vec B)\, dV = 0  \\
\therefore \vec\nabla\cdot\vec B = 0 \tag{2}
\end{gather}$$
## faraday-lenz law
- this requires [[content/012/PX275 - mathematical methods/term 1/E - stoke's theorem and the divergence theorem/PX275 - E1a - stokes' theorem\|stokes' theorem]]
$$\begin{gather}
\oint_{C} \vec E \cdot d\vec l = \iint_{S} ( \vec\nabla \times \vec E)\cdot d\vec S  = - \frac{d}{dt} \iint_{S} \vec B \cdot d\vec S \\
\iint_{S} \left(\vec\nabla \times \vec E + \frac{\partial  \vec B}{\partial t}\right)\cdot d\vec S = 0 \\
\therefore \vec\nabla \times \vec E =- \frac{\partial \vec B}{\partial t} \tag{3}
\end{gather}$$
## ampere's law
$$\begin{gather}
\oint_{C} \vec B \cdot d\vec l = \iint_{S} (\vec\nabla \times \vec B) \cdot d\vec S = \mu_{0} \iint_{S} \vec J \cdot d\vec S \\
\iint_{S} (\vec\nabla \times \vec B - \mu_{0}\vec J)\cdot d\vec S = 0\\
\vec\nabla\times \vec B = \mu_{0}\vec J
\end{gather}$$
- this is almost, but not quite the fourth equation
### ampere-maxwell law
$$\vec\nabla \cdot (\vec\nabla\times\vec B) = \mu_{0}\vec\nabla\cdot\vec J$$
- note: $\vec\nabla\cdot(\vec\nabla \times \vec v) = 0$
$$\implies \vec\nabla \cdot (\vec\nabla\times\vec B) = 0$$
- but the $RHS:$
$$\mu_{0} \vec\nabla\cdot\vec J = - \mu_{0} \frac{\partial \rho}{\partial t}$$
- from the [[content/012/PX284 - SMETO/part 2 - electromagnetic theory/O - introduction to EMT/PX284 - O3 - charge#conservation of charge\|continuity equation]]:
$$\vec\nabla\cdot(\vec\nabla \times \vec B) = 0 = \mu_{0} \left( \vec\nabla\cdot\vec J + \frac{\partial \rho}{\partial t}\right)$$
- this was maxwell's solution
- so, ampere's law is modified to:
$$\vec\nabla \times \vec B = \mu_{0} \left( \vec J  + \varepsilon_{0} \frac{\partial \vec E}{\partial t}\right) \tag{4}$$
- this is called **the ampere-maxwell equation**
- the added term is historically called the **displacement current density**

- checking:
$$\begin{align*}
\vec\nabla\cdot (\vec\nabla \times \vec B) &= 0 \\
&= \mu_{0} \left( \vec\nabla\cdot\vec J + \varepsilon_{0}\frac{\partial }{\partial t}(\vec\nabla\cdot\vec E) \right) \\
&= \mu_{0} \left( \vec\nabla\cdot\vec J + \varepsilon_{0}\frac{\partial }{\partial t} (\rho/\varepsilon_{0})\right)\\
&= \mu_{0}\left(\vec\nabla\cdot\vec J + \frac{\partial \rho}{\partial t}\right)
\end{align*}$$

- the reason this was not discovered earlier is because ampere's law alone is a good quasi-static approximation, as the additional term, $\bigg|\varepsilon_{0} \cfrac{\partial \vec E}{\partial t} \bigg| \ll |\vec J|$
### parallel-plate capacitor
-  considering a parallel-plate capacitor
- current flow will build up opposite charges on each plate
- an electric field is generated between the plates
- considering a closed loop around the connecting wire:
$$\oint_{C}\vec B \cdot d\vec l = \iint_{S_{1}} (\vec\nabla \times \vec B) \cdot d\vec S = \iint_{S_{2}} (\vec\nabla \times \vec B) \cdot d\vec S$$
	where, $S_{2}$ goes around a plate of the capacitor, but not $S_{1}$

$$\iint_{S_{1}} \mu_{0} \left(\vec J + \varepsilon_{0} \frac{\partial \vec E}{\partial t}\right) = \iint_{S_{1}} \mu_{0} \left(\vec J + \varepsilon_{0} \frac{\partial \vec E}{\partial t}\right)$$
- for ${} LHS$, ${} \cfrac{\partial \vec E}{\partial t} = 0 {}$
- for $RHS$, $\vec J = 0$
- for a parallel-plate capacitor:
$$\begin{gather}
|\vec E| = \frac{\sigma}{\varepsilon_{0}} = \frac{Q}{A\varepsilon_{0}} \\
\frac{\partial E}{\partial t} = \frac{1}{A\varepsilon_{0}}\frac{\partial Q}{\partial t} = \frac{I}{A\varepsilon_{0}}  \\\\
\implies \iint_{S_{1}} \mu_{0}\vec J \cdot d\vec S = \mu_{0}I \\
\implies \iint_{S_{2}} \mu_{0} \frac{\partial \vec E}{\partial t}  \cdot d\vec S = \mu_{0}I 
\end{gather}$$
