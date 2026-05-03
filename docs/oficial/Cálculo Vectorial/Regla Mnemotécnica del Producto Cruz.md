Armas tu matriz así, poniendo $\mathbf{i, j, k}$ (que representan a $x, y, z$) en el techo:
$$
\begin{vmatrix}
\mathbf{i} & \mathbf{j} & \mathbf{k} \\
u_1 & u_2 & u_3 \\
v_1 & v_2 & v_3
\end{vmatrix}
$$
*   **Para la coordenada $\mathbf{i}$ (la $x$):** Con tu dedo, tapa toda la columna de la $\mathbf{i}$. Te quedan cuatro números a la derecha. Multiplícalos en cruz (diagonal principal menos diagonal secundaria): $(u_2v_3 - u_3v_2)$.
*   **Para la coordenada $\mathbf{j}$ (la $y$):** Tapa la columna de la $\mathbf{j}$. Multiplica en cruz lo que queda a los lados: $(u_1v_3 - u_3v_1)$. 
*   **Para la coordenada $\mathbf{k}$ (la $z$):** Tapa la columna de la $\mathbf{k}$. Multiplica en cruz lo que te quedó a la izquierda: $(u_1v_2 - u_2v_1)$.
Luego, con Si $\mathbf{v} = \langle v_1, v_2, v_3 \rangle$ y $\mathbf{u} = \langle u_1, u_2, u_3 \rangle$, el **producto cruz** de $\mathbf{v}$ y $\mathbf{u}$ es el vector
$$\mathbf{v} \times \mathbf{u} = \langle v_2u_3 - v_3u_2, \ v_3u_1 - v_1u_3, \ v_1u_2 - v_2u_1 \rangle$$