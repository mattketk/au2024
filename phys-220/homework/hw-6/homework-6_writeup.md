# Physics 220 Homework 6 Writeup
For problems 1 and 2, we take the speed of light to be $c=1$.
## Problem 1
(a) The final 4-momentum after the interaction is the sum of the two 4-momenta vectors corresponding to each particle, $$\begin{align}
p_{f}^{\mu}=\begin{pmatrix}
\gamma_{1}m_{1} + \gamma_{2} m_{2} \\
\gamma_{1}m_{1}v_{1} + \gamma_{2}m_{2}v_{2}
\end{pmatrix}
\end{align}$$
Taking its Lorentz invariant, we get $$\begin{align}
p_{i}^{\mu}p_{i,\mu}&=-\left( \gamma_{1}m_{1}+\gamma_{2}m_{2} \right) ^2 + \left( \gamma_{1}m_{1}v_{1}-\gamma_{2}m_{2}v_{2} \right) ^2 \\
&=(\gamma_{1}m_{1}v_{1})^{2} - 2 (\gamma_{1}m_{1}v_{1})(\gamma_{2}m_{2}v_{2})+(\gamma_{2}m_{2}v_{2})^{2} \\
&- \left( \gamma_{1}m_{1} \right) ^{2}-2\gamma_{1}\gamma_{2}m_{1}m_{2}-(\gamma_{2}m_{2})^{2}
\end{align}$$
Also noting that $$\gamma^{2}m^2 \left( v^{2}-1 \right) = m^{2} \frac{v^{2}-1}{1-v^2}=-m^2$$
The Lorentz invariant simplifies to $$\begin{align}
-(m_{1}^{2}+m_{2}^{2})-2\gamma_{1}\gamma_{2}m_{1}m_{2} & (1+v_{1}v_{2})
\end{align}$$
which equals the Lorentz invariant of final momentum $$\begin{align}
-m^2&=-(m_{1}^{2}+m_{2}^{2})-2\gamma_{1}\gamma_{2}m_{1}m_{2}(1+v_{1}v_{2}) \\
\implies m^{2}&=\left( m_{1}^2+m_{2}^2 \right) +2\gamma_{1}\gamma_{2}m_{1}m_{2}(1+v_{1}v_{2})
\end{align}$$
(b) Since both $m_{1},m_{2}>0$ and $0<1+v_{1}v_{2}< 2$, both terms on the right-hand side are manifestly positive, so $m>0$ and the resulting product cannot be a photon (or any massless particle for that matter).
(c) For $m=0$, both masses $m_{1},m_{2}$ must vanish.
## Problem 2
The system conserves 4-momentum, so the sum of the 4-momentum vectors for the pion and neutron should equal the 4-momenta of the products (kaon and lambda baryon) $$\begin{align}
p^{\mu}_{\pi} &= \begin{pmatrix}
E_{\pi} \\
\sqrt{ E^{2}_{\pi} - m_{\pi}^2 }
\end{pmatrix} \\
p_{n}^\mu &= \begin{pmatrix}
m_{n} \\
0
\end{pmatrix} \\
\implies p_{i}^{\mu} &= \begin{pmatrix}
E_{\pi} + m_{n} \\
\sqrt{ E_{\pi}^2 - m_{\pi}^2 }
\end{pmatrix} = p_{f}^{\mu} = \begin{pmatrix}
m_{\Lambda} + m_{\kappa} \\
0
\end{pmatrix}
\end{align}$$
Relating the 4-momenta to its Lorentz invariant, we get the relation $$\begin{align}
-\left( E_{\pi}+m_{n} \right) ^2 +(E_{\pi}^2 - m_{\pi}^2) = -(m_{\Lambda}+m_{\kappa})^2
\end{align}$$
Rearranging the equation for $E_{\pi}$, we get $$\begin{align}
E_{\pi}= T_{\pi} + m_{\pi}=\frac{\left( m_{\kappa}+m_{\Lambda} \right) ^2 - \left( m_{n}^2+m_{\pi}^2 \right) }{2 m_{n}}
\end{align}$$
Substituting the numerical values, we get $$T_{\pi} = E_{\pi} - m_{\pi} = \left( 899 - 139 \right) \, \mathrm{MeV} = 760 \, \mathrm{MeV} $$

