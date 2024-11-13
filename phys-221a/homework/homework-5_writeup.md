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
![[sakurai2-12.jpg]]
## Sakurai 2.14
Recognize that the finite translation operator $\hat{T} (a) = \exp \left(  \frac{-ipa}{\hbar} \right)$ is acting on the ground state of the the SHO. Thus, the expectation value $\left< x \right>$ is $$\left< x^{(H)} \right> = \bra{0} \hat{T}^{\dagger} x(0) \hat{T} \ket{0} \cos \left( \omega t \right) + \bra{0} \hat{T}^{\dagger} p (0) \hat{T} \ket{0} \frac{\sin \left( \omega t \right)}{m\omega} $$ We may simplify the evaluation of this expression by noting the following commutator relations, $$\begin{align}
\left[ \hat{x}, \hat{T} (a) \right] &= -a \hat{T}(a) \implies \hat{x} \hat{T} (a) = -a \hat{T} (a) + \hat{T} (a) x\\
\left[ \hat{p}, \hat{T} (a) \right] &= 0 \implies \hat{p} \hat{T} (a) = \hat{T} (a) \hat{p}
\end{align}$$
($\hat{p}$ commutes with $\hat{T}$ because momentum is a generator of translation.)  Substituting the commutator relations, we get $$\begin{align}
\left< x^{(H)} \right> &= \bra{0} \hat{T}^{\dagger}\hat{T} x(0) \ket{0}\cos \left( \omega t \right) - a \bra{0} \hat{T}^{\dagger} \hat{T} \ket{0} \cos \left( \omega t \right)  + \bra{0} \hat{T}^{\dagger} \hat{T} p(0) \ket{0} \frac{\sin \left( \omega t \right) }{m\omega} \\
&= -a \cos \left( \omega t \right) 
\end{align}$$
## Sakurai 2.16
(a)
$$\begin{align}
\bra{m} a^2 \ket{n} &= \sqrt{ n (n-1) } \delta_{m,(n-2)} \\
\bra{m} \left( a^{\dagger} \right) ^2 \ket{n} &= \sqrt{ \left( n+1 \right) \left( n+2 \right)  }\delta_{m,(n+2)} \\
\bra{m} aa^{\dagger} \ket{n} &= (n+1)\delta_{mn} \\
\bra{m} a^{\dagger}a \ket{n} &= n\delta_{mn}   
\end{align}$$
The resulting relations are $$\begin{align}
\bra{m} \hat{x} \ket{n} &= \frac{1}{2} \sqrt{ \frac{2\hbar}{m\omega} } \left( \bra{m} a \ket{n} + \bra{m} a^{\dagger} \ket{n}  \right) = \sqrt{ \frac{\hbar}{2m\omega} } \left( \sqrt{ n } \delta_{m,(n-1)} + \sqrt{ n+1 }\delta_{m,(n+1)} \right) \\
\bra{m} \hat{p} \ket{n} &= \frac{-im\omega}{2} \sqrt{ \frac{2\hbar}{m\omega} } \left( \bra{m} a \ket{n} - \bra{m} a^{\dagger} \ket{n} \right) = -i \sqrt{ \frac{\hbar m\omega}{2} }\left( \sqrt{ n }\delta_{m,(n-1)} - \sqrt{ n+1 } \delta_{m,(n+1)} \right) \\
\end{align}$$
Derive the following relations
$$\begin{align}
\bra{m} \hat{x} = \sqrt{ \frac{\hbar}{2m\omega} } \left( \sqrt{ m }\bra{m-1} + \sqrt{ m+1 }\bra{m+1}  \right)  \\
\bra{m} \hat{p} = -i \sqrt{ \frac{\hbar m\omega}{2} } \left( \sqrt{ m+1 }\bra{m+1} - \sqrt{ m } \bra{m-1}  \right) 
\end{align}$$

