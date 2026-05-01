Del ejemplo 1 de **[[E-Serie de Taylor y Maclaurin]]**, se concluye que $e^x$ tiene un desarrollo en serie de potencias en $0$, entonces 
$$e^x = \sum_{n=0}^{\infty} \frac{x^n}{n!}$$
Así que, **¿cómo podemos determinar si ($e^x$) tiene una representación como serie de potencias?**
Investiguemos la cuestión más general: **¿en qué circunstancias una función es igual a la suma de su serie de Taylor?** En otras palabras, si ($f$) tiene derivadas de todos los órdenes, cuándo es cierto que
$$f(x) = \sum_{n=0}^{\infty} \frac{f^{(n)}(a)}{n!} (x-a)^n$$
Como sucede con cualquier serie convergente (de lo contrario no estarían definidas las derivadas $f^{(n)}$), esto quiere decir que ($f(x)$) es el límite de la sucesión de sumas parciales. En el caso de la serie de Taylor, las sumas parciales son
$$T_n(x) = \sum_{i=0}^{n} \frac{f^{(i)}(a)}{i!} (x - a)^i$$
$$= f(a) + \frac{f'(a)}{1!} (x - a) + \frac{f''(a)}{2!} (x - a)^2 + \cdots + \frac{f^{(n)}(a)}{n!} (x - a)^n$$
Observe que ($T_n$) es una polinomial de grado ($n$) llamado [[Polinomio-de-Taylor]].
En general, ($f(x)$) es la suma de su serie de Taylor si$$f(x) = \lim_{n \to \infty} T_n(x)$$Si hacemos
$$R_n(x) = f(x) - T_n(x) \quad \text{de manera que} \quad f(x) = T_n(x) + R_n(x)$$
entonces ($R_n(x)$) se llama residuo de la serie de Taylor. Si podemos de alguna manera demostrar que ($\lim_{n \to \infty} R_n(x) = 0$), entonces se sigue que
$$\lim_{n \to \infty} T_n(x) = \lim_{n \to \infty} [f(x) - R_n(x)] = f(x) - \lim_{n \to \infty} R_n(x) = f(x)$$
****
#### **Otra forma de verlo**
Adjuntamos el teorema del inciso [[Series de Taylor y Maclaurin]]...
Sea $f$ una función tal que existe $f^{(n)}$ $\forall n \ge 0$. Se cumple
$$ f(x) = \sum_{n=0}^{\infty} \frac{f^{(n)}(a)}{n!} (x-a)^n \quad \forall x \in (a-c, a+c) \iff \lim_{n \to \infty} R_{n,a}(x) = 0 \quad \forall x \in (a-c, a+c). $$
**Demostración.**
($\Rightarrow$) Supongamos que $$f(x) = \sum_{n=0}^{\infty} \frac{f^{(n)}(a)}{n!} (x-a)^n$$Entonces por definición de serie tenemos que $f(x) = \lim_{n \to \infty} T_{n,a}(x)$ (límite de sumas parciales).
Luego, $$\lim_{n \to \infty} R_{n,a}(x) = \lim_{n \to \infty} (f(x) - T_{n,a}(x)) = \lim_{n \to \infty} f(x) - \lim_{n \to \infty} T_{n,a}(x) = f(x) - f(x) = 0$$
($\Leftarrow$) Si $\lim_{n \to \infty} R_{n,a}(x) = 0$ $\forall x \in (a-c, a+c)$, entonces
$$\lim_{n \to \infty} T_{n,a}(x) = \lim_{n \to \infty} (f(x) - R_{n,a}(x)) = \lim_{n \to \infty} f(x) - \lim_{n \to \infty} R_{n,a}(x) = f(x) - 0 = f(x)$$
Luego, por definición $f(x) = \sum_{n=0}^{\infty} \frac{f^{(n)}(a)}{n!} (x-a)^n$ $\forall x \in (a-c, a+c)$.
