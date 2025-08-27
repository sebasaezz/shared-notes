---
{"dg-publish":true,"permalink":"/cursos/ingenieria-civil/2024-1/algebra-lineal/7-ortogonalidad/complemento-ortogonal-de-un-subespacio-y-ortogonalidad-de-espacios-fila-y-columna/","tags":["ExMAT1203"]}
---

# Concepto

Para un espacio que tenga un subespacio, existirá un espacio de vectores fuera del subespacio que sean ortogonales a todo vector en el subespacio.

# Complemento ortogonal de un subespacio

> [!definition] complemento ortogonal de un subespacio
> Si un vector $\mathbf{z}$ en el espacio es [[Cursos/Ingeniería Civil/2024-1/Álgebra Lineal/7 Ortogonalidad/Ortogonalidad entre vectores#^f532de\|ortogonal]] a todo vector de un subespacio $W\in\mathbb{R}^{n}$, entonces $\mathbf{z}$ es ortogonal a $W$. El conjunto de todos los $\mathbf{z}$ que son ortogonales  a $W$ se denomina complemento ortogonal de $W$, y se designa como $W^{\perp}$ (perpendicular a $W$).
> Siempre se cumplirá que:
> - $\mathbf{x}\in W^{\perp}\iff \mathbf{x}·\mathbf{z}=0: \mathbf{z}\in W$ Es decir, un vector $\mathbf{x}$ está en $W^{\perp}$ si y solo si es ortogonal a todo vector y conjunto que genera $W$.
> - $W^{\perp } \subseteq   \mathbb{R}^{n}$

# Ortogonalidad de espacios fila y columna

> [!theorem] Ortogonalidad de espacios fila y columna de una matriz
> Dada una matriz $A_{m\times n}$ se cumplirá siempre que sus espacios fila nulo serán complementos ortogonales de la siguiente forma:
> - $(\operatorname{fila}A)^{\perp}=\operatorname{nul}A$
> - $(\operatorname{nul}A)^{\perp}=\operatorname{col}A^{T}$

# Ejemplo
## Ejemplo Gráfico

Sea $W$ un [[Cursos/Ingeniería Civil/2024-1/Álgebra Lineal/5 Subespacios y Dimension/Espacio vectorial\|espacio]] en $\mathbb{R}^{3}$ con [[Cursos/Ingeniería Civil/2024-1/Álgebra Lineal/5 Subespacios y Dimension/Dimensión de un espacio vectorial\|dimensión]] $2$ (plano), y $L$ uno con dimensión $1$ (recta), tal que la recta pase de forma perpendicular al plano y por el $\mathbf{0}$, entonces $L$ será $W^{\perp}$, se cumplirá que el ángulo formado por todo $w \in W$ con todo $z\in L$ será de $90º$.

Además se cumplirá que $W=L^{\perp}$, ya que no hay otro subespacio que cumpla la [[Cursos/Ingeniería Civil/2024-1/Álgebra Lineal/7 Ortogonalidad/Ortogonalidad entre vectores\|ortogonalidad]].

Notar que para que sean [[Cursos/Ingeniería Civil/2024-1/Álgebra Lineal/5 Subespacios y Dimension/Subespacios vectoriales#^cca75d\|subespacios]] tiene que pasar por el $\mathbf{0}$.

![Pasted image 20240614192832.png](/img/user/Cursos/Ingenier%C3%ADa%20Civil/2024-1/%C3%81lgebra%20Lineal/7%20Ortogonalidad/attachments/Pasted%20image%2020240614192832.png)