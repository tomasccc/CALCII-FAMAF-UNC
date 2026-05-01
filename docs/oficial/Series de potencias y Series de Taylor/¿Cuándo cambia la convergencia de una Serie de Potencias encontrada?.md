Multiplicar por un monomio (como $x$, $x^2$, $5x$) o sumar un término finito (como sumar $+5$ o $+x^3$) NUNCA altera el radio de convergencia de una serie. Y de hecho, tiene sentido si pensamos la serie expresada con sus sumas parciales.
Sin embargo, el radio **sí se altera** cuando interactúan dos series completas o cuando modificamos el "corazón" de la función.
****
### **Suma o Resta de dos Series**
Si sumamos una función con términos infinitos con otra función con términos infinitos, el radio de convergencia del resultado será **el más pequeño de los dos**.
- Supongamos sumamos $e^x$ (que converge en todo $R$, o sea $R_1​=∞$) con $\frac{1}{1-x}$​ (que es una serie geométrica que solo converge entre $−1$ y $1$, o sea $R_2​=1$).
- La nueva función combinada $e^x+\frac{1}{1-x}$​ colapsará (tendrá una asíntota) en $x=1$.
- **Regla:** El nuevo radio será $R=\text{min}(R_1​,R_2​)$.
La exepción se dá cuando las funciones se cancelan al sumarse. Por ejemplo, $f(x)$ y $-f(x)$ ambas con $R=1$, el resultado al sumarlas es $0$, y el radio es $R = \infty$, ya que la expresión siempre converge a $0$.
****
### **Sustitución**
* Si tenemos una serie para $f(u)$ que converge solo para $|u| < 1$ (es decir, $R = 1$).
* Y decidimos sustituir $u = 3x$.
* Ahora la condición de convergencia es $|3x| < 1$, lo que significa que $|x| < \frac{1}{3}$.
* Ahora $R = \frac{1}{3}$
(Si tenemos una función como seno por ejemplo, al encontrar su serie de taylor nos encontraremos con que es válida para todo $x$. Luego si sustituimos el argumento del seno, la función seguirá siendo válida para todo $x$).
