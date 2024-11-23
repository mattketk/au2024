# Special Relativity notes from Geometric Algebra
$$\left( ct \right) ^2 - r^2 = \left( ct' \right) ^{2} - \left( r' \right) ^2 = 0$$
- Defining four orthogonal vectors $\left\{ \gamma_{0}, \gamma_{1}, \gamma_{2}, \gamma_{3} \right\}$ where 
	- $\gamma_{0}^2=1$
	- $\gamma_{0}\cdot \gamma_{i} = 0$
	- $\gamma_{i} \cdot \gamma_{j} = -\delta_{ij}$
	- which form the Minkowski metric where 
	- $$\gamma_{\mu}\cdot\gamma_{\nu} = \eta_{\mu \nu} = \begin{pmatrix}
1 & 0 & 0 & 0 \\
0 & -1 & 0 & 0  \\
0 & 0 & -1 & 0 \\
0 & 0 & 0 & -1
\end{pmatrix}$$
- Pseudoscalar 
	- $$I = \gamma_{0}\gamma_{1}\gamma_{2}\gamma_{3}$$
	- Its reverse $$\tilde{I} = \gamma_{3}\gamma_{2}\gamma_{1}\gamma_{0} = I$$
	- $\tilde{I}I = -1$
- Spacetime paths
	- Let $x(\lambda)$ be a curve in spacetime where $\lambda$ is some monotonically-increasing parameter $$x' = \frac{dx \left( \lambda \right) }{d\lambda}$$ $$\frac{dx}{d\tau}= \frac{d\lambda}{d\tau} \frac{dx}{d\lambda}$$
	- $\tau$ is proper time: the time measured by a clock along its own worldline
- Lorentz Transform $$\begin{pmatrix}
x' \\
ct'
\end{pmatrix} = \begin{pmatrix}
\gamma & -\gamma\beta \\
\gamma\beta & \gamma
\end{pmatrix} \begin{pmatrix}
x \\
ct
\end{pmatrix}$$