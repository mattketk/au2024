# Physics 220 Homework Writeup
## Problem 1
(a) We note that the volume element of the transformed phase space is $$d^n x^\prime = \left| \mathbf{J} \right|  d^n x = \prod_{i} dx_{i}^\prime$$
For each differential, to first order $$\begin{align} dx_{i}^{\prime} &= dx_{i} + \left( v_{i} (x_{i} + dx_{i}) - v_{i} (x_{i}) \right) dt  \\
&= dx_{i} + \left( v_{i} (x_{i}) + \frac{ \partial v_{i} (x_{i}) }{ \partial x_{i} } dx_{i}  - v_{i} (x_{i})\right) dt = dx_{i}+ \frac{ \partial v_{i} }{ \partial x_{x} } dx_{i} dt  \\
&=  dx_{i} \left( 1+\frac{ \partial v_{i} }{ \partial x_{i} } dt \right)
\end{align} $$
Multiplying each differential together, $$\prod_{i} dx_{i}^\prime = \prod_{i} dx_{i} \left( 1+ \frac{ \partial v_{i} (x_{i}) }{ \partial x_{i} } dt \right) $$
Neglecting terms with $dt^n$ with $n \geq 2$, $$\prod_{i} dx_{i}^\prime \to \prod_{i}dx_{i} + \sum_{i} \frac{ \partial v_{i} }{ \partial x_{i} } dx_{i} dt = \left| \mathbf{J} \right| \prod_{i} dx_{i}  $$
Since $\sum_{i}\frac{ \partial v_{i} }{ \partial x_{i} } = 0$, the determinant of $\mathbf{J}$ must be 1. Therefore, the transformation preserves canonical volume.
(b)
## Problem 2
## Problem 3
## Problem 4
