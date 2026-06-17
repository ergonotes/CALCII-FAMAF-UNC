**Ejemplo 1.** Si $f(x, y) = xy / (x^2 + y^2)$, ¿existe el $\lim_{(x, y) \to (0, 0)} f(x, y)$?

**Solución.** Si $y = 0$, entonces $f(x, 0) = 0/x^2 = 0$. Por tanto,
$$
f(x, y) \to 0 \quad \text{cuando} \quad (x, y) \to (0, 0) \text{ a lo largo del eje } x
$$
Si $x = 0$, entonces $f(0, y) = 0/y^2 = 0$, así que
$$
f(x, y) \to 0 \quad \text{cuando} \quad (x, y) \to (0, 0) \text{ a lo largo del eje } y
$$

Aunque se han obtenido límites idénticos a lo largo de los ejes, eso no demuestra que el límite dado sea de 0. Aproxime ahora $(0, 0)$ a lo largo de otra recta, por decir $y = x$. Para todas las $x \neq 0$,
$$
f(x, x) = \frac{x^2}{x^2 + x^2} = \frac{1}{2}
$$
Por tanto, $f(x, y) \to \frac{1}{2}$ cuando $(x, y) \to (0, 0)$ a lo largo de $y = x$. Como se han obtenido límites diferentes a lo largo de trayectorias diferentes, el límite dado no existe. $\blacksquare$
![[Pasted image 20260516194216.png]]
En la figura siguiente se explica con más claridad el ejemplo. La cresta que se forma arriba de la recta $y = x$ se corresponde con el hecho de que $f(x, y) = \frac{1}{2}$ para todos los puntos $(x, y)$ en esa recta, excepto en el origen.
![[Pasted image 20260516194321.png]]
****
**Ejemplo 2.** Si $f(x, y) = \frac{xy^2}{x^2 + y^4}$, ¿existe el $\lim_{(x, y) \to (0, 0)} f(x, y)$?

**Solución.** Con la solución del ejemplo 2 en mente, intente ahorrar tiempo permitiendo que $(x, y) \to (0, 0)$ a lo largo de cualquier recta que pasa por el origen. Si la recta no es el eje $y$, entonces $y = mx$, donde $m$ es la pendiente, y

$$
f(x, y) = f(x, mx) = \frac{x(mx)^2}{x^2 + (mx)^4} = \frac{m^2x^3}{x^2 + m^4x^4} = \frac{m^2x}{1 + m^4x^2}
$$

Así, $f(x, y) \to 0$ cuando $(x, y) \to (0, 0)$ a lo largo de $y = mx$.

Se obtiene el mismo resultado que $(x, y) \to (0, 0)$ a lo largo de la recta $x = 0$. Así, $f$ tiene el mismo valor límite a lo largo de todas las rectas que pasan por el origen. Sin embargo, eso no demuestra que el límite dado sea de 0, porque si ahora se permite que $(x, y) \to (0, 0)$ a lo largo de la parábola $x = y^2$, se tiene

$$
f(x, y) = f(y^2, y) = \frac{y^2 \cdot y^2}{(y^2)^2 + y^4} = \frac{y^4}{2y^4} = \frac{1}{2}
$$

de manera $f(x, y) \to \frac{1}{2}$ cuando $(x, y) \to (0, 0)$ a lo largo de $x = y^2$.

Como trayectorias distintas conducen a valores límite diferentes, el límite dado no existe. $\blacksquare$
****
**Ejemplo 3.** Determine si existe $$\lim_{(x, y) \to (0, 0)} \frac{3x^2y}{x^2 + y^2}$$
**Solución.** Como en el ejemplo anterior, se podría demostrar que el límite a lo largo de cualquier recta que pasa por el origen es 0. Esto no prueba que el límite dado sea de 0, pero los límites a lo largo de las parábolas $y = x^2$ y $x = y^2$ también resultan ser de 0, de manera que empiece a sospechar que ese límite sí existe y es igual a 0.
Sea $\varepsilon > 0$. Se quiere encontrar $\delta > 0$ tal que
$$
\text{si} \quad 0 < \sqrt{x^2 + y^2} < \delta \quad \text{entonces} \quad \left| \frac{3x^2y}{x^2 + y^2} - 0 \right| < \varepsilon
$$
es decir que si $\quad 0 < \sqrt{x^2 + y^2} < \delta \quad \text{entonces} \quad \frac{3x^2|y|}{x^2 + y^2} < \varepsilon$

Pero $x^2 \le x^2 + y^2$ ya que $y^2 \ge 0$, de modo que $x^2 / (x^2 + y^2) \le 1$ y por tanto

$$
\frac{3x^2|y|}{x^2 + y^2} \le 3|y| = 3\sqrt{y^2} \le 3\sqrt{x^2 + y^2}
$$

Así, si elige $\delta = \varepsilon / 3$ y considera $0 < \sqrt{x^2 + y^2} < \delta$, entonces
$$
\left| \frac{3x^2y}{x^2 + y^2} - 0 \right| \le 3\sqrt{x^2 + y^2} < 3\delta = 3\left(\frac{\varepsilon}{3}\right) = \varepsilon
$$

De ahí que, por la definición,
$$
\lim_{(x, y) \to (0, 0)} \frac{3x^2y}{x^2 + y^2} = 0
$$ $\blacksquare$


****
--8<-- "includes/fuente.md"
