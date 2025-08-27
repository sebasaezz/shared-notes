---
{"dg-publish":true,"permalink":"/cursos/ingenieria-civil/2024-1/algebra-lineal/7-ortogonalidad/longitud-o-norma-de-un-vector-vector-unitario-y-distancia-entre-vectores/","tags":["ExMAT1203"]}
---


> [!definition] longitud o norma de un vector
> Gráficamente, es la longitud de un vector, matemáticamente se representa para $v\in\mathbb{R}^{n}$ como $\lvert \rvert v \rvert \rvert$ y se define como:
> $$\lvert \lvert v \rvert  \rvert =\sqrt{ v_{1}^{2}+v_{2}^{2}+\dots+v_{n}^{2} }=\sqrt{ v·v }$$
> Esto además implica que:
> $$ \lvert \lvert v \rvert  \rvert ^{2}=v·v $$
> y, con $c\in\mathbb{R}$
>$$\lvert \lvert cv \rvert  \rvert=\lvert c \rvert· \lvert \lvert v \rvert  \rvert  $$
{ #2b7762}


# Vector unitario

A partir de esto, se puede definir que, para llegar al vector unitario de un vector, se debe aplicar lo siguiente:

> [!definition] vector unitario y normalización
> Un vector unitario $v$ es todo vector que tenga norma 1, es decir, $\lvert \lvert v \rvert \rvert=1$.

## Normalización

> [!theorem] Normalización
> Dado un vector $v$, se puede asignar un vector $u$ tal que tenga la misma dirección y sentido que $v$, pero tenga norma 1.
> $$
> u=\frac{1}{\lvert \lvert v \rvert  \rvert }·v
> $$
{ #fc6b11}


### Representación gráfica de la normalización
<iframe scrolling="yes" title="Vector unitario de un vector" src="https://www.geogebra.org/material/iframe/id/t2cmxkwz/width/900/height/500/border/888888/sfsb/true/smb/false/stb/false/stbh/false/ai/false/asb/false/sri/false/rc/false/ld/false/sdz/false/ctl/false" width="900px" height="500px" style="border:0px;"> </iframe>

# Distancia entre vectores

La norma de la diferencia entre dos vectores

> [!definition] distancia entre vectores
> $$
> dist(v,u)=\lvert \lvert v-u \rvert  \rvert 
> $$
{ #812913}


# Ejemplo

Sea: $\mathbf{v}=\begin{bmatrix}1 \\-2 \\2 \\0\end{bmatrix}$, encontrar vector unitario $\mathbf{u}$ en la misma dirección de $\mathbf{v}$.

Se calcula la longitud de $\mathbf{v}$:

$$
\lvert \lvert \mathbf{v} \rvert \rvert =\sqrt{ 1+4+4 }= 3
$$

Así, y según la normalización.

$$
\mathbf{u}=\frac{1}{\lvert \lvert \mathbf{v} \rvert \rvert }·\mathbf{v}=\frac{1}{3}·\begin{bmatrix}
1 \\
-2 \\
2 \\
0
\end{bmatrix}=\begin{bmatrix}
\frac{1}{3} \\
-\frac{2}{3} \\
\frac{2}{3} \\
0
\end{bmatrix}
$$
