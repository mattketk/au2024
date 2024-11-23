# Time Evolution with time-dependent Hamiltonian
- Dyson series
- [[arbitrary-state]]
- $$i\hbar \frac{d}{dt} \begin{pmatrix}
C_{\uparrow} (t)  \\
C_{\downarrow}(t)
\end{pmatrix} = \frac{\hbar}{2} \begin{pmatrix}
\omega_{0} & \omega_{1} e^{-i\omega_{1}t} \\
\omega_{1}e^{i\omega_{1}t} & -\omega_{0}
\end{pmatrix} \begin{pmatrix}
C_{\uparrow}(t)  \\
C_{\downarrow} (t)
\end{pmatrix}$$
## Rotating wave
$$\ket{\psi(t)}  = \begin{pmatrix}
C'_{\uparrow}(t) e^{-i\omega t/2} \\
C'_{\downarrow}(t) e^{i\omega t/2}
\end{pmatrix}$$
$$\hat{H}' = \frac{\hbar}{2} \begin{pmatrix}
-\Delta \omega  & \omega_{1} \\
\omega_{1} & \Delta \omega
\end{pmatrix}$$
where $\Delta \omega \equiv \omega - \omega_{0}$
