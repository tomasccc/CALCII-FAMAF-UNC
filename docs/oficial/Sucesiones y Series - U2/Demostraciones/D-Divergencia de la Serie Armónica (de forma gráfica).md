Graficamos la función $y=\frac{1}{x}$
![[Pasted image 20260401153602.png]]
Nos vamos a enfocar en un bloque arbitrario de términos que empieza en un número $c$ y termina en su cuadrado, $c^2$.
Los rectángulos azules representan los términos de la serie armónica. El ancho de cada rectángulo es 1. Por lo que, el área de cada rectángulo es exactamente su altura ($\frac{1}{c+1}, \frac{1}{c+2}$, etc.).
Queremos ver cuánto suman como mínimo los rectángulos azules de ese bloque, la imagen dibuja un rectángulo rojo por debajo de todos ellos.
*   La base del rectángulo rojo: Va desde $x = c$ hasta $x = c^2$. Su longitud es la diferencia: $c^2 - c$.
*   La altura del rectángulo rojo: Como la curva va bajando, el rectángulo azul más pequeño de ese bloque es el último, cuya altura es $\frac{1}{c^2}$. El rectángulo rojo usa esta altura mínima.
*   El área del rectángulo rojo: Base $\times$ Altura.
$$
(c^2 - c) \cdot \frac{1}{c^2} = \frac{c^2}{c^2} - \frac{c}{c^2} = 1 - \frac{1}{c}
$$

**La Primera Desigualdad**
Es evidente a simple vista que los rectángulos azules juntos son más grandes (tienen más área) que el rectángulo rojo que está debajo de ellos. Matemáticamente, esto se escribe como la primera línea de ecuaciones de la imagen:
$$
\frac{1}{c+1} + \frac{1}{c+2} + \frac{1}{c+3} + \cdots + \frac{1}{c^2} \ge 1 - \frac{1}{c}
$$
**La magia del $\ge$ 1**
Si sumamos el término $\frac{1}{c}$ a ambos lados:
$$
\frac{1}{c} + \frac{1}{c+1} + \frac{1}{c+2} + \cdots + \frac{1}{c^2} \ge 1
$$
¿Qué significa esto? que cualquier bloque de la serie armónica que empiece en el término $\frac{1}{c}$ y termine en el término $\frac{1}{c^2}$, suma obligatoriamente un número mayor o igual a 1.
Los sucesivos bloques de la serie indican:
$$
\frac{1}{1} \ge 1
$$
$$
\frac{1}{2} + \frac{1}{3} + \frac{1}{4} \ge 1
$$
$$
\frac{1}{5} + \cdots + \frac{1}{25} \ge 1
$$
$$
\frac{1}{26} + \cdots + \frac{1}{26^2} \ge 1
$$
Como la serie es infinita, podemos seguir armando estos bloques para siempre. Si sumamos todos los bloques, estamos sumando algo que es mayor o igual a sumar "unos" infinitamente:
$$
\sum_{n=1}^\infty \frac{1}{n} \ge \sum_{i=1}^\infty 1= 1 + 1 + 1 + 1 + \cdots = \infty
$$