## Problem 3
(a) Start with the relativistic Lagrangian $$L=-mc^2 \sqrt{ 1-\beta^2 } - V$$
$$L=-mc^2\sqrt{ 1-\beta^2 }- \frac{1}{2}kx^2$$
Transforming into the Hamiltonian, we get $$H=p_{i} \dot{q}^{i}- L=\frac{mv_{i}v^{i}}{\sqrt{ 1-\beta^2} } + mc^2 \sqrt{ 1-\beta^{2} }+V$$
(c) This can be rearranged as the total energy of the system, $$H=\frac{mc^2}{\sqrt{ 1-\beta^2 }} + V = T + V + mc^2 = E$$
(b) The Hamiltonian does not explicitly depend on time, so the total energy $E$ is conserved. Rearranging the above relation, $$\begin{align}
\frac{mc^{2}}{\sqrt{ 1-\beta^2 }} &= E-V \\
\frac{\left( mc^2 \right) ^2}{1-\beta^2} &= \left( E-V \right) ^2 \\
\frac{\dot{x}^2}{c^2} &= 1- \frac{\left( mc^2 \right) ^2}{\left( E-V \right) ^2}
\end{align}$$
We demand the potential $V(x)$ to be symmetric about the origin and that the total energy $E$ is $V(0) \leq E\leq V_{\text{max}}$ so $$V\left( \pm a \right) = E$$
(d) Rearranging the relation between $\dot{x}$ and the energy and potential, $$\begin{align}
\frac{1}{\dot{x}}&=\frac{1}{\sqrt{ 1- \frac{\left( mc^2 \right) ^2}{\left( E-V \right) ^2} }} \\
dt &= \frac{dt}{\sqrt{ 1- \frac{\left( mc^2 \right) ^2}{\left( E-V \right) ^2} }} \\
P&=\int \, dt= \int_{0}^{a}  \, \frac{dt}{\sqrt{ 1- \frac{\left( mc^2 \right) ^2}{\left( E-V \right) ^2} }} 
\end{align}$$
(e) Introducing relativistic corrections (to first order), write the energy as $$E=mc^2 \left( 1+\epsilon \right) $$
$$\frac{E-V(x)}{mc^2} = \frac{mc^2 (1+\epsilon) - V(x)}{mc^2} = 1+\epsilon - \frac{1}{2} \frac{kx^2}{mc^2}=1+\epsilon-\kappa x^2=1+\kappa(a^{2}-x^{2})$$
(Defined a parameter $\kappa\equiv \frac{k}{2mc^2}$ and let $\epsilon=ka^2 / 2mc^2=\kappa a^2$). This results in the period integral expression 
$$\begin{align}

P&=\int \, dt= \frac{4}{c}\int_{0}^{a}  \, \frac{dx}{\sqrt{ 1- \frac{1}{\left( 1+\kappa (a^2 - x^2) \right)^2 } }} 
\end{align}$$
For a first order approximation, neglect terms $\left( \kappa a^2 \right)^2$ or higher, which makes the following polynomial simplify to $$\begin{align}
\left( 1+\kappa (a^2 - x^2) \right)^2&=1+\kappa a^2 - kx^2  \\
&+ \kappa a^2 + \left( \kappa a^2 \right) ^2 - \left( \kappa x^2 \right) \left( \kappa a^2 \right) \\
&-\kappa x^2 + \left( \kappa a^2 \right) \left( \kappa x^2 \right) + \left( \kappa x^2 \right) \\
&=1 + 2\kappa\left(a^{2}-x^{2} \right) 
\end{align}$$
Substituting, $$\begin{align}
P&= \frac{4}{c}\int_{0}^{a}  \, \frac{dx}{\sqrt{ 1- \frac{1}{ 1 + 2\kappa\left(a^{2}-x^{2} \right)} }} \approx \frac{4}{c}\int_{0}^{a}  \, \frac{dx}{\sqrt{ 2 \kappa \left( a^{2}-x^2 \right)  }} \left[ 1- \frac{3\kappa}{4} (a^{2} - x^{2}) \right]   
\end{align}$$
Change the variables with the relation $x=a\sin \phi \implies a^2-x^2 = a^2 \cos^2\phi$, $$P= \frac{4}{c}\int_{x=0}^{x=a}  \, \frac{\cos \phi d\phi}{\sqrt{ 2\kappa a^2 \cos^2\phi }} \left( 1- \frac{3\kappa}{4} \cos^2 \phi \right) = \frac{4}{ac \sqrt{ 2\kappa }} \int_{x=0}^{x=a} \left( 1- \frac{3\kappa}{4} \cos^2 \phi \right) \, d\phi$$

