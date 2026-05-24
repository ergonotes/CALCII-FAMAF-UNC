$$\mathbf{u} = \frac{\mathbf{v}}{||\mathbf{v}||}$$
****
Tomemos un vector cualquiera $\mathbf{v} = \langle x, y \rangle$.
Sabemos por Pitágoras que su longitud original es:

$$L = \sqrt{x^2 + y^2}$$

El proceso de normalización nos dice que debemos dividir el vector entre su longitud $L$.

$$\mathbf{u} = \frac{\mathbf{v}}{L} = \left\langle \frac{x}{L}, \frac{y}{L} \right\rangle$$

Ahora, **¿Cuál es la longitud de este nuevo vector $\mathbf{u}$?**
Vamos a aplicarle la fórmula de Pitágoras a nuestro nuevo vector $\mathbf{u}$:
$$||\mathbf{u}|| = \sqrt{\left(\frac{x}{L}\right)^2 + \left(\frac{y}{L}\right)^2}$$
$$||\mathbf{u}|| = \sqrt{\frac{x^2}{L^2} + \frac{y^2}{L^2}}$$
$$||\mathbf{u}|| = \sqrt{\frac{x^2 + y^2}{L^2}}$$Al principio definimos que $L = \sqrt{x^2 + y^2}$, lo que significa que **$L^2 = x^2 + y^2$**. Luego
$$||\mathbf{u}|| = \sqrt{\frac{L^2}{L^2}}$$
$$||\mathbf{u}|| = \sqrt{1}$$
$$||\mathbf{u}|| = \mathbf{1}$$