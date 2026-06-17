**Ejemplo 1.** Evalúe $f(3, 2)$; determine y trace el dominio. 
$f(x, y) = \frac{\sqrt{x + y + 1}}{x - 1}$
luego $f(3, 2) = \frac{\sqrt{3 + 2 + 1}}{3 - 1} = \frac{\sqrt{6}}{2}$

La expresión para $f$ tiene sentido si el denominador no es $0$ y la cantidad bajo el signo de raíz cuadrada es no negativa. Así, el dominio de $f$ es

$$
D = \{(x, y) \mid x + y + 1 \ge 0, x \neq 1\}
$$

La desigualdad $x + y + 1 \ge 0$, o $y \ge -x - 1$ describe los puntos que se encuentran en o sobre la recta $y = -x - 1$, mientras que $x \neq 1$ significa que los puntos sobre la recta $x = 1$ deben excluirse del dominio.
![[Pasted image 20260515164904.png]]
****
**Ejemplo 2.** Determine el dominio y el rango de $g(x, y) = \sqrt{9 - x^2 - y^2}$.
El dominio de $g$ es
$$
D = \{(x, y) \mid 9 - x^2 - y^2 \ge 0\} = \{(x, y) \mid x^2 + y^2 \le 9\}
$$

el cual es un disco con centro $(0, 0)$ y radio $3$. El rango de $g$ es

$$
\{z \mid z = \sqrt{9 - x^2 - y^2}, (x, y) \in D\}
$$

Como $z$ es una raíz cuadrada positiva, $z \ge 0$. Asimismo, como $9 - x^2 - y^2 \le 9$, se tiene

$$
\sqrt{9 - x^2 - y^2} \le 3
$$

Así, el rango es

$$
\{z \mid 0 \le z \le 3\} = [0, 3]
$$
... Y para este último ejemplo agregamos la gráfica del mismo, que refiere a otro concepto en funciones de varias variables, ya que estamos:
![[Pasted image 20260516182645.png]]

****
--8<-- "includes/fuente.md"
