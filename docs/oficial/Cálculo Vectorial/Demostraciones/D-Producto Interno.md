Teniendo la figura:

![[Pasted image 20260502112319.png]]

Queremos demostrar que:
Si $\theta$ es el ángulo entre los vectores $\mathbf{a}$ y $\mathbf{b}$, entonces
$$ \mathbf{a} \cdot \mathbf{b} = \|\mathbf{a}\| \|\mathbf{b}\| \cos \theta $$
****

**Demostración**. Si se aplica la ley de los cosenos al triángulo $OAB$ de la figura, se obtiene

$$|AB|^2 = |OA|^2 + |OB|^2 - 2 |OA| |OB| \cos \theta$$

(Observe que la ley de los cosenos no deja de aplicarse en los casos límite en que $\theta = 0$ o $\pi$, o $OA = \mathbf{0}$ o $OB = \mathbf{0}$.)

Pero $|OA| = \|\mathbf{a}\|$, $|OB| = \|\mathbf{b}\|$ y $|AB| = \|\mathbf{a} - \mathbf{b}\|$, así que la ecuación se convierte en

$$ \|\mathbf{a} - \mathbf{b}\|^2 = \|\mathbf{a}\|^2 + \|\mathbf{b}\|^2 - 2 \|\mathbf{a}\| \|\mathbf{b}\| \cos \theta $$

Si se usan las propiedades 1, 2 y 4 del producto punto, el miembro izquierdo de esta ecuación puede reescribirse como sigue:

$$ \|\mathbf{a} - \mathbf{b}\|^2 = (\mathbf{a} - \mathbf{b}) \cdot (\mathbf{a} - \mathbf{b}) $$

$$ = \mathbf{a} \cdot \mathbf{a} - \mathbf{a} \cdot \mathbf{b} - \mathbf{b} \cdot \mathbf{a} + \mathbf{b} \cdot \mathbf{b} $$

$$ = \|\mathbf{a}\|^2 - 2 \mathbf{a} \cdot \mathbf{b} + \|\mathbf{b}\|^2 $$

Por tanto, la ecuación 5 da

$$ \|\mathbf{a}\|^2 - 2 \mathbf{a} \cdot \mathbf{b} + \|\mathbf{b}\|^2 = \|\mathbf{a}\|^2 + \|\mathbf{b}\|^2 - 2 \|\mathbf{a}\| \|\mathbf{b}\| \cos \theta $$

Así,

$$ -2 \mathbf{a} \cdot \mathbf{b} = -2 \|\mathbf{a}\| \|\mathbf{b}\| \cos \theta $$

o

$$ \mathbf{a} \cdot \mathbf{b} = \|\mathbf{a}\| \|\mathbf{b}\| \cos \theta $$