# Physics 220 Homework Writeup
## Problem 1
(a) We note that the volume element of the transformed phase space is $$d^n x^\prime = \left| \mathbf{J} \right|  d^n x = \prod_{i} dx_{i}^\prime$$
For each differential, to first order $$\begin{align} dx_{i}^{\prime} &= dx_{i} + \left( v_{i} (x_{i} + dx_{i}) - v_{i} (x_{i}) \right) dt  \\
&= dx_{i} + \left( v_{i} (x_{i}) + \frac{ \partial v_{i} (x_{i}) }{ \partial x_{i} } dx_{i}  - v_{i} (x_{i})\right) dt = dx_{i}+ \frac{ \partial v_{i} }{ \partial x_{x} } dx_{i} dt  \\
&=  dx_{i} \left( 1+\frac{ \partial v_{i} }{ \partial x_{i} } dt \right)
\end{align} $$
Multiplying each differential together, $$\prod_{i} dx_{i}^\prime = \prod_{i} dx_{i} \left( 1+ \frac{ \partial v_{i} (x_{i}) }{ \partial x_{i} } dt \right) $$
Neglecting terms with $dt^n$ with $n \geq 2$, $$\prod_{i} dx_{i}^\prime \to \prod_{i}dx_{i} + \sum_{i} \frac{ \partial v_{i} }{ \partial x_{i} } dx_{i} dt = \left| \mathbf{J} \right| \prod_{i} dx_{i}  $$
Since $\sum_{i}\frac{ \partial v_{i} }{ \partial x_{i} } = 0$, the determinant of $\mathbf{J}$ must be 1. Therefore, the transformation preserves canonical volume.
(b) Combining the two relations $$v_{i} = \sum_{j} J_{ij} \frac{\partial H}{\partial x_{j}}$$ $$\sum_{i} \frac{ \partial v_{i} }{ \partial x_{i} } = 0 $$
we get $$\sum_{ij} J_{ij} \frac{\partial^2 H}{\partial x_{i} \partial x_{j}} = 0$$
The symplectic matrix $\mathbf{J}$ takes on the following values $$J_{ij} = \begin{cases}
-1 \text{ if i=n+k, j=k} \\
+1 \text{ if i=k, j=n+k}  \\
0 \text{ otherwise}
\end{cases}$$
This makes the sum over $i,j$ evaluate to $$- \frac{\partial^2 H}{\partial x_{n+k} \partial x_{k}} + \frac{\partial^2 H}{\partial x_{k} \partial_{n+k}} = 0$$ The derivatives commute, so the result is zero. Therefore, $v_{i}$ is divergenceless if Hamilton's equations hold.
## Problem 2
(a) $$\left\{ L_{i}, K_{j} \right\} = \left\{ L_{i}, \frac{1}{m}\epsilon_{jkl}p_{k} L_{l} - \hat{r}_{j} \right\} = \frac{1}{m}\left\{L_{i, } \epsilon_{jkl}p_{k} L_{l}  \right\} - \left\{ L_{i} , \hat{r}_{j} \right\}   $$
$$=\frac{\epsilon_{jkl}}{m} \left(\left\{ L_{i}, p_{k} \right\}L_{l} + p_{k} \left\{ L_{i}, L_{l} \right\} \right) - \left\{ L_{i}, \frac{q_{j}}{\sqrt{ q_{a} q_{a} }} \right\}  $$
The individual brackets evaluate to
- $$\left\{ L_{i}, p_{k} \right\} = \epsilon_{ilm} \left\{ q_{l} p_{m}, p_{k} \right\} = \epsilon_{ikm} p_{m}$$
- $$\left\{ L_{i}, \frac{q_{j}}{\sqrt{ q_{a} q_{a} }} \right\} = \epsilon_{ilm} \left\{ q_{l} p_{m}, \frac{q_{j}}{\sqrt{ q_{a}q_{a} }}\right\} = \epsilon_{ilm} \frac{q_{l}}{\sqrt{ q_{a} q_{a} }} + \epsilon_{ilm} q_{l}q_{j} q_{m} \frac{1}{\left( q_{a}^2 \right) ^{3/2}} = \epsilon_{ilm} \frac{q_{l}}{\sqrt{ q_{a}q_{a} }}$$
Continuing,
$$\begin{align}\left\{ L_{i}, K_{j} \right\} &= \frac{\epsilon_{jkl}}{m} \left( \epsilon_{ikm} p_{m} L_{l} + \epsilon_{ilm} L_{m} p_{k} \right) +\epsilon_{ilm} \frac{q_{l}}{\sqrt{ q_{a}q_{a} }}  \\
&=\frac{1}{m} \left(\left( \delta_{lm}\delta_{ij} - \delta_{il}\delta_{jm} \right) L_{l} p_{m} - \left( \delta_{ij} \delta_{km} - \delta_{jm} \delta_{ki} \right) L_{m} p_{k}  \right)+ \dots  \\
&= \epsilon_{ijk} K_{k}
\end{align}$$
(b) 
## Problem 3

