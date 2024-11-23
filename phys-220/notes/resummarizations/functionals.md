# Functionals
## Introduction
- map a function to a real number
- ex. $$S \left[ q(t) \right] = \int L \left( q,\dot{q}, t \right) \, dt$$
## Taylor Expansion Analogy
- First variation $$\delta S = \int \frac{\delta S}{\delta q} \delta q \, dt$$
- Second variation $$\delta^2 S = \frac{1}{2}\int \frac{\delta^2 S}{\delta q^2} \delta q^2 \, dt$$
	- or, in a more generalized form, $$\delta ^2 S = \frac{1}{2} \int \frac{\delta^2 S}{\delta q (t) \delta q (t^\prime)} \delta q (t) \delta q(t^\prime) \, dt$$
- These variations are a continuous analog to the discrete Taylor expansions, 
	- first order, $$\sum_{i} \frac{\partial f}{\partial x_{i}} \delta x_{i}$$
	- second order, $$\sum_{i,j} \frac{\partial ^2 f}{\partial x_i \partial x_{j}} \delta x_{i} \delta x_{j}$$