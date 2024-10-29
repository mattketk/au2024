# Physics 221A Homework 4
## Sakurai 2.1
## Hints
- Look at Heisenberg picture section in Sakurai
- Heisenberg EoM $$\frac{dA^{(H)}}{dt}= \frac{1}{i\hbar} \left[ A^{(H)}, H \right] $$
	- where $A^{(H)} = \mathcal{U}^{\dagger} (t) A^{(S)} \mathcal{U} (t)$ and $\mathcal{U} (t) = \exp \left( -\frac{iHt}{\hbar} \right)$
The time evolution operators evaluate to $$\mathcal{U}(t) = \exp \left( -\frac{i\hat{H} t}{\hbar} \right) = \sum_{n=0}^\infty \left( -\frac{i\hbar \omega}{2\hbar} \right)^n \frac{1}{n!} \begin{pmatrix}
1 & 0 \\
0 & -1
\end{pmatrix}^{n}= \begin{pmatrix}
\exp \left( -\frac{i\omega t}{2} \right) & 0 \\
0 & \exp \left( \frac{i\omega t}{2} \right) 
\end{pmatrix} $$
The operator is unitary, so that $$\mathcal{U}^{\dagger} (t) = \begin{pmatrix}
\exp \left( \frac{i\omega t}{2} \right)  & 0 \\
0 & \exp \left( -\frac{i\omega t}{2} \right)
\end{pmatrix}$$
As a shorthand, let $e-$ denote $\exp(-i \omega t /2)$ and $e+$ denote $\exp \left( i \omega t / 2 \right)$. 

For $S_{z}^{(H)}$, $$S_{z}^{(H)} (t) = \frac{\hbar \omega}{2} \begin{pmatrix}
e+ & 0 \\
0 & e-
\end{pmatrix} \begin{pmatrix}
1 & 0  \\
0 & -1
\end{pmatrix} \begin{pmatrix}
e- & 0 \\
0 & e+
\end{pmatrix}= \frac{\hbar \omega}{2} \begin{pmatrix}
1 & 0 \\
0 & -1
\end{pmatrix} = S_{z}^{(S)}$$
Therefore, $S_{z}$ is time independent (under this Hamiltonian).

For $S_{x}^{(H)}$, $$S_{x}^{(H)} (t) = \frac{\hbar \omega}{2} \begin{pmatrix}
e+ & 0 \\
0 & e-
\end{pmatrix} \begin{pmatrix}
0 & 1  \\
1 & 0
\end{pmatrix} \begin{pmatrix}
e- & 0 \\
0 & e+
\end{pmatrix}= \frac{\hbar \omega}{2} \begin{pmatrix}
0 & \exp \left( i\omega t \right)  \\
\exp \left( -i \omega t \right) & 0
\end{pmatrix}$$
For $S_{z}^{(H)}$, $$S_{y}^{(H)} (t) = \frac{\hbar \omega}{2} \begin{pmatrix}
e+ & 0 \\
0 & e-
\end{pmatrix} \begin{pmatrix}
0 & -i  \\
i & 0
\end{pmatrix} \begin{pmatrix}
e- & 0 \\
0 & e+
\end{pmatrix}= \frac{\hbar \omega}{2} \begin{pmatrix}
0 & -i\exp \left( i\omega t \right)  \\
i\exp \left( -i \omega t \right) & 0
\end{pmatrix}$$
## Sakurai 2.3

## Sakurai 2.6
### Hints
$$\left[ \left[ H, x \right], x \right] = \dots -\frac{1}{m} $$
$$\bra{a''} -\frac{1}{2}\left[ \left[ H, x \right] , x \right] \ket{a''} = \frac{1}{2m}$$
## Sakurai 2.7
Using the "Generalized Ehrenfest's theorem" (Griffiths 3.73), which states that $$\frac{d}{dt} \left< \hat{Q} \right> = \frac{i}{\hbar} \left< \left[ \hat{Q}, \hat{H} \right] \right> + \left< \frac{\partial \hat{Q}}{\partial t} \right> $$
Let $\hat{Q} = \hat{x} \cdot \hat{p}$, $$\frac{d}{dt} \left< \hat{x} \cdot \hat{p} \right> = \frac{i}{\hbar} \left< \left[ \hat{x} \cdot \hat{p}, \hat{H} \right] \right> + \left< \frac{\partial \hat{x}}{\partial t} \cdot \hat{p} + \frac{\partial \hat{p}}{\partial t} \cdot \hat{x} \right>$$
The second term on the right-hand side of the equation vanishes because neither $\hat{x}$ nor $\hat{p}$ have explicit time dependence. Expanding the first term on the right-hand side, $$ \frac{d}{dt} \left< \hat{x} \cdot \hat{p} \right> = \frac{i}{\hbar} \left< \left( \hat{x} \cdot \hat{p} \right) \hat{H} - \hat{H}(\hat{x}\cdot \hat{p}) \right> = \frac{i}{\hbar} \left[ \bra{\psi} \left( \hat{x}\cdot \hat{p} \right) \hat{H}\ket{\psi} - \bra{\psi} \hat{H} \left( \hat{x} \cdot \hat{p} \right) \ket{\psi} \right] $$
Let $\ket{\psi}$ be a stationary state, such that $\hat{H} \ket{\psi}= E\ket{\psi}$. The equation becomes $$\frac{d}{dt} \left< \hat{x} \cdot \hat{p} \right> = \frac{i}{\hbar} \left[ E\bra{\psi} \left( \hat{x}\cdot \hat{p} \right) \ket{\psi} - E\bra{\psi} \left( \hat{x} \cdot \hat{p} \right) \ket{\psi} \right] = 0$$
Thus, when the quantum state is stationary, the total time derivative $\frac{d}{dt} \left< \hat{x} \cdot \hat{p} \right>$ goes to zero, the virial theorem applies.
## Sakurai 2.11
