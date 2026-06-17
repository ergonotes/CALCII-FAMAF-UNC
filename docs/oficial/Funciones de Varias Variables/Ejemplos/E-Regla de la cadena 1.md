**Ejemplo.** Sea $f(x,y) = x^2 + y^2 + xy$, con $x(t) = \text{sen}(t)$, $y(t) = e^t$. Hallar $\frac{df}{dt}$.

* Tenemos que: $\frac{\partial f}{\partial x}(x, y) = 2x + y \ ; \ \frac{\partial f}{\partial y}(x, y) = 2y + x$.
  $x'(t) = \cos(t) \ ; \ y'(t) = e^t$.

Luego
$$
\begin{aligned}
\frac{df}{dt} &= \frac{\partial f}{\partial x}(x(t), y(t)) \cdot x'(t) + \frac{\partial f}{\partial y}(x(t), y(t)) \cdot y'(t) \\
&= (2x(t) + y(t)) \cdot \cos(t) + (2y(t) + x(t)) e^t \\
&= (2\text{sen}(t) + e^t) \cos(t) + (2e^t + \text{sen}(t)) e^t \quad (1)
\end{aligned}
$$

##### **Observación:** Notar que... 
si escribimos $$f(t) = x^2(t) + y^2(t) + x(t)y(t) = \text{sen}^2(t) + e^{2t} + \text{sen}(t)e^t$$
entonces $\frac{df}{dt} = 2\text{sen}(t)\cos(t) + 2e^{2t} + \cos(t)e^t + \text{sen}(t)e^t$ que es igual a $(1)$.
****
A veces, usar la Regla de la Cadena, como hicimos en el ejemplo es más rápido y ordenado si las funciones son horriblemente complejas.
Otras veces, si las sustituciones son fáciles, simplemente meter las funciones adentro y derivar todo de golpe (la observación) se nos hace más memorable, y funciona como una forma alternativa si las funciones originales tienen picos o puntos no derivables.

****
--8<-- "includes/fuente.md"
