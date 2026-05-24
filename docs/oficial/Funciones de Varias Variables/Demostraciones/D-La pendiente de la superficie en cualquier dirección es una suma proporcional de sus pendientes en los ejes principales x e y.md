**Teorema.** Si $f$ es una función derivable de $x$ y $y$ entonces $f$ tiene una derivada direccional en la dirección de cualquier vector unitario $\mathbf{u} = \langle a, b \rangle$ y
$$
D_{\mathbf{u}}f(x, y) = f_x(x, y)a + f_y(x, y)b
$$
****
**Demostración.** Si se define una función $g$ de la variable $h$ mediante
$$
g(h) = f(x_0 + ha, y_0 + hb)
$$
por la definición de una derivada se tiene
$$
(4) \ \ \quad g'(0) = \lim_{h \to 0} \frac{g(h) - g(0)}{h} = \lim_{h \to 0} \frac{f(x_0 + ha, y_0 + hb) - f(x_0, y_0)}{h} = D_{\mathbf{u}}f(x_0, y_0)
$$
Por otro lado, se puede escribir $g(h) = f(x, y)$, donde $x = x_0 + ha$, $y = y_0 + hb$, de forma que la [[6.Regla de la Cadena]] da

$$
g'(h) = \frac{\partial f}{\partial x} \frac{dx}{dh} + \frac{\partial f}{\partial y} \frac{dy}{dh} = f_x(x, y)a + f_y(x, y)b
$$
Si se pone ahora $h = 0$, entonces $x = x_0$, $y = y_0$ y
$$ (5) \ \quad
g'(0) = f_x(x_0, y_0)a + f_y(x_0, y_0)b
$$
Al comparar las ecuaciones 4 y 5 se observa que

$$
D_{\mathbf{u}}f(x_0, y_0) = f_x(x_0, y_0)a + f_y(x_0, y_0)b \quad \blacksquare
$$

