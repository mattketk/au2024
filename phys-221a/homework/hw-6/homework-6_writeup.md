# Physics 221A Homework 6 Writeup
## Sakurai 2.27
## Sakurai 2.29
## Sakurai 2.30
## Sakurai 2.35
## Sakurai 2.36
From the WKB consistency condition, $$\int_{x_{1}}^{x_{2}} \sqrt{ 2m (E-V(x)) } \, dx = \left( n+\frac{1}{2} \right) \pi \hbar $$
where $x_{1}, x_{2}$ are the locations of the turning points of the bound state. For a harmonic oscillator, $V(x)=\frac{1}{2}m \omega^2 x^2$. For a given state with energy $E$, the turning points correspond to the positions where $E-V(x)=0$. The zeros of this expression are $$\begin{align}
\frac{m\omega^2 x^2}{2}&=E \\
x^2 &= \frac{2E}{m\omega^2} \\
x^{\pm}_{0}&= \pm \sqrt{ \frac{2E}{m\omega^2} }
\end{align}$$
We evaluate the integral on the left-hand side for a harmonic oscillator system-- first by non-dimensionalizing the integral and then by u-substitution, $$\begin{align}
\int_{x^{-}_{0}}^{x^{+}_{0}} \sqrt{ 2m \left( E- \frac{m\omega^2x^2}{2} \right)  } \, dx &=\sqrt{ 2mE } \int_{x^{-}_{0}}^{x^{+}_{0}} dx \, \sqrt{ 1-\frac{m\omega^2 x^2}{2E} } \\ 
\eta = \sqrt{ \frac{m\omega^2}{2E} } x &\implies dx = \sqrt{ \frac{2E}{m\omega^2} } \, d \eta \\
\eta (x_{0}^\pm)&=\pm 1 \\
\sqrt{ 2mE } \sqrt{ \frac{2E}{m\omega^2} }\int_{x=x^{-}_{0}}^{x=x^{+}_{0}} d \eta \sqrt{ 1-\eta^2 } &= \frac{2E}{\omega} \int_{-1}^{1} d \eta \sqrt{ 1-\eta^2 }= \frac{2E}{\omega} \frac{\pi}{2} = \left( n+\frac{1}{2} \right) \pi \hbar \\
\therefore E &= \left( n+\frac{1}{2} \right) \hbar \omega
\end{align}$$
## Sakurai 2.41
## Sakurai 2.44