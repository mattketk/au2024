# Equations for Midterm I

- Completeness relation $$\ket{a} = \sum_{\alpha} \ket{\alpha} \bra{\alpha} \ket{a}  $$
## Density matrix
- Density operator $$\rho \equiv \sum_{i} w_{i} \ket{\alpha^{(i)}} \bra{\alpha^{(i)}} $$
- Density trace $$\hat{\rho}_{ji} = \sum_{n} \bra{\phi_{j}} \ket{\phi_{n}} P_{n} \bra{\phi_{n}} \ket{\phi_{i}}   $$
- Ensemble average relation $$\left[ A \right] = \mathrm{Tr} \left( \hat{\rho} A \right) $$
## Momentum as a generator of translation
- Translation operator $$\hat{T} \left( dx \right) = \hat{I} - i \hat{k} dx$$
	- $\hat{k}$ is a generator corresponding to momentum 
	- Obeys unitarity $\hat{T}^{\dagger}\hat{T}=\hat{I}$, $$\hat{T}^{\dagger}=\hat{I}+i\hat{k}dx \implies \hat{T}^{\dagger}\hat{T}= \left( \hat{I} + i\hat{k}dx \right) \left( \hat{I} - i\hat{k}dx \right) = \hat{I}\hat{I} + \hat{k}\hat{k}dx^2= \hat{I} $$ in the limit as $\lim_{ dx \to 0 }$ and neglecting $dx^2$ terms
- In a periodic space where $\left( x \in S', L^2(S') \right)$, momentum is discrete $$p=p_{n} = \frac{\hbar n}{l}$$ $l$ is the spatial period. If the momentum were continuous in this space, the wave function in this space would have discontinuities.
## A similar argument for the Hamiltonian and time...
- Heisenberg equation of motion $$\frac{d}{dt} \left< \hat{A} \right> = \frac{i}{\hbar}\left< \hat{H}, \hat{A}^{(S)} \right> $$