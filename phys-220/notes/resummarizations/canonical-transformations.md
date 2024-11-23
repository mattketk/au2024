# Canonical Transformations
- Motivated by finding a set of coordinates which are convenient for a system/problem
- Point transformation of configuration space: $$Q_{i} = Q_{i} (q, t)$$
- Point transformation of phase space: $$Q_{i} (q, p, t)$$ $$P_{i}(q,p,t)$$
- We demand a transformation $K(Q,P,t)$ that accepts a $Q, P$ as canonical coordinates $$\dot{Q}_{i} = \frac{ \partial K }{ \partial P_{i} } $$ $$\dot{P}_{i} = - \frac{ \partial K }{ \partial Q_{i} } $$
- $Q,P$ must also satisfy $$\delta \int_{t_{1}}^{t_{2}} \left( P_{i}Q_{i} - K (Q, P, t) \right)  \, dt = 0 $$
- The statement is satisfied if the relations are connected by a relation of the form $$\lambda \left( p_{i}\dot{q}_{i} - H \right) = P_{i} \dot{Q}_{i} - K + \frac{dF}{dt}$$
	- $F$ is a function of phase space coords. with continuous second derivatives
	- $\lambda$ is a constant independent of $Q,P,t$
- **A canonical transformation is thus when** $\lambda=1$ $$p_{i} q_{i} - H = P_{i} \dot{Q}_{i} - K + \frac{dF}{dt}$$
- *Restricted* canonical transformations have no explicit time dependence
## Other Conditions for Canonical Transforms
- Poisson Brackets
	- The following must be satisfied for $Q(q,p), P(q,p)$
		- $$\left\{ Q_{i}, P_{j} \right\} = \delta_{ij}$$ $$\left\{ Q_{i}, Q_{j} \right\} = 0$$ $$\left\{ P_{i}, P_{j} \right\} = 0$$
- Matrix
	- $$\mathbf{M} \mathbf{J} \mathbf{M}^T = \mathbf{J}$$
## Generating Functions
- The $F$ in the canonical transformation equation
	- Vanishes at the end points if $F$ is a function of $q,p,t$ or $Q,P,t$ or a mix
	- specifies the equations of transformation
- Example $$F=F_{1} (q,Q,t)$$
- Table of generating functions ![[goldstein9-1_table.png]]