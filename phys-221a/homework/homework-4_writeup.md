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
(a) ![[Sakurai-2-3a.JPG]]
(a) and (b) ![[Sakurai-2-3b.JPG]]
(c) ![[Sakurai-2-3c.JPG]]
## Sakurai 2.6
$$\begin{align}\left[ H,x \right]& = \frac{1}{2m} \left[ p^2,x \right] + \left[ V(x), x \right] \\
&= -\frac{1}{2m} \left[ x,p^2 \right]  \\
&= -i \hbar \frac{p}{m} \end{align}$$
$$\implies \left[ [H,x], x \right] = -\frac{i\hbar}{m} \left[ p, x \right] = -\frac{\hbar^2}{m}$$
$$\left[ \left[ H,x \right] ,x \right] = \left[ Hx, x \right] - \left[ x, Hx \right] = Hxx - xHx - xHx + xxH = Hxx -2xHx + xxH $$
$$\begin{align}\left< \left[ \left[ H,x \right] ,x \right]  \right> &= \bra{a''} Hxx \ket{a''} - 2 \bra{a''} xHx \ket{a''} + \bra{a''} xxH \ket{a''} \\
&=2E_{a''}\bra{a''} xx\ket{a''} -2 \bra{a''} xHx\ket{a''}
\end{align}$$
Using the completeness relation in the $\ket{a'}$ basis, $$\begin{align}&2E_{a''} \sum_{a'} \bra{a''} x\ket{a'} \bra{a'} x \ket{a''} - 2\sum_{a'}\bra{a''} x \ket{a'} \bra{a'} Hx \ket{a''} \\
&2E_{a''}\sum_{a'} \bra{a''} x\ket{a'} \bra{a'} x \ket{a''} - 2E_{a'} \sum_{a'} \bra{a''} x\ket{a'} \bra{a'} x \ket{a''}  \\
&= -2\sum_{a'} \bra{a''} x\ket{a'} \bra{a'} x \ket{a''} \left( E_{a'} - E_{a''} \right) = -\frac{\hbar^2}{m}  \end{align}$$
$$\therefore \sum_{a'} \left| \bra{a''} x \ket{a'}  \right| ^2 \left( E_{a'} - E_{a''} \right) = \frac{\hbar^2}{2m}$$
## Sakurai 2.7
Using the "Generalized Ehrenfest's theorem" (Griffiths 3.73), which states that $$\frac{d}{dt} \left< \hat{Q} \right> = \frac{i}{\hbar} \left< \left[ \hat{Q}, \hat{H} \right] \right> + \left< \frac{\partial \hat{Q}}{\partial t} \right> $$
Let $\hat{Q} = \hat{x} \cdot \hat{p}$, $$\frac{d}{dt} \left< \hat{x} \cdot \hat{p} \right> = \frac{i}{\hbar} \left< \left[ \hat{x} \cdot \hat{p}, \hat{H} \right] \right> + \left< \frac{\partial \hat{x}}{\partial t} \cdot \hat{p} + \frac{\partial \hat{p}}{\partial t} \cdot \hat{x} \right>$$
The second term on the right-hand side of the equation vanishes because neither $\hat{x}$ nor $\hat{p}$ have explicit time dependence. Expanding the first term on the right-hand side, $$ \frac{d}{dt} \left< \hat{x} \cdot \hat{p} \right> = \frac{i}{\hbar} \left< \left( \hat{x} \cdot \hat{p} \right) \hat{H} - \hat{H}(\hat{x}\cdot \hat{p}) \right> = \frac{i}{\hbar} \left[ \bra{\psi} \left( \hat{x}\cdot \hat{p} \right) \hat{H}\ket{\psi} - \bra{\psi} \hat{H} \left( \hat{x} \cdot \hat{p} \right) \ket{\psi} \right] $$
Let $\ket{\psi}$ be a stationary state, such that $\hat{H} \ket{\psi}= E\ket{\psi}$. The equation becomes $$\frac{d}{dt} \left< \hat{x} \cdot \hat{p} \right> = \frac{i}{\hbar} \left[ E\bra{\psi} \left( \hat{x}\cdot \hat{p} \right) \ket{\psi} - E\bra{\psi} \left( \hat{x} \cdot \hat{p} \right) \ket{\psi} \right] = 0$$
Thus, when the quantum state is stationary, the total time derivative $\frac{d}{dt} \left< \hat{x} \cdot \hat{p} \right>$ goes to zero, the virial theorem applies.
## Sakurai 2.11
(a) The Hamiltonian in matrix form is $$\hat{H} = \begin{pmatrix}
0 & \Delta \\
\Delta & 0
\end{pmatrix}$$ The following eigenvalues are $\lambda = \pm \Delta$
- For $\lambda_{1} = \Delta$, $\ket{\lambda_{1}} = \frac{1}{\sqrt{ 2 }} \begin{pmatrix}1\\1\end{pmatrix}$
- For $\lambda_{2} = -\Delta$, $\ket{\lambda_{2}} = \frac{1}{\sqrt{ 2 }} \begin{pmatrix}1\\-1\end{pmatrix}$

(b) Expressing the base kets $\ket{R}, \ket{L}$ in terms of the Hamiltonian eigenstates,
$$\begin{align}
\ket{R} = \frac{1}{\sqrt{ 2 }} \left( \ket{\lambda_{1}} -\ket{\lambda_{2}}  \right) \\ \\
\ket{L} = \frac{1}{\sqrt{ 2 }} \left( \ket{\lambda_{1}} + \ket{\lambda_{2}}  \right) 
\end{align}$$
Applying the time evolution operator to each of these results in $$\begin{align}
U(t) \ket{R} = \frac{1}{\sqrt{ 2 }} \left( \exp \left( -i\Delta t /\hbar \right) \ket{ \lambda_{1}} - \exp \left( +i \Delta t /\hbar \right) \ket{\lambda_{2}}  \right)  \\
U(t) \ket{L} = \frac{1}{\sqrt{ 2 }} \left( \exp \left( -i\Delta t /\hbar \right) \ket{ \lambda_{1}} + \exp \left( +i \Delta t /\hbar \right) \ket{\lambda_{2}}  \right)\end{align}$$
Re-expressing the basis, $$\begin{align}
U(t) \ket{R} &= \cos \left( \Delta t / \hbar \right) \ket{R} - i\sin \left( \Delta t / \hbar \right) \ket{L}  \\
U(t) \ket{L} &= \cos \left( \Delta t /\hbar \right) \ket{L}  - i \sin \left( \Delta t / \hbar \right) \ket{R}  
\end{align}$$
Therefore, $\ket{\alpha; t}$ evaluates to $$\begin{align} \\
\ket{\alpha;t}&=\bra{R} \ket{\alpha} \left( \cos \left( \Delta t / \hbar \right) \ket{R} - i\sin \left( \Delta t / \hbar \right) \ket{L} \right)  \\
&+ \bra{L} \ket{\alpha} \left( \cos \left( \Delta t /\hbar \right) \ket{L}  - i \sin \left( \Delta t / \hbar \right) \ket{R} \right) \\
\end{align}$$

(c) Let $R_{\alpha} = \bra{R} \ket{\alpha}, L_{\alpha} = \bra{R} \ket{\alpha}$$$ \begin{align} \\
\left| \bra{R} \ket{\alpha;t}   \right| ^2 &= \left| R_{\alpha} \cos \left( \Delta t /\hbar \right) - i L_{\alpha} \cos \left( \Delta t /\hbar \right) \right|^2 \\
&=R_{\alpha}^2 \cos^2 \left( \frac{\Delta t}{\hbar} \right) + L_{\alpha}^2 \sin^2 \left( \frac{\Delta t}{\hbar} \right) \end{align} $$
If the particle is found in the state $\ket{R}$ with certainty at $t=0$, then there is no chance that $\ket{L}$ is measured.

(d) $$\begin{align} \\
a_{R} (t) = \bra{R } \ket{\alpha ; t}  = R_{\alpha} \cos \left( \frac{\Delta t}{\hbar} \right)  - i L_{\alpha} \sin \left( \frac{\Delta t}{\hbar} \right) \\ \\
a_{L} (t) = \bra{L} \ket{\alpha;t} = L_{\alpha} \cos\left( \frac{\Delta t}{\hbar} \right)- i R_{\alpha} \sin \left( \frac{\Delta t}{\hbar} \right) 
\end{align}$$
$$i\hbar \frac{\partial}{\partial t} a_{R} (t) = \Delta a_{L} (t)$$

$$i\hbar \frac{\partial}{\partial t} a_{L} (t) = \Delta a_{R} (t)$$
$$\implies -\frac{\hbar^2}{\Delta} \frac{\partial^{2}}{\partial t^2} a_{R} (t) = \Delta a_{R}(t)$$
$$\implies -\frac{\hbar^2}{\Delta} \frac{\partial^{2}}{\partial t^2} a_{L} (t) = \Delta a_{L}(t)$$

(e) Suppose the Hamiltonian is $$H = \Delta \ket{L} \bra{R} $$, the time evolution operator becomes $$U = 1- \frac{it\Delta}{\hbar} \ket{L} \bra{R} $$
The time-evolving state $U(t) \ket{\alpha} = \ket{\alpha ; t}$ becomes $$\ket{\alpha;t} = R_{\alpha}\left( 1- i t \Delta /  \hbar\right) \ket{L} + L_{\alpha}\ket{L}   $$
To test probability conservation, $$\left| \bra{R} \ket{\alpha;t}  \right| ^2 + \left| \bra{L} \ket{\alpha;t}  \right|^2 = 1$$
however, $$\left| \bra{L} \ket{\alpha;t}  \right| ^2 + \left| \bra{R} \ket{\alpha;t}  \right| ^2 = \left| L_{\alpha} + R_{\alpha} - R_{\alpha} it \Delta /\hbar \right|^2 + \left| \bra{R} \ket{\alpha;t}  \right| ^2 \neq 1 $$