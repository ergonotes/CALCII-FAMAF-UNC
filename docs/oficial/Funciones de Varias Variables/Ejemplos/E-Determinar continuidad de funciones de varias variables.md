**Ejemplo 1.** ¿Dónde es continua la función $f(x, y) = \frac{x^2 - y^2}{x^2 + y^2}$?

**Solución.** La función $f$ es discontinua en $(0, 0)$ porque no está definida ahí. Como $f$ es una función racional, es continua en su dominio, el cual es el conjunto
$D = \{(x, y) \mid (x, y) \neq (0, 0)\}$. $\blacksquare$
****
**Ejemplo 2.** Sea

$$
f(x, y) = \begin{cases} 
      \frac{3x^2y}{x^2 + y^2} & \text{si } (x, y) \neq (0, 0) \\
      0 & \text{si } (x, y) = (0, 0) 
   \end{cases}
$$

Se sabe que $f$ es continua para $(x, y) \neq (0, 0)$, ya que ahí es igual a una función racional. Asimismo, del ejemplo 3 del inciso [[E-Determinar limites de funciones de varias variables]], se tiene

$$
\lim_{(x, y) \to (0, 0)} f(x, y) = \lim_{(x, y) \to (0, 0)} \frac{3x^2y}{x^2 + y^2} = 0 = f(0, 0)
$$

Por tanto, $f$ es continua en $(0, 0)$, y en consecuencia es continua en $\mathbb{R}^2$. $\blacksquare$
****
**Ejemplo 3.** ¿Dónde es continua la función $h(x, y) = \arctan(y/x)$?

**Solución.** La función $f(x, y) = y/x$ es una función racional, y por tanto continua excepto en la recta $x = 0$. La función $g(t) = \arctan t$ es continua en todas partes. Así, la función compuesta

$$
g(f(x, y)) = \arctan(y/x) = h(x, y)
$$

es continua excepto en $x = 0$. La gráfica de la figura 9 muestra la interrupción en la gráfica de $h$ arriba del eje $y$. $\blacksquare$
![[Pasted image 20260517111030.png]]

****
--8<-- "includes/fuente.md"
