---
{"dg-publish":true,"permalink":"/cursos/ingenieria-civil/2024-1/algebra-lineal/7-ortogonalidad/ortogonalidad-entre-vectores/","tags":["ExMAT1203"]}
---

# Concepto

El concepto de perpendicular, pero extrapolado a $\mathbb{R}^{n}$.

# Definición

Para $\mathbb{R}^{2}$, la perpendicularidad está dada por la presencia de un ángulo de $90º$ entre dos vectores. Esto implicará que si se tienen dos vectores $v$ y $u$ que son perpendiculares entre sí, se tendrá la misma distancia entre los vectores si es que se invierte uno de ellos, ya que el ángulo de $90º$ invertido seguirá siendo de $90º$.

![Pasted image 20240614152238.png](/img/user/Cursos/Ingenier%C3%ADa%20Civil/2024-1/%C3%81lgebra%20Lineal/7%20Ortogonalidad/attachments/Pasted%20image%2020240614152238.png)

Así, se dará que para dos vectores $\mathbf{u}$ y $\mathbf{v}$ perpendiculares, $\text{dist}(\mathbf{u},\mathbf{v})=\text{dist}(\mathbf{u},-\mathbf{v})$. Esto se generaliza a $\mathbb{R}^{n}$.

> [!definition] ortogonalidad por distancia
> Para dos vectores $\mathbf{u},\mathbf{v}\in\mathbb{R}^{n}$, se dice que son ortogonales si es que se cumple que:
> $$
> \text{dist}(\mathbf{u},\mathbf{v})=\text{dist}(\mathbf{u},-\mathbf{v})
> $$
{ #3bc79d}


## El producto punto entre los vectores es cero

`\begin{proof}`

Si se considera el cuadrado de la distancia entre $\mathbf{u}$ y $\mathbf{v}$, se tiene que:

$$
\begin{align}
[\text{dist}(\mathbf{u},\mathbf{v})]^{2} & =\lvert \lvert \mathbf{u}-\mathbf{v} \rvert \rvert ^{2} \\
 & =(\mathbf{u}-\mathbf{v})·(\mathbf{u}-\mathbf{v}) \\
 & =\mathbf{u}^{2}+\mathbf{v}^{2}-2\mathbf{u}\mathbf{v}
\end{align}
$$

Esto por propiedades del [[Cursos/Ingeniería Civil/2024-1/Álgebra Lineal/7 Ortogonalidad/Producto punto o interior y propiedades\|producto punto]]. También se tiene que la distancia entre $\mathbf{u}$ y $-\mathbf{v}$ es:

$$
\begin{align}
[\text{dist}(\mathbf{u},-\mathbf{v})]^{2} & =\lvert \lvert \mathbf{u}+\mathbf{b} \rvert \rvert ^{2} \\
 & =\mathbf{u}^{2}+\mathbf{v}^{2}+2\mathbf{u}\mathbf{v}
\end{align}
$$

Dado lo dicho en la [[#^3bc79d]], se debe cumplir que:

$$
\begin{align}
 & &  \text{dist}(\mathbf{u},\mathbf{v}) & =\text{dist}(\mathbf{u},-\mathbf{v}) \\
 \implies &  &  [\text{dist}(\mathbf{u},\mathbf{v})]^{2} & =[\text{dist}(\mathbf{u},-\mathbf{v})]^{2} \\
\implies &  & \mathbf{u}^{2}+\mathbf{v}^{2}-2\mathbf{u}\mathbf{v} & =\mathbf{u}^{2}+\mathbf{v}^{2}+2\mathbf{u}\mathbf{v} \\
\implies &  & 2\mathbf{u}\mathbf{v} & =0 \\
\implies &  & \mathbf{u}\mathbf{v} & =0
\end{align}
$$

`\end{proof}`

Esto nos lleva a una definición más simple de ortogonalidad, que es la que se considera como definición de ortogonalidad:

> [!definition] ortogonalidad
> Dos vectores $\mathbf{u}$ y $\mathbf{v}$ son ortogonales entre sí, si y solo sí
> $$\mathbf{u}·\mathbf{v}=0$$
{ #f532de}


Notar que $\mathbf{0}$ es ortogonal a todo $\mathbf{v}\in\mathbb{R}^{n}$, ya que $\mathbf{0}·\mathbf{v}=\mathbf{0}: \forall \mathbf{v}\in\mathbb{R}^{n}$.