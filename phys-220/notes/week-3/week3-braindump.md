# Week 3 PHYS 220 braindump
- Poisson bracket need-to-know
	- Definition $$\left[ u, v \right] _{q,p} = \frac{ \partial u }{ \partial q_{i} } \frac{ \partial v }{ \partial p_{i} } - \frac{ \partial u }{ \partial p_{i} } \frac{ \partial v }{ \partial q_{i} } $$
- Hamiltonian state vector $$\mathbf{\eta} = \begin{pmatrix}q_{1} \\ \vdots \\ q_{N} \\ p_{1} \\ \vdots \\ p_{N}\end{pmatrix}$$
- J matrix $$\mathbf{J} = \begin{bmatrix}
\mathbf{0} & \mathbf{I} \\ -\mathbf{I} & \mathbf{0}
\end{bmatrix}$$
	- Orthogonal matrix: $\mathbf{JJ^T} = \mathbf{I}$
- Compact form of Hamilton's equations $$\dot{\mathbf{\eta}} = \mathbf{J} \frac{ \partial H }{ \partial \mathbf{\eta} } $$