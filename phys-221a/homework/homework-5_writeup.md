# Physics 221A Homework 5 Writeup
## Sakurai 2.12
(a)
$$\begin{align}
\Psi (x,t) =\bra{x'} \ket{\alpha;t} &= \frac{1}{\sqrt{ 2 }} \bra{x'} \ket{0} e^{-i E_{0} t / \hbar} + \frac{e^{i\delta}}{\sqrt{ 2 }} \bra{x'} \ket{1} e^{-i E_{1} t / \hbar}  \\
&= \frac{1}{\sqrt{ 2 }} \psi_{0} (x) e^{-i E_{0}t / \hbar} + \frac{e^{i\delta}}{\sqrt{ 2 }} \psi_{1} (x) e^{-i E_{1}t / \hbar}
\end{align}$$
where $$\begin{align}
\psi_{0}(x) &= \left( \frac{m\omega}{\pi \hbar} \right)^{1/4} \exp \left( -\frac{m\omega}{\hbar} x^2 \right) \\
\psi_{1} (x) &= \left( \frac{m\omega}{\pi \hbar} \right)^{1/4} \left( \sqrt{ \frac{m\omega}{\hbar} }x \right) \exp \left( -\frac{m\omega x^2}{2\hbar} \right) 
\end{align}$$
The expectation value $\left< x \right>$$$\begin{align}
\left< x \right> &= \int \Psi^\star x \Psi \, dx =  \\
&= \frac{1}{2} \int x \left[ \left(\psi_{0} (x) e^{iE_{0}t / \hbar} + e^{-i\delta} e^{iE_{1}t / \hbar} \psi_{1}(x) \right) \left( \psi_{0} (x) e^{-iE_{0}t / \hbar} + e^{i\delta} e^{-iE_{1}t / \hbar} \psi_{1}(x) \right)  \right] \, dx \\
&= \frac{1}{2} \left[ \int x \psi^2_{0} (x) \, dx + e^{i \left[ (E_{1} - E_{0}) t / \hbar - \delta \right] } \int x\psi_{0}(x) \psi_{1}(x) \, dx + e^{-i \left[ (E_{1} - E_{0}) t / \hbar - \delta \right] } \int x\psi_{0}(x) \psi_{1}(x) \, dx + \int x \psi^2_{1} (x) \, dx \right]  \\
&= \frac{e^{i \left[ (E_{1} - E_{0}) t / \hbar - \delta \right] } + e^{-i \left[ (E_{1} - E_{0}) t / \hbar - \delta \right] }}{2} \int x \psi_{0}(x) \psi_{1}(x) \, dx \\
&= \cos \left( \frac{E_{1}-E_{0}}{\hbar} t - \delta \right) \int_{-\infty}^{\infty} x \psi_{0} (x) \psi_{1}(x) \, dx  \\
&= \sqrt{ \frac{\hbar}{m\omega} } \cos \left( \frac{E_{1}-E_{0}}{\hbar} t - \delta \right) 
\end{align}$$
The expectation value $\left< p \right>$ 
# TODO!!!

## Sakurai 2.19
(a) We have a state which is a linear combination of the ground and first excited QHO states $$\ket{\psi} = a \ket{0} + b \ket{1} $$
The resulting expectation value $$\begin{align}
\bra{\psi} \hat{x} \ket{\psi} &= \left( \bra{0} a^* + \bra{1} b^* \right) \hat{x} \left( a \ket{0} + b \ket{1}  \right) \\
&= aa^* \bra{0} x \ket{0} + a^* b \bra{0} x \ket{1} + ab^* \bra{1} x \ket{0} + bb^* \bra{1} x \ket{1} \\
&= a^* b \bra{0} x \ket{1} + ab^* \bra{1} x \ket{0}   
\end{align}$$
Using the relation $$\bra{n'} x \ket{n} = \sqrt{ \frac{\hbar}{2m\omega} } \left( \sqrt{ n }\delta_{n', n-1} + \sqrt{ n+1 }\delta_{n',n+1} \right) $$
$$\bra{\psi} \hat{x} \ket{\psi}=\sqrt{ \frac{\hbar}{2m\omega} } \left( ab^* + a^* b \right) $$
The terms are maximized for $a=b=\frac{1}{2}$, so $\left< x \right> = \sqrt{ \frac{\hbar}{2m\omega} }$
(b) $E_{0} = \left( 0 + \frac{1}{2} \right)\hbar \omega= \hbar \omega / 2$ and $E_{1}= \frac{3}{2}\hbar\omega$