to derive $$\bra{m} \left\{ \hat{x},\hat{p} \right\} \ket{n} = \bra{m} \hat{x} \hat{p} \ket{n} + \bra{m} \hat{x} \hat{p} \ket{n} = i\hbar \left( \sqrt{ n(m+1) }\delta_{(m+1),(n-1)} + \sqrt{ m(n+1) }\delta_{(m-1),(n+1)}\right)  $$
Finally, derive the following relations $$\begin{align}
\bra{m} a^2 \ket{n} &= \sqrt{ n (n-1) } \delta_{m,(n-2)} \\
\bra{m} \left( a^{\dagger} \right) ^2 \ket{n} &= \sqrt{ \left( n+1 \right) \left( n+2 \right)  }\delta_{m,(n+2)} \\
\bra{m} aa^{\dagger} \ket{n} &= (n+1)\delta_{mn} \\
\bra{m} a^{\dagger}a \ket{n} &= n\delta_{mn}   
\end{align}$$
to derive the following relations
$$\begin{align}
\bra{m} \hat{x}^2 \ket{n} &= \frac{\hbar}{2m\omega} \left( \sqrt{ n(n-1) }\delta_{m,(n-2)} + (n+1) \delta_{mn} + n\delta_{mn} + \sqrt{ (n+1)(n+2) }\delta_{m,(n+2)} \right)  \\
\bra{m} \hat{p}^2 \ket{n} &= -\frac{\hbar m\omega}{2} \left( \sqrt{ n(n-1) }\delta_{m,(n-2)} - (n+1) \delta_{mn} - n\delta_{mn} + \sqrt{ (n+1)(n+2) }\delta_{m,(n+2)} \right) 
\end{align}$$
(b) Verifying the virial theorem $$\left< \frac{\hat{p}^{2}}{m} \right> = \left< x \frac{dV}{dx} \right> $$
The left-hand side evaluates to $$\frac{1}{m} \left< \hat{p}^2 \right> = \frac{1}{m} \left( - \frac{\hbar m\omega}{2} \left( -(n+1)-n \right)  \right) =\hbar \omega \left( n+\frac{1}{2} \right) $$
To evaluate the right-hand side, evaluate the potential spatial derivative $$\frac{dV}{dx} = \frac{1}{2}m \omega^{2} \frac{d}{dx} (x^2)= m\omega^{2} x$$ the right-hand side becomes $$\left< x \frac{dV}{dx} \right> = m\omega^{2} \left< x^2 \right> = m\omega^2 \left( \frac{\hbar}{2m\omega}(2n+1) \right) = \hbar \omega \left( n + \frac{1}{2} \right)  $$
Using the algebra of annihilation and creation operators, we prove the virial theorem for QHOs.
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
For the Schrödinger picture, $$\begin{align}
\left< x \right> &= \frac{1}{2} \left( \exp \left( i\omega t /2\right) \bra{0} + \exp \left( i 3 \omega t / 2 \right) \bra{1} \right) \hat{x} \left( \exp \left( -i\omega t /2\right) \ket{0} + \exp \left( -i 3 \omega t / 2 \right) \ket{1} \right) \\
&=\frac{1}{2} \left[ \bra{0} \hat{x} \ket{0} + \exp \left( -i \omega t \right) \bra{0} \hat{x} \ket{1} + \exp \left( i\omega t \right) \bra{1} \hat{x} \ket{0} + \bra{1} \hat{x} \ket{1} \right]  \\
&=\frac{\exp \left( i\omega t \right) + \exp \left( -i\omega t \right)}{2} \sqrt{ \frac{\hbar}{2m\omega} }  \\
&=\sqrt{ \frac{\hbar}{2m\omega} }\cos \left( \omega t \right) 
\end{align}$$
(ii) From the Heisenberg equation of motion $$\begin{align}
\frac{d x^{(H)}}{dt}&= -\frac{i}{\hbar} \left[ \hat{x}, \hat{H} \right] =  -\frac{i}{\hbar} \left( \left[ \hat{x}, \frac{\hat{p}^2}{2m} \right] + \left[ \hat{x}, V(x) \right]  \right) \\
&= -\frac{i}{2m\hbar} \left( \left[ \hat{x}, \hat{p} \right] \hat{p} + \hat{p} \left[ \hat{x}, \hat{p}\right]  \right) \\
&= \frac{\hat{p} (0)}{m} \\
\implies x^{(H)}(t) &= x(0) + \frac{\hat{p}(0)}{m}t
\end{align}$$
The expectation value is $$\left< x^{(H)} \right> = \left< x(0) \right> + \frac{t}{m} \left< \hat{p}(0) \right> = \sqrt{ \frac{\hbar}{2m\omega}} \cos \left( \omega t \right) $$
(c) $$\left< \left( \Delta x \right) ^2 \right> = \left< x^2 \right> - \left< x \right> ^2$$
$$\begin{align}
\left< x^2 \right> &= \left< \left( \frac{\hbar}{2m\omega} \right) \left( a^{2}+ aa^{\dagger}+a^{\dagger}a+ \left( a^{\dagger} \right) ^2 \right)  \right> \\
&= \frac{1}{2} \left( \bra{0} x^{2}\ket{0} +\bra{0} x^2 \ket{1} + \bra{1} x^{2}\ket{0} + \bra{1} x^2 \ket{1} \right) \\
\end{align}$$
From the work in response to Sakurai 2.16, the "cross terms" vanish. $$ \left< x^{2} \right> = \frac{1}{2} \left( \bra{0} x^{2}\ket{0} + \bra{1} x^{2}\ket{1}  \right) = \frac{1}{2} \left( \frac{\hbar}{2m\omega}+ \frac{3\hbar}{2m\omega} \right) = \frac{\hbar}{m\omega} $$
$$\left< \left( \Delta x \right) ^2 \right> = \frac{\hbar}{m\omega} - \frac{\hbar}{2m\omega} \cos ^{2} \left( \omega t \right) $$

