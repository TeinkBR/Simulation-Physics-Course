# 2 Cannonball
# 2.1 Simulating a cannonball

Simulation of the trajectory of a cannonball in $2 \mathrm{D}$ until it hits the ground. As we known Newton's equations of motion:\\

\begin{equation}
\begin{aligned}
\frac{\mathrm{d} \mathbf{x}(t)}{\mathrm{d} t} &=\mathbf{v}(t) \\
\frac{\mathrm{d} \mathbf{v}(t)}{\mathrm{d} t} &=\frac{\mathbf{F}(t)}{m}
\end{aligned}
\end{equation}

The position $\mathbf{x}(t)$ is a function of time $t, m$ is the mass and $\mathbf{F}(t)$ is the time dependent force.

At time $t=0$, the cannonball (mass $m=2.0 \mathrm{~kg}$ ) is at $\mathbf{x}(0)=\mathbf{0}$ and has a velocity of $\mathbf{v}(0)=(50,50)^{\top} \mathrm{m} \mathrm{s}^{-1}$.

A simple Euler scheme is used to to simulate the cannon ball motion by appending the position $\mathbf{x}(t)$ and velocity $\mathbf{v}(t)$ at time $t$ to the time $t+\Delta t(\Delta t=0.1 \mathrm{~s})$ :\\

\begin{equation}
\begin{aligned}
&\mathbf{x}(t+\Delta t)=\mathbf{x}(t)+\mathbf{v}(t) \Delta t \\
&\mathbf{v}(t+\Delta t)=\mathbf{v}(t)+\frac{\mathbf{F}(t)}{m} \Delta t
\end{aligned}
\end{equation}
