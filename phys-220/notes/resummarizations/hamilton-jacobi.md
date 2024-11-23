# Hamilton Jacobi Theory
- Consider coordinate transformation as a function of time and initial coordinates $Q \left( q_{0}, p_{0}, t \right),\, P \left( q_{0}, p_{0}, t \right)$ such that the new coordinates are constant in time $$\begin{align}
\frac{ \partial K }{ \partial P_{i} } = \dot{Q}_{i} = 0  \\
-\frac{ \partial K }{ \partial Q_{i} } = \dot{P}_{i} = 0  
\end{align}$$
- The new Hamiltonian $K$ is also equal to zero, which relates to the old Hamiltonian by the relation $$K=H+\frac{ \partial F }{ \partial t } = 0$$ where $F$ is a generating function which determines how the coordinates transform
- Forms a 1st order PDE of $n+1$ variables $(q_{1},\dots,q_{n}, t)$ $$H \left( q_{1},\dots, q_{n}; \frac{ \partial F_{2} }{ \partial q_{1} },\dots, \frac{ \partial F_{2} }{ \partial q_{n} } , t \right) + \frac{ \partial F_{2}}{ \partial t } = 0 $$