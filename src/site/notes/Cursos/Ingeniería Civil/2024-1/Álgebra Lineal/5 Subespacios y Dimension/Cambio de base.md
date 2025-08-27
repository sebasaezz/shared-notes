---
{"dg-publish":true,"permalink":"/cursos/ingenieria-civil/2024-1/algebra-lineal/5-subespacios-y-dimension/cambio-de-base/","tags":["I3MAT1203"]}
---

# Concepto

Un espacio $V$ puede tener varias bases, si se tiene $B$ y $C$, el cambio de base trata de explicar este cambio.

"Básicamente cambiar imágenes de perros a gatos" 

(Sánchez, 2024)

# Matriz de cambio de coordenadas

> [!definition] Matriz de cambio de coordenadas (cambio de base)
> Se cumplirá para un espacio $V$ con base $\mathcal{B}=\{ b_{1},b_{2},\dots,b_{n} \}$ y base $\mathcal{C}=\{  c_{1},c_{2},\dots,c_{n} \}$ que:
> $$
> \underset{\mathcal{C}\leftarrow\mathcal{B}}{P}=\big[ \begin{array}[]] [b_{1}]_{\mathcal{C}} & [b_{2}]_{\mathcal{C}} & \cdots & [b_{n}]_{\mathcal{C}}\end{array} \big]
> $$
> Esta siendo la matriz que cumple que $[x]_{\mathcal{C}}=\underset{\mathcal{C}\leftarrow\mathcal{B}}{P}[x]_{\mathcal{B}}$
{ #713117}


## Demostración

`\begin{proof}`

Dadas las bases $\mathcal{B}=\{ b_{1},b_{2},\dots,b_{n} \}$ y $\mathcal{C}=\{c_{1},c_{2},\dots,c_{n}\}$ de un espacio vectorial $V$, y un vector $x=\alpha_{1}b_{1}+\alpha_{2}b_{2}+\dots+a_{n}b_{n}$.

Se quiere encontrar una matriz $\underset{\mathcal{C}\leftarrow\mathcal{B}}{P}$ tal que $[x]_{\mathcal{C}}=\underset{\mathcal{C}\leftarrow\mathcal{B}}{P}[x]_{\mathcal{B}}$.

Se tiene que:

$$
[x]_{\mathcal{B}}=\begin{bmatrix}
\alpha_{1} \\
\alpha_{2} \\
\vdots \\
\alpha_{n}
\end{bmatrix}
$$

Partiendo por la ecuación:

$$
x=\alpha_{1}b_{1}+\alpha_{2}b_{2}+\dots+a_{n}b_{n}
$$

Se puede aplicar el vector coordenado, esto se puede ya que según [[Cursos/Ingeniería Civil/2025-2/Dinámica de Sistemas Mecánicos/1 Cinemática/Vectores coordenados o coordenadas de un vector y sistemas de coordenadas#^89b87e\|este teorema]], estos son una transformación lineal.

$$
\implies[x]_{\mathcal{C}}=[\alpha_{1}b_{1}+\alpha_{2}b_{2}+\dots+a_{n}b_{n}]_{\mathcal{C}}
$$

Ahora, como es una transformación lineal, se pueden aplicar sus propiedades:

$$
\implies[x]_{\mathcal{C}}=\alpha_{1}[b_{1}]_{\mathcal{C}}+\alpha_{2}[b_{2}]_{\mathcal{C}}+\dots+[b_{n}]_{\mathcal{C}}
$$
$$
\implies [x]_{\mathcal{C}}=\big[ \begin{array}[]] [b_{1}]_{\mathcal{C}} & [b_{2}]_{\mathcal{C}} & \cdots & [b_{n}]_{\mathcal{C}}\end{array} \big]
\begin{bmatrix}
\alpha_{1} \\
\alpha_{2} \\
\vdots \\
\alpha_{n}
\end{bmatrix}
$$

Pero ya se dijo que $[x]_{\mathcal{B}}=\begin{bmatrix}\alpha_{1} \\\alpha_{2} \\\vdots \\\alpha_{n}\end{bmatrix}$ entonces:

$$
\implies[x]_{\mathcal{C}}=\big[ \begin{array}[]] [b_{1}]_{\mathcal{C}} & [b_{2}]_{\mathcal{C}} & \cdots & [b_{n}]_{\mathcal{C}}\end{array} \big][x]_{\mathcal{B}}
$$

Finalmente se llegó a la ecuación que se quería al inicio, lo que implica que:

$$
\underset{\mathcal{C}\leftarrow\mathcal{B}}{P}=\big[ \begin{array}[]] [b_{1}]_{\mathcal{C}} & [b_{2}]_{\mathcal{C}} & \cdots & [b_{n}]_{\mathcal{C}}\end{array} \big]
$$

