# Physics 221A Homework 4
## Sakurai 2.1
## Hints
- Look at Heisenberg picture section in Sakurai
- Heisenberg EoM $$\frac{dA^{(H)}}{dt}= \frac{1}{i\hbar} \left[ A^{(H)}, H \right] $$
	- where $A^{(H)} = \mathcal{U}^{\dagger} (t) A^{(S)} \mathcal{U} (t)$ and $\mathcal{U} (t) = \exp \left( -\frac{iHt}{\hbar} \right)$
## Sakurai 2.3
## Sakurai 2.6
### Hints
$$\left[ \left[ H, x \right], x \right] = \dots -\frac{1}{m} $$
$$\bra{a''} -\frac{1}{2}\left[ \left[ H, x \right] , x \right] \ket{a''} = \frac{1}{2m}$$
## Sakurai 2.7
Using the "Generalized Ehrenfest's theorem" (Griffiths 3.73), which states that $$\frac{d}{dt} \left< \hat{Q} \right> = \frac{i}{\hbar} \left< \left[ \hat{Q}, \hat{H} \right] \right> + \left< \frac{\partial \hat{Q}}{\partial t} \right> $$
Let $\hat{Q} = \hat{x} \cdot \hat{p}$, $$\frac{d}{dt} \left< \hat{x} \cdot \hat{p} \right> = \frac{i}{\hbar} \left< \left[ \hat{x} \cdot \hat{p}, \hat{H} \right] \right> + \left< \frac{\partial \hat{x}}{\partial t} \cdot \hat{p} + \frac{\partial \hat{p}}{\partial t} \cdot \hat{x} \right>$$
The second term on the right-hand side of the equation vanishes because neither $\hat{x}$ nor $\hat{p}$ have explicit time dependence. Expanding the first term on the right-hand side, $$ \frac{d}{dt} \left< \hat{x} \cdot \hat{p} \right> = \frac{i}{\hbar} \left< \left( \hat{x} \cdot \hat{p} \right) \hat{H} - \hat{H}(\hat{x}\cdot \hat{p}) \right> = \frac{i}{\hbar} \left[ \bra{\psi} \left( \hat{x}\cdot \hat{p} \right) \hat{H}\ket{\psi} - \bra{\psi} \hat{H} \left( \hat{x} \cdot \hat{p} \right) \ket{\psi} \right] $$
Let $\ket{\psi}$ be a stationary state, such that $\hat{H} \ket{\psi}= E\ket{\psi}$. The equation becomes $$\frac{d}{dt} \left< \hat{x} \cdot \hat{p} \right> = \frac{i}{\hbar} \left[ E\bra{\psi} \left( \hat{x}\cdot \hat{p} \right) \ket{\psi} - E\bra{\psi} \left( \hat{x} \cdot \hat{p} \right) \ket{\psi} \right] = 0$$
Thus, when the quantum state is stationary, the total time derivative $\frac{d}{dt} \left< \hat{x} \cdot \hat{p} \right>$ goes to zero, the virial theorem applies.
## Sakurai 2.11
