# Physics 220 Homework 3
## Problem 1.18
## Problem 1.21
## Problem 1.23
The dispersion of the position wave function is $$ \begin{align}
\left< \left( \Delta x \right) ^2 \right> &= \left< x^2 \right> - \left< x \right> ^2 = \int_{0}^{a} \psi^\star (x) x^2 \psi (x) \, dx - \left( \int_{0}^{a} \psi^\star (x) x \psi (x) \, dx  \right) ^2  \\
&= \frac{2}{a} \int_{0}^{a} x^2 \sin ^2 \left( \frac{n\pi x}{a} \right)  \, dx - \left( \frac{2}{a} \int_{0}^{a} x \sin^2 \left( \frac{n\pi x}{a} \right)  \, dx  \right) ^2 \\
&= \frac{4\pi^2 n^2 a^2 - 6a^2}{12\pi^2 n^2} - \frac{a^2}{4} \end{align} $$
The dispersion of the momentum wave function is $$ \begin{align}
\left< ( \Delta p) ^2 \right> &= \left< p^2 \right> - \left< p \right> ^2  \\ &= \hbar^2 \frac{2}{a} \left( \frac{n\pi}{a} \right) ^2 \int_{0}^{a} \sin^2 \left( \frac{n\pi x}{a} \right) \, dx - 0^2 = \left( \frac{n\pi \hbar}{a} \right) ^2  
\end{align}$$
Taking the product of the dispersions, $$ \begin{align}
\left<  \left( \Delta x \right) ^2 \right> \left< \left( \Delta p \right) ^2 \right> &= \left( \frac{4 \pi^2 n^2 - 6}{12} - \frac{n^2 \pi^2}{4} \right) \hbar^2  \\
&= \left( \frac{\pi^2 n^2 -6}{12} \right) \geq \frac{1}{4} \implies n^2 \geq \frac{9}{\pi^2} \implies n \geq \frac{3}{\pi}
\end{align} $$
## Problem 1.25
(a) Operator $\hat{A}$ exhibits a degenerate spectrum as, out of the three eigenvalues it has, two of them are $-a$. Determining the eigenvalues of $\hat{B}$, $$\det \left( \hat{B} - \lambda \hat{I} \right) = \begin{vmatrix}
-\lambda & 0 & 0 \\
0 & -b-\lambda & -ib  \\
0 & ib & -b-\lambda 
\end{vmatrix} = \left( b-\lambda \right) \begin{vmatrix}
-\lambda & -ib  \\
ib & -\lambda
\end{vmatrix} = -(\lambda-b) (\lambda + b) (\lambda - b) = 0$$
From the characteristic polynomial, it is clear that the polynomial has degenerate roots, and therefore $\hat{B}$ has a degenerate spectrum.

(b) $\left[ \hat{A}, \hat{B} \right]= \hat{A}\hat{B} - \hat{B}\hat{A}$, which computes to $$\begin{align}&\begin{pmatrix}
a & 0 & 0 \\
0 & -a & 0  \\
0 & 0 & -a
\end{pmatrix} \begin{pmatrix}
b & 0 & 0  \\
0 & 0 &  -ib  \\
0 & ib & 0
\end{pmatrix} - \begin{pmatrix}
b & 0 & 0  \\
0 & 0 &  -ib  \\
0 & ib & 0
\end{pmatrix} \begin{pmatrix}
a & 0 & 0 \\
0 & -a & 0  \\
0 & 0 & -a
\end{pmatrix}  \\
&= \begin{pmatrix}
ab & 0 & 0  \\
0 & 0 & iab  \\
0 & -iab & 0
\end{pmatrix} - \begin{pmatrix}
ab & 0 & 0  \\
0 & 0 & iab  \\
0 & -iab & 0
\end{pmatrix} = \vec{0} \end{align}$$
(c) 

## Problem 1.30