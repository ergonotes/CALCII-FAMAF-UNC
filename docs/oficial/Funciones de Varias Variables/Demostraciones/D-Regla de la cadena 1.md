**Demostración.** Un cambio de $\Delta t$ en $t$ produce cambios de $\Delta x$ en $x$ y de $\Delta y$ en $y$. Esto produce a su vez un cambio de $\Delta z$ en $z$, y por la definición de derivabilidad en el inciso [[6.Regla de la Cadena]], se tiene

$$
\Delta z = \frac{\partial f}{\partial x} \Delta x + \frac{\partial f}{\partial y} \Delta y + \varepsilon_1 \Delta x + \varepsilon_2 \Delta y
$$

donde $\varepsilon_1 \to 0$, $\varepsilon_2 \to 0$ cuando $(\Delta x, \Delta y) \to (0, 0)$. Al dividir ambos miembros de esta ecuación entre $\Delta t$, se tiene

$$
\frac{\Delta z}{\Delta t} = \frac{\partial f}{\partial x} \frac{\Delta x}{\Delta t} + \frac{\partial f}{\partial y} \frac{\Delta y}{\Delta t} + \varepsilon_1 \frac{\Delta x}{\Delta t} + \varepsilon_2 \frac{\Delta y}{\Delta t}
$$

Si ahora se permite que $\Delta t \to 0$, entonces $\Delta x = g(t + \Delta t) - g(t) \to 0$, porque $g$ es derivable y por tanto continua. De igual forma, $\Delta y \to 0$. Esto significa a su vez que $\varepsilon_1 \to 0$ y $\varepsilon_2 \to 0$, así que

$$
\begin{aligned}
\frac{dz}{dt} &= \lim_{\Delta t \to 0} \frac{\Delta z}{\Delta t} \\
&= \frac{\partial f}{\partial x} \lim_{\Delta t \to 0} \frac{\Delta x}{\Delta t} + \frac{\partial f}{\partial y} \lim_{\Delta t \to 0} \frac{\Delta y}{\Delta t} + \left( \lim_{\Delta t \to 0} \varepsilon_1 \right) \lim_{\Delta t \to 0} \frac{\Delta x}{\Delta t} + \left( \lim_{\Delta t \to 0} \varepsilon_2 \right) \lim_{\Delta t \to 0} \frac{\Delta y}{\Delta t} \\
&= \frac{\partial f}{\partial x} \frac{dx}{dt} + \frac{\partial f}{\partial y} \frac{dy}{dt} + 0 \cdot \frac{dx}{dt} + 0 \cdot \frac{dy}{dt} \\
&= \frac{\partial f}{\partial x} \frac{dx}{dt} + \frac{\partial f}{\partial y} \frac{dy}{dt}
\end{aligned}
$$

Como se suele escribir $\partial z/\partial x$ en vez de $\partial f/\partial x$, se puede reescribir la regla de la cadena en la forma

$$
\frac{dz}{dt} = \frac{\partial z}{\partial x} \frac{dx}{dt} + \frac{\partial z}{\partial y} \frac{dy}{dt}
$$

****
--8<-- "includes/fuente.md"
