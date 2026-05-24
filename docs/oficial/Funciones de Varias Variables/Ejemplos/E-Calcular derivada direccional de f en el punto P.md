**Ejemplo:** calcular la derivada direccional de $f(x, y) = x e^y$ en el punto $P = (2, 0)$ en la dirección de $\vec{v} = (1, \sqrt{3})$.

* Notemos que $\vec{v}$ no es unitario ya que $\|\vec{v}\| = \sqrt{1+3} = 2$. Luego, debemos considerar el vector $\vec{u} = \frac{\vec{v}}{\|\vec{v}\|} = \frac{1}{2}(1, \sqrt{3})$ que tiene la misma dirección que $\vec{v}$ pero es unitario.

Por otra parte, $\frac{\partial f}{\partial x}(x, y) = e^y$ y $\frac{\partial f}{\partial y}(x, y) = x e^y$, ambas son funciones continuas.

Luego, por teorema, $D_{\vec{u}}f(2, 0) = \langle \nabla f(2, 0), \vec{u} \rangle = \langle (e^0, 2e^0), (\frac{1}{2}, \frac{\sqrt{3}}{2}) \rangle = \frac{1}{2} + \sqrt{3} \ \blacksquare$