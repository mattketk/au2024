# Final Equations to put on equation sheet
## Creation and annihilation
- Creation $\hat{a}_{-}=\hat{a} = \sqrt{ \frac{m\omega}{2\hbar} } \left( \hat{x} - \frac{i\hat{p}}{m\omega} \right)$
- Annihilation $\hat{a}_{+} = \hat{a}^{\dagger} = \sqrt{ \frac{m\omega}{2\hbar} } \left( \hat{x} + \frac{i\hat{p}}{m\omega} \right)$
- Hamiltonian $\hat{H} = \left( \hat{a}\hat{a}^{\dagger} - \frac{1}{2} \right)\hbar \omega$
### Algebra
- $$\begin{align}
\bra{m} a^2 \ket{n} &= \sqrt{ n (n-1) } \delta_{m,(n-2)} \\
\bra{m} \left( a^{\dagger} \right) ^2 \ket{n} &= \sqrt{ \left( n+1 \right) \left( n+2 \right)  }\delta_{m,(n+2)} \\
\bra{m} aa^{\dagger} \ket{n} &= (n+1)\delta_{mn} \\
\bra{m} a^{\dagger}a \ket{n} &= n\delta_{mn}   
\end{align}$$
## Delta Function Potential Well
- Only potential well with one bound state AND one scattering state $$V(x, x') = -V_{0}\delta(x-x')$$
- Wave function (for $x'=0$) $$$\psi(x)=\begin{cases}
\sqrt{ \kappa } \exp(\kappa x) \, x<0 \\ \\
\sqrt{ \kappa } \exp(-\kappa x) \, x>0
\end{cases}$$ where $\kappa\equiv mV_{0} / \hbar^2$
## Angular Momentum Operators
$$\begin{align}
\mathbf{J}^2 \ket{j,m} &= \hbar^2 j(j+1) \ket{j,m} \\
J_{z} \ket{j,m} &= \hbar m \ket{j,m} \\
J_{\pm} \ket{j,m} &= \sqrt{ (j \mp m) (j \pm m + 1) } \hbar \ket{j,m\pm 1} 
\end{align}$$
- Ladder operators