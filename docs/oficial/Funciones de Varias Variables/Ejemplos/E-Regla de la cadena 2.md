**Ejemplo:** Sea $f(x,y) = xy + 2y^2 + x^3$, donde $x(s,t) = st$, $y(s,t) = e^{st}$. Calcular $\frac{\partial f}{\partial s}$ en el punto $(s,t) = (1,1)$.

* Tenemos que: 
  * $f_x(x,y) = y + 3x^2$ ; $f_y(x,y) = x + 4y$.
  * $x_s(s,t) = t$ ; $y_s(s,t) = t e^{st}$.

Luego,
$$
\begin{aligned}
\frac{\partial f}{\partial s}(s,t) &= f_x(x(s,t), y(s,t)) \cdot x_s(s,t) + f_y(x(s,t), y(s,t)) \cdot y_s(s,t) \\
&= (e^{st} + 3(st)^2)t + (st + 4e^{st})t e^{st} \quad (\square)
\end{aligned}
$$
Finalmente, si evaluamos en $(s, t) = (1, 1)$ obtenemos

$$
\frac{\partial f}{\partial s}(1, 1) = (e + 3) \cdot 1 + (1 + 4e)e = 4e^2 + 2e + 3
$$

#### **Observación:** notar que si escribimos $f(s, t) = x(s, t)y(s, t) + 2y^2(s, t) + x^3(s, t) = st e^{st} + 2 e^{2st} + s^3 t^3$

entonces $\frac{\partial f}{\partial s}(s, t) = t e^{st} + st^2 e^{st} + 2 \cdot 2t e^{2st} + 3 s^2 t^3$ que es igual a $(\blacksquare)$.