$$ P \approx \frac{2\pi}{c} \frac{1}{\sqrt{ 2\kappa }} \left( 1-\frac{3}{8}\kappa a^{2} \right) = 2\pi \sqrt{ \frac{m}{k} } \left( 1- \frac{3}{16} \frac{ka^2}{mc^2} \right) $$
## Problem 4
- Velocity addition $$u'=\frac{v-u}{1-uv}$$
We can make conservation statements for infinitesimals in the lab frame, namely, the conservation of energy and 4-momentum, $$\begin{align}
\Delta p&=0=d \left( \gamma_{v} m v \right) +\gamma_{u'}u'dm \\
\Delta E&=0=d(m\gamma_{u})+\gamma_{u'}dm
\end{align}$$
The statement for energy conservation can be rearranged as follows, $$\gamma_{u'}dm = -d (m\gamma_{u})$$
substituting into the momentum conservation relation, $$-d (\gamma_{v}mv)=-u'd(m\gamma_{u}) \implies \frac{d}{dt}(\gamma_{v}mv)=u'\frac{d}{dt}(m\gamma_{u})$$
$$\dot{\gamma}_{v}mv + \gamma_{v}\dot{m}v + \gamma_{v}m\dot{v}=u'\left( \dot{m}\gamma_{u'}+m\dot{\gamma}_{u'} \right) $$
$$\dot{\gamma}_{v}=\dot{v}v\gamma^{3}_{v}$$
Dividing both sides by $\gamma_{v}\dot{m}$, $$\frac{\dot{\gamma}_{v}mv}{\gamma_{v}\dot{m}}+v+m \frac{dv}{dm}=u' (\dot{m}\gamma_{u'}+ m \dot{\gamma}_{u'})$$
$$\frac{\dot{v}v^2\gamma^{3}m}{\gamma_{v}\dot{m}}+v+\frac{\gamma_{v}m}{\gamma_{v}\dot{m}}\dot{v}t=\frac{uv\dot{m}\gamma_{u'}}{1-uv} \frac{1}{\dot{m}\gamma_{u}}+u'(m\dot{v}v\gamma_{v}^3)$$
$$\begin{align}
(1+v^2\gamma_{v}^2)-u'v\gamma ^2)m \frac{dv}{dm}&=u'-v \\
\left( \frac{1}{\gamma^2}+v^2-u'v \right)\gamma_{v}^2 m \frac{dv}{dm}&=u'-v  \\
\left( 1-u'v\right)\gamma_{v}^2 m \frac{dv}{dm}&=u'-v
\end{align}$$
Which becomes $$\frac{1}{u(1-v^2)}dv = \frac{dm}{m}$$
Integrating, we get $$\frac{1}{u} \frac{1}{2}\ln \left( \frac{1+v}{1-v} \right) =\ln \left( \frac{m}{m_{0}} \right) \implies \frac{1+v}{1-v}=\exp \left( 2u \ln \left( \frac{m}{m_{0}} \right)  \right) $$
$$v=\frac{\exp \left( 2u \ln \left( \frac{m}{m_{0}} \right) \right) +1 }{\exp \left( 2u \ln \left( \frac{m}{m_{0}} \right)  \right) -1}$$
$$v=c\tanh \left( \frac{u}{c}\ln \left( \frac{m}{m_0} \right)  \right)  $$