## Sakurai 2.23
We note that since the QHO systems are independent of one another, they can be measured simultaneously. As a result, $$\begin{align}
[a_{\pm}, a_{\mp}]=[a^{\dagger}_{\pm}, a^{\dagger}_{\mp}]=[a_{\pm}, a^{\dagger}_{\mp}]=[a^{\dagger}_{\pm}, a_{\mp}]=0
\end{align}$$
Proving the commutator relation $$\left[ J_{z}, J_{\pm} \right] = \pm \hbar J_{\pm}$$
$$\begin{align}
\left[ J_{z}, J_{\pm} \right] &=\frac{\hbar^2}{2} \left( a^{\dagger}_{+} a_{+} - a^{\dagger}_{-}a_{-} \right)a^{\dagger}_{\pm} a_{\mp} - \frac{\hbar^{2}}{2}a^{\dagger}_{\pm} a_{\mp} \left( a^{\dagger}_{+}a_{+} - a^{\dagger}_{-}a_{-} \right) \\
&= \frac{\hbar^{2}}{2} \left( \left[ a^{\dagger}_{+}a_{+}, a^{\dagger}_{\pm} a_{\mp} \right] + \left[ a^{\dagger}_{\pm} a_{\mp}, a^{\dagger}_{-} a_{-} \right]  \right) 
\end{align}$$
Using the commutator relation $$\left[ AB, CD \right] = A[B, C]D + [A,C]BD + CA[B,D]+ C[A,D]B$$, we evaluate each commutator term:
- $$\left[ a^{\dagger}_{+}a_{+}, a^{\dagger}_{\pm} a_{\mp} \right]= \pm a^{\dagger}_{\pm} a_{\mp}$$
- $$\left[ a^{\dagger}_{\pm} a_{\mp}, a^{\dagger}_{-} a_{-} \right]=\pm a^{\dagger}_{\pm}a_{\mp}$$
Substituting these results into the original commutator, $$\left[ J_{z}, J_{\pm} \right] = \frac{\hbar^{2}}{2}\left(\pm 2 a^{\dagger}_{\pm}a_{\mp} \right)= \pm \hbar^{2} a^{\dagger}_{\pm} a_{\mp} = \pm \hbar J_{\pm} $$
Proving that $$\left[ \mathbf{J}^{2}, J_{z} \right] = 0$$
$$\begin{align}
\left[ \mathbf{J}^{2}, J_{z} \right] &= \left[ J_{z}^{2}, J_{z} \right] + \frac{1}{2} \left( [J_{+}J_{-}, J_{z}]+[J_{-}J_{+},J_{z}] \right)  \\
&= \left[ J_{z}^{2}, J_{z} \right] + \frac{1}{2} \left( [J_{+}, J_{z}]J_{-}+J_{+}\left[ J_{-}, J_{z} \right] + \left[ J_{-}, J_{z} \right] J_{+} + J_{-} \left[ J_{+}, J_{z} \right]  \right)  \\
&= 0 + \frac{1}{2}\left( -\hbar J_{+}J_{-} + \hbar J_{+}J_{-} +  \hbar J_{-}J_{+} - \hbar J_{-}J_{+} \right) = 0 \\
\end{align}$$
$$\mathbf{J}^2= \frac{\hbar^{2}}{2} N \left( \frac{N}{2}+1 \right)$$![[sakurai2-23.jpg]]