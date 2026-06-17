**Ejemplo 1.** Sea $f(x, y) = x^2 + y^2 - 2x - 6y + 14$. Entonces,
$$
f_x(x, y) = 2x - 2 \quad f_y(x, y) = 2y - 6
$$
Estas derivadas parciales son iguales a 0 cuando $x = 1$ y $y = 3$, así que el único punto crítico es $(1, 3)$. Al completar el cuadrado se descubre que
$$
f(x, y) = 4 + (x - 1)^2 + (y - 3)^2
$$
Como $(x - 1)^2 \ge 0$ y $(y - 3)^2 \ge 0$, se tiene $f(x, y) \ge 4$ para todos los valores de $x$ e $y$. Por tanto, $f(1, 3) = 4$ es un mínimo local, y de hecho es el mínimo absoluto de $f$. Esto puede confirmarse geométricamente en la gráfica de $f$, que es el paraboloide elíptico con vértice $(1, 3, 4)$ que aparece en la figura 2. $\blacksquare$
****
**Ejemplo 2.** Determine los valores extremos de $f(x, y) = y^2 - x^2$.

**Solución.** Como $f_x = -2x$ y $f_y = 2y$, el único punto crítico es $(0, 0)$. Nótese que para puntos en el eje $x$ se tiene $y = 0$, así que $f(x, y) = -x^2 < 0$ (si $x \neq 0$). Sin embargo, para puntos en el eje $y$ se tiene $x = 0$, así que $f(x, y) = y^2 > 0$ (si $y \neq 0$). En consecuencia, todos los discos con centro $(0, 0)$ contienen puntos donde $f$ adopta valores positivos, así como puntos en los que $f$ adopta valores negativos. Por tanto, $f(0, 0) = 0$ no puede ser un valor extremo para $f$, por lo que $f$ no tiene ningún valor extremo. $\blacksquare$

****
--8<-- "includes/fuente.md"