`\end{proof}`

## Inversa de cambio de base

> [!corollary] La inversa de matriz cambio de coordenadas o cambio de base
> Dada la [[#^713117]], se tiene que:
> $$(\underset{\mathcal{C}\leftarrow\mathcal{B}}{P})^{-1}=\underset{\mathcal{B}\leftarrow\mathcal{C}}{P}$$

## Técnica para encontrar matriz de cambio de coordenadas

> [!corollary] Técnica para encontrar matriz de cambio de coordenadas
> Dadas las bases $\mathcal{B}=\{ b_{1},b_{2},\cdots,b_{n} \}$ y $\mathcal{C}=\{ c_{1},c_{2},\cdots,c_{n} \}$ de un espacio vectorial $V$
> $$
> [\begin{array}{cccc|cc}
> b_{1} & b_{2} & \cdots & b_{n} & c_{1} &c_{2} & \cdots & c_{n} 
> \end{array}]
> \sim
> [
> \space I \space \space|\space \underset{\mathcal{C}\leftarrow\mathcal{B}}{P}\space
> ]
> $$

# Ejemplo

Dada la base $B=\{ b_{1},b_{2} \}$ y $x=3b_{1}+b_{2}$

y la base $C=\{ c_{1},c_{2} \}$

tal que $b_{1}=4c_{1}+c_{2}$ y $b_{2}=-6c_{1}+c_{2}$

Entonces $[x]_{B}=\begin{bmatrix} 3\\1\end{bmatrix}$

Encuentre $[x]_{C}$

$$
x=3\underbrace{(4c_{1}+c_{2})}_{b_{1}}+\underbrace{(-6c_{1}+c_{2})}_{b_{2}}

=6c_{1}+4c_{2} \implies [x]_{C}=
\begin{bmatrix}
6 \\
4
\end{bmatrix}
$$
**Resolución 2:**
$$
x=3b_{1}+b_{2}
$$

Se aplica $[x]_{C}$ a cada lado de la ecuación:

$$
[x]_{C}=[3b_{1}+b_{2}]_{C}
$$

Pero la función coordenadas en una transformación lineal, entonces se pueden aplicar las propiedades:

$$
[x]_{C}=3[b_{1}]_{C}+[b_{2}]_{C}
$$

Dada la definición de el vector coordenadas, $[b_{1}]_{C}$ son los pesos de $\{ c_{1},c_{2} \}$ para que sea $b_{1}$. Por las igualdades dadas anteriormente, estos serían:

$$
[b_{1}]_{C}=\begin{bmatrix}
4 \\
1
\end{bmatrix}
;
[b_{2}]_{C}=\begin{bmatrix}
-6 \\
1
\end{bmatrix}
$$

Entonces:

$$
[x]_{C}=3\begin{bmatrix}
4 \\
1
\end{bmatrix}+\begin{bmatrix}
-6 \\
1
\end{bmatrix}
=
\begin{bmatrix}
6 \\
4
\end{bmatrix}
$$
