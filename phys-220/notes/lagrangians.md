# Lagrangians and the principle of least action
- $$S \left[ q(t) \right] = \int_{t_{1}}^{t_{2}} L \left( q, \dot{q}, t \right)  \, dt $$
- path $q(t)$ maps to a real number quantity called the action
- given two endpoints contained within $q(t)$, there is a $q(t)$ which is an **extremum** of the action
## Euler-Lagrange Equation
$$\frac{ \partial L }{ \partial q } - \frac{\partial}{\partial t} \left( \frac{ \partial L }{ \partial \dot{q} }  \right) = 0$$
- Take the same form in all coordinate systems
	- coordinate system must be invertible such that $$J_{ij} = \frac{\partial r_{i}}{\partial q_{j}}$$ $$\det \left( \mathbf{J} \right) \neq 0$$
	- coordinate systems can have "inconsistent units" $$(r, \theta, \phi)$$