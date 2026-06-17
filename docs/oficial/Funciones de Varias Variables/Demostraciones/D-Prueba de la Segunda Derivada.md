**Prueba de la segunda derivada.** Suponga que las segundas derivadas parciales de $f$ son continuas en un disco con centro $(a, b)$ y que $f_x(a, b) = 0$ y $f_y(a, b) = 0$ (es decir, que $(a, b)$ es un punto crítico de $f$). Sea

$$
D = D(a, b) = f_{xx}(a, b)f_{yy}(a, b) - [f_{xy}(a, b)]^2
$$

(a) Si $D > 0$ y $f_{xx}(a, b) > 0$, entonces $f(a, b)$ es un mínimo local.
(b) Si $D > 0$ y $f_{xx}(a, b) < 0$, entonces $f(a, b)$ es un máximo local.
(c) Si $D < 0$, entonces $f(a, b)$ no es un máximo ni un mínimo local.
****
**Demostración.** **PARTE (a).** Calcule la derivada direccional de segundo orden de $f$ en la dirección de $\mathbf{u} = \langle h, k \rangle$. La derivada de primer orden está dada por el teorema del inciso [[7.Derivada Direccional]]:

$$
D_{\mathbf{u}}f = f_x h + f_y k
$$

Al aplicar este teorema por segunda vez se tiene

$$
\begin{aligned}
D_{\mathbf{u}}^2 f &= D_{\mathbf{u}}(D_{\mathbf{u}}f) = \frac{\partial}{\partial x}(D_{\mathbf{u}}f)h + \frac{\partial}{\partial y}(D_{\mathbf{u}}f)k \\
&= (f_{xx}h + f_{yx}k)h + (f_{xy}h + f_{yy}k)k \\
&= f_{xx}h^2 + 2f_{xy}hk + f_{yy}k^2 \quad (\text{por el teorema de Clairaut})
\end{aligned}
$$

Si se completa el cuadrado en esta expresión se obtiene

$$
D_{\mathbf{u}}^2 f = f_{xx} \left( h + \frac{f_{xy}}{f_{xx}}k \right)^2 + \frac{k^2}{f_{xx}}(f_{xx}f_{yy} - f_{xy}^2)
$$
Si reescribimos la ecuación con esa $D$, queda así:
$$D_{\mathbf{u}}^2 f = f_{xx} \left( h + \frac{f_{xy}}{f_{xx}}k \right)^2 + \frac{k^2}{f_{xx}} D$$
Vemos que $\left( h + \frac{f_{xy}}{f_{xx}}k \right)^2$ **siempre es positivo o cero.** Tal como $k^2$ por misma razón.
Como los términos al cuadrado son inofensivos (no cambian signos), nos interesan los valores de $f_{xx}$ y de $D$, para determinar el comportamiento de la función en $f(a, b)$.
Recordemos que estamos en el caso (a):
Se dio que $f_{xx}(a, b) > 0$ y $D(a, b) > 0$. Pero $f_{xx}$ y $D = f_{xx}f_{yy} - f_{xy}^2$ son funciones continuas, así que existe un disco $B$ con centro $(a, b)$ y radio $\delta > 0$ tal que $f_{xx}(x, y) > 0$ y $D(x, y) > 0$ siempre que $(x, y)$ está en $B$. Por tanto, al examinar la ecuación se advierte que $D_{\mathbf{u}}^2 f(x, y) > 0$ cada vez que $(x, y)$ está en $B$. Esto significa que si $C$ es la curva obtenida de la intersección de la gráfica de $f$ con el plano vertical que pasa por $P(a, b, f(a, b))$ en la dirección de $\mathbf{u}$, $C$ es cóncava hacia arriba en un intervalo de longitud $2\delta$. Esto es cierto en la dirección de todos los vectores $\mathbf{u}$, de modo que si se restringe $(x, y)$ a $B$, la gráfica de $f$ reside arriba de su plano tangente horizontal en $P$. Así, $f(x, y) \ge f(a, b)$ cada vez que $(x, y)$ está en $B$. Esto demuestra que $f(a, b)$ es un mínimo local. $\blacksquare$

****
--8<-- "includes/fuente.md"
