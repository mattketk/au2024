# Physics 220 Homework 7 Writeup
## Problem 1
(a) We define the coordinate system to be located at the center of mass of the system (i.e. the center of the rod of length $L$) when the mass-rod system is at rest with respect to the lab frame. The center of mass of the frame will have the position $(x,y)$. Additionally, the angle with respect to the vertical the rod makes will be $\phi$. The masses on the ends of the rods will then be $$\begin{align}
x_{1}&=x-\frac{L}{2}\sin \phi \\
x_{2}&=x+\frac{L}{2}\sin \phi \\
y_{1}&=y-\frac{L}{2}\cos \phi \\
y_{2}&=y+\frac{L}{2}\cos \phi
\end{align}$$
Its time derivatives are as follows, $$\begin{align}
\dot{x}_{1}&=\dot{x}-\frac{L}{2}\dot{\phi}\cos \phi \\
\dot{x}_{2}&=\dot{x}+\frac{L}{2}\dot{\phi}\cos \phi \\
\dot{y}_{1}&=\dot{y}+\frac{L}{2}\dot{\phi}\sin \phi \\
\dot{y}_{2}&=\dot{y}-\frac{L}{2}\dot{\phi}\sin \phi
\end{align}$$
The Lagrangian is $$\mathcal{L}=\frac{1}{2}m\left(\dot{x}_{1}^2+\dot{x}_{2}^2+\dot{y}_{1}^2+\dot{y}_{2}^2\right)-\frac{1}{2}k \left(y_{1}^2+y_{2}^2 \right)$$
Substituting these terms and simplifying we get a Lagrangian of the form $$\mathcal{L}= \frac{mL^2}{4} \dot{\phi}^2 + m(\dot{x}^2+\dot{y}^2) - \frac{kL^2}{4}\cos^2 \phi - ky^2$$To linearize the $\phi$-dependent potential term, we utilize a small angle approximation where $\cos^2 \phi \approx \left( 1- \phi^2 / 2 \right)^{2} \approx 1- \phi^2$ (we can neglect the 1 as constant terms in a Lagrangian do not change the motion of the system). We can also neglect the potential along the $x$ direction since its contribution is a fourth order contribution. $$\begin{align}
\mathcal{L}= \frac{m}{2} \left( \frac{L^2\dot{\phi}^2}{2}+ 2(\dot{x}^2+\dot{y}^2)\right)- \frac{k}{2}\left(-\frac{L^2}{2}\phi^2 + 2y^2 \right)
\end{align}$$
(c)
![[homework-7_1c.pdf]]
(d) The characteristic frequencies should increase with increasing the spring constants.
## Problem 2
![[homework-7_2d.pdf#page=1]]
![[homework-7_2d.pdf#page=2]]
![[homework-7_2d.pdf#page=3]]
## Problem 3
We define a coordinate for each mass, both measured from the ceiling of the system, $x_{1}, x_{2}$. As a result, the Lagrangian becomes $$\begin{align} \\
\mathcal{L}&=\frac{m}{2} \left( \dot{x}_{1}^2 +\dot{x}_{2}^2 \right) - \frac{k}{2} \left( x_{1}^2 + (x_{2}-x_{1})^2 \right) \\
&=\frac{m}{2} \left( \dot{x}_{1}^2 +\dot{x}_{2}^2 \right) - \frac{k}{2} \left( 2x_{1}^2 + x_{2}^2 - 2x_{1}x_{2}\right) 
\end{align}$$
The Hessian $\mathbf{M}, \mathbf{V}$ become $$\begin{align}
\mathbf{M} &= \begin{pmatrix}
1 & 0 \\
0 & 1
\end{pmatrix} \\
\mathbf{V} &= \begin{pmatrix}
2 & -1 \\
-1 & 1
\end{pmatrix}
\end{align}$$

Finding the eigenvalues with $\det \left( \mathbf{M}^{-1} \mathbf{V} - \lambda \mathbf{I} \right) = 0$, we get $$\lambda=\frac{1}{2}(3\pm \sqrt{ 5 })$$, and the following eigenvectors, $$\begin{align}
\lambda_{1} = \frac{1}{2} (3+\sqrt{ 17 }) &\to \vec{\gamma}_{1} = \begin{pmatrix}
\frac{-1-\sqrt{ 5 }}{2} \\
1
\end{pmatrix} \\
\lambda_{2} = \frac{1}{2} (3-\sqrt{ 17 }) &\to \vec{\gamma}_{2} = \begin{pmatrix}
\frac{-1+\sqrt{ 5 }}{2} \\
1
\end{pmatrix}
\end{align}$$
The ratios of the amplitudes are $\frac{-1-\sqrt{ 5 }}{2}, \frac{-1+\sqrt{ 5 }}{2}$
## Problem 4
The Lagrangian of the system is $$\mathcal{L}=T-V=\frac{m\dot{x}^2}{2}- \left( \frac{m\omega^{2}x^2}{2}+\frac{\lambda \cos \left( \gamma t \right) x^3}{3} \right) $$
which leads to the equation of motion of $$\ddot{x}+\omega_{0}^2x + \frac{\lambda}{m}\cos \left( \gamma t \right) x^2 = 0$$
We recognize that $\lambda$ is a small parameter, so the 0th order solution of the perturbation expansion of $$x(t)=x_{0}(t) + \epsilon x_{1}(t)$$
obeys the ODE in which the term with $\lambda$ vanishes, $$\ddot{x}_{0}+\omega_{0}^2 x_{0} = 0 \implies x_{0} (t) = A\cos \left( \omega_{0} t \right)  $$
Comparing the 2nd and third terms of the original ODE, we get $$\omega_{0}^2 A \gg \frac{\lambda}{m}A^2$$
Rearranging, $$\epsilon=\frac{\lambda A}{m\omega_{0}^2} \ll 1$$
b) Solving the ODE to first order, we get $$\begin{align}
\ddot{x}_{1} + \omega_{0}^2 x_{1} &=-\frac{\lambda A}{m\omega_{0}^2}\left( \ddot{x}_{0}+\frac{\lambda}{m}\cos \left( \gamma t \right) x_{0}^2 + \omega_{0}^2 x_{0}  \right) \\
\ddot{x}_{1}+\omega_{0}^2 x_{1}&=-\frac{\lambda A}{m\omega_{0}^2} \left(\frac{\lambda}{m} \cos \left( \gamma t \right) \cos ^{2} \left( \omega_{0} t \right) \right) 
\end{align}$$
Solving this ODE, $$x_{1}(t) = - \frac{A^{3}\lambda^{2}}{m^{2}\omega_{0}^{2}}\cos \left( \gamma t \right) \cos ^{2}(\omega_{0}t)$$
We will let $c_{1}\equiv -\frac{A^{3}\lambda^{2}}{m^{2}\omega_{0}^{2}}$. Rearranging, $$\begin{align}
x_{1}(t) &= \frac{C}{2} \cos \left( \gamma t \right) \left[ \cos \left(2 \omega_{0} t \right) +1 \right] \\
&=\frac{C}{2}\left( \cos \left[\left( 2 \omega_{0}  + \gamma\right)t\right] + \cos \left[ \left( 2\omega_{0} - \gamma \right) t \right] \right) + \frac{C}{2} \cos \left( \gamma t \right) 
\end{align}$$
In the limit that $\gamma \gg \omega_{0}$, $2\omega_{0}\pm\gamma \approx \pm\gamma$, the correction then vanishes, $$x_{1}(t) = C \cos\gamma t$$
