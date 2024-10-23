# Physics 220 Homework 3
## Problem 1.18
Consider $\ket{\phi}$ to be an eigenstate/ket of $\hat{A}\hat{B}$, $$\hat{A}\hat{B}\ket{\phi} =\lambda \ket{\phi} $$
This means $\left\{ \hat{A},\hat{B} \right\} \ket{\phi}=\hat{A}\hat{B}\ket{\phi}-\hat{B}\hat{A}\ket{\phi}=0$. Rearranging the equation, $$\hat{A}\hat{B} \ket{\phi}  = -\hat{B}\hat{A}\ket{\phi} = \lambda \ket{\phi} \implies \hat{B}\hat{A}\ket{\phi} = -\lambda \ket{\phi} $$
This suggests that switching the order of the operators yields the same eigenstate and eigenvalue magnitude but with the opposite sign.
## Problem 1.21
![[homework-3_121.pdf]]
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
$n$ must be an integer 1 or greater, so the inequality holds.
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
(c) The eigenvalue of $\hat{A}\hat{B}$ are, $$\det \left( \hat{A}\hat{B} - \lambda\hat{I} \right) = 0 \implies \begin{vmatrix}
ab & 0 & 0 \\
0 & 0 & iab \\
0 & -iab & 0
\end{vmatrix} = -(\lambda - ab) (\lambda + ab) (\lambda - ab) = 0$$
The characteristic polynomial has three roots, two of which are degenerate (i.e. $ab$). This means that each eigenstate cannot be distinguished solely by its corresponding eigenvalue, as the same eigenvalue may correspond to more than one eigenstate.
## Problem 1.30
(a) The classical Poisson bracket expression for $$\left\{ x, F(p_{x}) \right\}_{x,p_{x}} = \frac{ \partial x }{ \partial x } \frac{ \partial F(p_{x}) }{ \partial p_{x} } - \frac{ \partial F(p_{x}) }{ \partial x } \frac{ \partial x }{ \partial p_{x}} = \frac{ \partial F(p_{x})}{ \partial p_{x} }     $$ (b) The commutator of the operators $\hat{x}, \exp \left( i \hat{p}_{x} a / \hbar \right)$, where $$\exp \left( \frac{i\hat{p}_{x}a}{\hbar} \right) = \sum_{n=0}^\infty \frac{a^n}{n!} \frac{\partial^n}{\partial x^n}$$
The commutator evaluates to $$x \sum_{n=0}^\infty \frac{a^n}{n!}\frac{\partial^n}{\partial x^n}f(x) - \sum_{n=0}^\infty \frac{a^n}{n!} \frac{\partial^n}{\partial x ^n} \left[ x f(x) \right] $$
Applying Leibniz's product rule, where $$\frac{d^n}{dx^n} \left[ f(x)g(x) \right] = \sum_{k=0}^{n} \frac{n!}{k! (n-k)!} \frac{\partial ^ k}{\partial x^k} (x) \frac{\partial^{(n-k)} f(x)}{\partial x ^{(n-k)}} $$
The commutator expression further evaluates to $$x \sum_{n=0}^\infty \frac{a^n}{n!}\frac{\partial^n}{\partial x^n}f(x) - \sum_{n=0}^\infty a^n \left( \frac{x}{n!} f^{(n)} (x) + \frac{f^{(n-1)}(x)}{(n-1)!} \right) = -a \sum_{n^\prime=0}^\infty \frac{a^{n^\prime}}{n^\prime !} f^{(n)}(x) = -a \exp \left( \frac{ip_{x}a}{\hbar} \right) $$
(c) Applying the commutator to $\ket{x^\prime}$ as an operator evaluates to $$\left[ \hat{x}, \exp \left( \frac{i\hat{p}_{x}a}{\hbar} \right)  \right] \ket{x^\prime} = \left( \hat{x} \exp \left( \frac{i \hat{p}_{x}a}{\hbar} \right) - \exp \left( \frac{i \hat{p}_{x}a}{\hbar} \right) \hat{x} \right) \ket{x^\prime} = -a \exp \left( \frac{i p_{x} a}{\hbar} \right) \ket{x^\prime} $$
Rearranging the second term on the left-hand side of the equation, $$\hat{x} \exp \left( \frac{i \hat{p}_{x} a}{\hbar} \right) \ket{x^\prime} = (x-a) \exp \left( \frac{i \hat{p}_{x}a}{\hbar} \right) \ket{x^\prime} $$
The eigenvalue corresponding to the eigenstate is $x-a$.