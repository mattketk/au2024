# Lagrangians and the principle of least action
- $$S \left[ q(t) \right] = \int_{t_{1}}^{t_{2}} L \left( q, \dot{q}, t \right)  \, dt $$
- path $q(t)$ maps to a real number quantity called the action
- given two endpoints contained within $q(t)$, there is a $q(t)$ which is an **extremum** of the action
## Euler-Lagrange Equation
$$\frac{ \partial L }{ \partial q } - \frac{\partial}{\partial t} \left( \frac{ \partial L }{ \partial \dot{q} }  \right) = 0$$
- Take the same form in all coordinate systems
	- coordinate system must be invertible such that $$J_{ij} = \frac{\partial r_{i}}{\partial q_{j}}$$ $$\det \left( \mathbf{J} \right) \neq 0$$
	- coordinate systems can have "inconsistent units" $$(r, \theta, \phi)$$
## Constraints
- For $s$ constraints, introduce $s$ variables with indices $j=1,\dots,s$
- Add terms to the Lagrangian $$L_{i}=T_{i}-V_{i} + \sum_{j=1}^{\infty} \lambda_{j} \phi_{j}$$
	- Function $\phi_{j}$ is equal to 0 if constraint is satisfied and $\infty$ if not
		- works only for holonomic constraints
	- $\lambda_{j}$ assumed to be only a function of time (see Goldstein eq 2.27)
- Euler-Lagrange Equation $$\frac{ \partial L }{ \partial q_{i} } - \frac{d}{dt} \left( \frac{ \partial L }{ \partial \dot{q_{i}} }  \right) +\sum_{j} \lambda_{j}\frac{\partial \phi_{j}}{\partial q_{i}} =0 $$