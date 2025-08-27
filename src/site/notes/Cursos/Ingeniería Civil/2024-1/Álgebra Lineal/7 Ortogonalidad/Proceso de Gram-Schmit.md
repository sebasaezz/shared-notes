---
{"dg-publish":true,"permalink":"/cursos/ingenieria-civil/2024-1/algebra-lineal/7-ortogonalidad/proceso-de-gram-schmit/","tags":["ExMAT1203"]}
---

# Concepto

Obtener la [[Cursos/Ingeniería Civil/2024-1/Álgebra Lineal/7 Ortogonalidad/Base ortogonal y ortonormal\|Base ortogonal y ortonormal]] de un espacio generado en $\mathbb{R}^{n}$.

# Definición

Se parte con un espacio generado $W=\operatorname{Gen}\{ \mathbf{v}_{1},\mathbf{v}_{2},\cdots,\mathbf{v}_{j} \}=\operatorname{Gen}B$ en $\mathbb{R}^{n}$, los vectores generadores no son ortogonales entre ellos.

Ahora se quiere obtener la base $U=\{ \mathbf{u}_{1},\mathbf{u}_{2},\cdots,\mathbf{u}_{j} \}$ ortogonal tal que $\operatorname{Gen}U=W$.

Se debe elegir un vector en $B$ para poner a todos los demás en relación a este. Se elige normalmente a $\mathbf{u}_{1}=\mathbf{v}_{1}$. Ahora encontrar $\mathbf{u}_{2}$ ortogonal a $\mathbf{u}_{1}$. Se calcula la [[Cursos/Ingeniería Civil/2024-1/Álgebra Lineal/7 Ortogonalidad/Proyección ortogonal y escalar\|Proyección ortogonal y escalar]] $p_{1}$ de $\mathbf{v}_{2}$ en $\operatorname{Gen}\{ \mathbf{u}_{1} \}$ ($\operatorname{Proj}_{\operatorname{Gen}\{ \mathbf{u}_{1} \}}\mathbf{v}_{2}=p_{1}$), se tendrá que $\mathbf{u}_{2}=\mathbf{v}_{2}-p_{1}$ (La [[Cursos/Ingeniería Civil/2024-1/Álgebra Lineal/7 Ortogonalidad/Proyección ortogonal y escalar#^0065a8\|componente ortogonal]] de $\mathbf{v}_{2}$ en $\mathbf{u}_{1}$) cumple el requerimiento.

Así se seguirá por tantos $j$ vectores en $B$:

> [!definition] proceso de Gram-Schmidt
> Dado el espacio $W=\operatorname{Gen}\{ \mathbf{v}_{1},\mathbf{v}_{2},\cdots,\mathbf{v}_{j} \}$ en $\mathbb{R}^{n}$.
> $$
> \begin{align}
> \mathbf{u}_{1} & =  \mathbf{v}_{1} \\
> \mathbf{u}_{2} & =  \mathbf{v}_{2}- \frac{\mathbf{v}_{2}·\mathbf{u}_{1}}{\mathbf{u}_{1}·\mathbf{u}_{1}}\mathbf{u}_{1} & = & \mathbf{v}_{2}-\operatorname{Proj}_{\operatorname{Gen}\{ \mathbf{u}_{1} \}}(\mathbf{v}_{2}) \\
> \mathbf{u}_{3} & =\mathbf{v}_{3}-\frac{\mathbf{v}_{3}·\mathbf{u}_{1}}{\mathbf{u}_{1}·\mathbf{u}_{1}}\mathbf{u}_{1} -\frac{\mathbf{v}_{3}·\mathbf{u}_{2}}{\mathbf{u}_{2}·\mathbf{u}_{2}}\mathbf{u}_{2} & = & \mathbf{v}_{3}-\operatorname{Proj}_{\operatorname{Gen}\{ \mathbf{u}_{1},\mathbf{u}_{2} \}}(\mathbf{v}_{3}) \\
>  &~ ~ \vdots &  &  \\
> \mathbf{u}_{j} & =\mathbf{v}_{j}-\frac{\mathbf{v}_{j}·\mathbf{u}_{1}}{\mathbf{u}_{1}·\mathbf{u}_{1}}\mathbf{u}_{1}-\frac{\mathbf{v}_{j}·\mathbf{u}_{2}}{\mathbf{u}_{2}·\mathbf{u}_{2}}\mathbf{u}_{2}-\dots-\frac{\mathbf{v}_{j}·\mathbf{u}_{j-1}}{\mathbf{u}_{j-1}·\mathbf{u}_{j-1}}\mathbf{u}_{j-1} & =  & \mathbf{v}_{j}-\operatorname{Proj}_{\operatorname{Gen}\{ \mathbf{u}_{1},\mathbf{u}_{2},\dots,\mathbf{u}_{j-1} \}}(\mathbf{v}_{j}) 
> \end{align}
> $$
> Entonces $\{ \mathbf{u}_{1},\mathbf{u}_{2},\dots,\mathbf{u}_{j} \}$ será una base ortogonal de $W$.
> Además se cumplirá que $\operatorname{Gen}\{ \mathbf{u}_{1},\dots,\mathbf{u}_{k} \}=\operatorname{Gen}\{ \mathbf{v}_{1},\dots,\mathbf{v}_{k} \}$.
