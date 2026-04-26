Para ver por qué es cierto para $n=1$, supongamos que $|f''(x)| \leq M$. En particular, se tiene $f''(x) \leq M$, de tal manera que para $a \leq x \leq a + d$ tenemos
$$\int_{a}^{x} f''(t) dt \leq \int_{a}^{x} M dt$$
Una antiderivada de $f''$ es $f'$, por lo que según la parte 2 del teorema fundamental del cálculo tenemos
$$f'(x) - f'(a) \leq M(x - a) \quad \text{o bien } f'(x) \leq f'(a) + M(x - a)$$
Así que
$$\int_{a}^{x} f'(t) dt \leq \int_{a}^{x} [f'(a) + M(t-a)] dt$$
$$f(x) - f(a) \leq f'(a)(x-a) + M \frac{(x-a)^2}{2}$$
$$f(x) - f(a) - f'(a)(x-a) \leq \frac{M}{2}(x-a)^2$$
Pero $R_1(x) = f(x) - T_1(x) = f(x) - f(a) - f'(a)(x-a)$. De modo que
$$R_1(x) \leq \frac{M}{2}(x-a)^2$$
Un razonamiento similar, aplicando $f''(x) \geq -M$, demuestra que
$$R_1(x) \geq -\frac{M}{2}(x-a)^2$$
De manera que
$$|R_1(x)| \leq \frac{M}{2}|x-a|^2$$
Aunque hemos supuesto que $x > a$, cálculos similares muestran que esta desigualdad es válida también para $x < a$.
Esto demuestra la desigualdad de Taylor para el caso donde $n = 1$. El resultado para cualquier $n$ se demuestra de manera parecida integrando $n + 1$ veces. 