Para la demostración en particular de esta fórmula, debemos tener en cuenta otros teoremas previamente... 
****
#### 1 **Teorema** Si ($f^{(n+1)}$) es continua en un intervalo abierto ($I$) que contiene a ($a$), y ($x$) está en ($I$), entonces
$$R_n(x) = \frac{1}{n!} \int_a^x (x - t)^n f^{(n+1)}(t) dt$$
**Demostración** Usamos inducción matemática. Para ($n = 1$),
$$R_1(x) = f(x) - T_1(x) = f(x) - f(a) - f'(a)(x-a)$$
y la integral en el teorema es ($\int_a^x (x-t) f''(t) dt$). Para evaluar esta integral integramos por partes con ($u = x - t$) y ($dv = f''(t) dt$), así que ($du = -dt$) y ($v = f'(t)$). Por lo tanto
$$\int_a^x (x-t) f''(t) dt = [(x-t)f'(t)]_{t=a}^{t=x} + \int_a^x f'(t) dt$$
$$= 0 - (x-a)f'(a) + f(x) - f(a) \quad \text{(por TFC 2)}$$
$$= f(x) - f(a) - f'(a)(x-a) = R_1(x)$$
El teorema queda por lo tanto demostrado para ($n = 1$). Ahora suponemos que el Teorema 1 es verdadero para ($n = k$), esto es,
$$R_k(x) = \frac{1}{k!} \int_a^x (x - t)^k f^{(k+1)}(t) dt$$
Queremos demostrar que es verdadero para ($n = k + 1$), esto es
$$R_{k+1}(x) = \frac{1}{(k+1)!} \int_a^x (x - t)^{k+1} f^{(k+2)}(t) dt$$
Nuevamente usamos integración por partes, esta vez con ($u = (x-t)^{k+1}$) y ($dv = f^{(k+2)}(t)$). entonces
$du = -(k+1)(x-t)^k dt$ y $v = f^{(k+1)}(t)$, así que
$$\frac{1}{(k+1)!} \int_a^x (x - t)^{k+1} f^{(k+2)}(t) dt$$
$$= \frac{1}{(k+1)!} \left[ (x - t)^{k+1} f^{(k+1)}(t) \right]_{t=a}^{t=x} + \frac{k+1}{(k+1)!} \int_a^x (x - t)^k f^{(k+1)}(t) dt$$
$$= 0 - \frac{1}{(k+1)!} (x - a)^{k+1} f^{(k+1)}(a) + \frac{1}{k!} \int_a^x (x - t)^k f^{(k+1)}(t) dt$$
$$= -\frac{f^{(k+1)}(a)}{(k+1)!} (x - a)^{k+1} + R_k(x)$$
$$= f(x) - T_k(x) - \frac{f^{(k+1)}(a)}{(k+1)!} (x - a)^{k+1}$$
$$= f(x) - T_{k+1}(x) = R_{k+1}(x)$$
Por lo tanto, (1) es verdadera para ($n = k + 1$) cuando es verdadera para ($n = k$). Así, por inducción matemática, es verdadera para todo ($n$).
****
#### 2 **Teorema del Valor Medio Ponderado para Integrales.** Si ($f$) y ($g$) son continuas en ($[a, b]$) y ($g$) no cambia de signo en ($[a, b]$), entonces existe un número ($c$) en ($[a, b]$) tal que
$$\int_a^b f(x)g(x)dx = f(c) \int_a^b g(x)dx$$
**Demostración** Dado que ($g$) no cambia de signo, ($g(x) \ge 0$) o ($g(x) \le 0$) para todo ($a \le x \le b$). Por motivos de concreción, supongamos que ($g(x) \ge 0$). Por el **Teorema del Valor Extremo**, ($f$) tiene un mínimo absoluto ($m$) y un máximo absoluto ($M$), por lo que ($m \le f(x) \le M$) para ($a \le x \le b$). Dado que ($g(x) \ge 0$), tenemos
$$mg(x) \le f(x)g(x) \le Mg(x) \quad a \le x \le b$$
y entonces
($3$)
$$m \int_a^b g(x)dx \le \int_a^b f(x)g(x)dx \le M \int_a^b g(x)dx$$
Si ($\int_a^b g(x)dx = 0$), estas desigualdades muestran que ($\int_a^b f(x)g(x)dx = 0$) y entonces el Teorema 2 es verdadero porque ambos lados de la ecuación son 0. Si ($\int_a^b g(x)dx \neq 0$), debe ser positivo y podemos dividir por ($\int_a^b g(x)dx$) en ($3$):
$$m \le \frac{\int_a^b f(x)g(x)dx}{\int_a^b g(x)dx} \le M$$
Entonces, por el **Teorema del Valor Intermedio**, existe un número ($c$) en $[a, b]$ tal que
$$f(c) = \frac{\int_a^b f(x)g(x)dx}{\int_a^b g(x)dx} \quad \text{y entonces} \quad \int_a^b f(x)g(x)dx = f(c) \int_a^b g(x)dx$$
****
#### 4 **Teorema.** Si ($f^{(n+1)}$) es continua en un intervalo abierto ($I$) que contiene a ($a$), y ($x$) está en ($I$), entonces existe un número ($c$) entre ($a$) y ($x$) tal que
$$R_n(x) = \frac{f^{(n+1)}(c)}{(n+1)!} (x - a)^{n+1}$$
**Demostración.** La función ($g(t) = (x - t)^n$) no cambia de signo en el intervalo de ($a$) a ($x$), por lo que el Teorema del Valor Medio Ponderado para Integrales nos da un número ($c$) entre ($a$) y ($x$) tal que
$$\int_a^x (x - t)^n f^{(n+1)}(t) dt = f^{(n+1)}(c) \int_a^x (x - t)^n dt$$
$$= -f^{(n+1)}(c) \left[ \frac{(x - t)^{n+1}}{n+1} \right]_{t=a}^{t=x} = f^{(n+1)}(c) \frac{(x-a)^{n+1}}{n+1}$$
Entonces, por el Teorema 1,
$$R_n(x) = \frac{1}{n!} \int_a^x (x - t)^n f^{(n+1)}(t) dt$$
$$= \frac{1}{n!} f^{(n+1)}(c) \frac{(x-a)^{n+1}}{n+1} = \frac{f^{(n+1)}(c)}{(n+1)!} (x - a)^{n+1}$$
La fórmula para el término del residuo en el Teorema 4 se llama la **forma de Lagrange del término del residuo**. Observa que esta expresión

$$R_n(x) = \frac{f^{(n+1)}(c)}{(n+1)!} (x - a)^{n+1}$$
es muy similar a los términos de la serie de Taylor excepto que ($f^{(n+1)}$) se evalúa en ($c$) en lugar de ($a$). Todo lo que podemos decir sobre el número ($c$) es que se encuentra en algún lugar entre ($x$) y ($a$).


****
--8<-- "includes/fuente.md"