(a) The Lagrangian of a charged particle with mass $m$ and charge $e$ within a magnetic field $\mathbf{B}$ has the form $$L = \frac{m\dot{\mathbf{x}}^2}{2} + e\mathbf{A} \cdot\dot{\mathbf{x}} = \frac{\left( \mathbf{p} - e\mathbf{A} \right) ^2}{2m} + e \mathbf{A} \cdot \mathbf{\dot{x}}$$
The conjugate momentum of the particle is $$p_{i} = \frac{ \partial L }{ \partial \dot{x}_{i} } = m\dot{x}_{i} + eA_{i} $$
Rearranging the above result, $$m\dot{x}_{i} = p_{i} - eA_{i}$$
The Poisson bracket $\left\{ m\dot{x}_{i} , m \dot{x}_{j} \right\}$ evaluates to $$\begin{align}&=\sum_{k} \left[ \frac{ \partial (m\dot{x}_{i}) }{ \partial x_{k} } \frac{ \partial (m\dot{x}_{j}) }{ \partial p_{k} }    - \frac{ \partial (m\dot{x}_{i}) }{ \partial p_{k} } \frac{ \partial (m\dot{x}_{j}) }{ \partial x_{k} } \right] \\
&=\sum_{k} \left[ \frac{ \partial (p_{i} - eA_{i}) }{ \partial x_{k} } \frac{ \partial (p_{j} - eA_{j})}{ \partial p_{k} }    - \frac{ \partial (p_{i}-eA_{i}) }{ \partial p_{k} } \frac{ \partial (p_{j}-eA_{j}) }{ \partial x_{k} } \right] \\
&=\sum_{k} \left[ -e \frac{ \partial A_{i} }{ \partial x_{k} } \delta_{jk}- \left( -e \delta_{ik} \frac{ \partial A_{j} }{ \partial x_{k} }  \right)   \right] \\
&=-e \sum_{k} \left[ \frac{ \partial A_{i} }{ \partial x_{j} }  - \frac{ \partial A_{j} }{ \partial x_{i} }  \right] = -e \epsilon_{ijk}B_{k}  \end{align}$$
For $\left\{ m\dot{x}_{i}, x_{j} \right\}$, $$\sum_{k} \left[ \frac{\partial}{\partial x_{k}} \left( p_{i} - eA_{i} \right) \frac{\partial}{\partial p_{k}}x_{j} - \frac{\partial}{\partial p_{k}} \left( p_{i} - eA_{i} \right) \frac{\partial}{\partial x_{k}} x_{j} \right]$$
The first term in the sum vanishes due to the partial derivative of $x_{j}$ with respect to $p_{k}$, leaving $$\sum_{k} \left[ - \frac{\partial}{\partial p_{k}} \left( p_{i} - eA_{i} \right) \frac{\partial}{\partial x_{k}} x_{j} \right] = \sum_{k} \left[ -\delta_{ik} \delta_{jk} \right] = -\delta_{ij}$$
(b) The magnetic vector potential $A_{i}=0$ since the field is no longer divergenceless. Evaluating $\left\{ J,H \right\}$, $$ = \left\{ m\epsilon_{ijk}x_{i} \dot{x}_{j} - eg_{m} \hat{x}_{i}, \frac{m\dot{x}_{j}\dot{x}_{j}}{2} \right\} = \left\{ m\epsilon_{ijk}x_{i} \dot{x}_{j}, \frac{m\dot{x}_{j}\dot{x}_{j}}{2} \right\} - eg_{m} \left\{ \hat{x_{i}}, \frac{m\dot{x}_{j}\dot{x}_{j}}{2} \right\}  $$
The partial derivatives of $\hat{x}_{i}$ with respect to canonical position and momentum are zero. While the momentum derivative may be apparent by inspection, the spatial derivative evaluates to $$\frac{\partial \left( \hat{x}_{i} \right) }{\partial x_{k}} = \frac{\partial}{\partial x_{k}} \left( \frac{x_{i}}{\sqrt{ x_{k}x_{k} }} \right) = \frac{\delta_{ik} \sqrt{ x_{k} x_{k} } - x_{i}}{x_{k} x_{k}} = \frac{x_{i} - x_{i}}{x_{k} x_{k}} = 0$$
As a result, the second term's Poisson bracket is zero, leaving only the first term to be the only term. That bracket evaluates to $$\left\{ m \epsilon_{ijk} x_{i} \dot{x}_{j}, \frac{m\dot{x}_{j} \dot{x}_{j}}{2} \right\} = \sum_{k} \left( \frac{ \partial A }{ \partial x_{k} } \frac{ \partial B }{ \partial p_{k} }  - \frac{ \partial A }{ \partial p_{k} } \frac{ \partial B }{ \partial x_{k} }  \right)  $$
The partial derivatives in the Poisson bracket evaluate to:
- $$\frac{\partial A}{\partial x_{k}} = m \epsilon_{ijk}\delta_{ik}\dot{x}_{j}$$
- $$\frac{ \partial A }{ \partial p_{k} } = \epsilon_{ijk} \delta_{jk} x_{i} $$
These two partial derivatives evaluate to zero, so the sum must be zero for all $k$. Therefore $$\left\{ m \epsilon_{ijk} x_{i} \dot{x}_{j}, \frac{m\dot{x}_{j} \dot{x}_{j}}{2} \right\} = 0$$
(c) Angular momentum is not conserved for the charge in the presence of a monopole magnetic field.
## Problem 4
The following conditions must hold for a transformation to be canonical:
- $$\left\{ Q_{i}, Q_{j} \right\} = 0$$
- $$\left\{ P_{i}, P_{j} \right\} = 0$$
- $$\left\{ Q_{i}, P_{j} \right\} = \delta_{ij}$$
(a) The relevant partial derivatives for $P=\frac{1}{2} \left( p^2 + q^2 \right)$ and $Q = \arctan \left( \frac{q}{p} \right)$ $$\frac{ \partial Q_{i} }{ \partial q_{k}} = \delta_{ik} \frac{p_{i}}{q_{i}^2 + p_{i}^2} $$
$$\frac{\partial P_{j}}{p_{k}} = \delta_{jk} p_{j}$$
$$\frac{\partial Q_{i}}{\partial p_{k}} = -\delta_{ik} \frac{q_{i}}{q_{i}^2 + p_{i}^2}$$
$$\frac{\partial P_{j}}{\partial q_{k}} = \delta_{jk} q_{j}$$
Evaluating the Poisson bracket, $$\left\{ Q_{i}, P_{j} \right\} = \delta_{ij} \left( \frac{p_{i} p_{j}}{q_{i}^2 + p_{i}^2} + \frac{q_{i}q_{j}}{p_{i}^2 + q_{i}^2} \right)= \delta_{ij} $$
(b) The relevant partial derivatives for $P=\frac{1}{q}$ and $Q=pq^{2}$ $$\frac{\partial Q_{i}}{\partial q_{k}} = 2p_{i} q_{i} \delta_{ik}$$
$$\frac{\partial P_{j}}{\partial p_{k}} = 0$$
$$\frac{\partial Q_{i}}{\partial p_{k}} = q_{i}^2 \delta_{ik}$$
$$\frac{\partial P_{j}}{\partial q_{k}}= - \frac{\delta_{jk}}{q_{i}^2}$$
$$\left\{ Q_{i}, P_{j} \right\} = \sum_{k} \left[ 0 + \delta_{ik} \delta_{jk} \frac{q_{i}^2}{q_{i}^2} \right] = \delta_{ij}$$
(c) The relevant partial derivative for $P=\sqrt{q } \left( 1 + \sqrt{ q } \cos p \right)\sin p$ and $Q = \ln \left( 1+ \sqrt{ q } \cos p \right)$
$$\left\{ Q_{i}, P_{j} \right\} = \frac{2 \sqrt{ q } \sin^2 p (1 + \sqrt{ q }\cos p) + 2 \sqrt{ q } \cos^2 p (1+ \sqrt{ q }\cos p)}{2 \sqrt{ q } (1+ \cos p)} \delta_{ij} = \delta _{ij}$$
