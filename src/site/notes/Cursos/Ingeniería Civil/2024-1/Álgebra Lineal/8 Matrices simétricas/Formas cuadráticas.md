---
{"dg-publish":true,"permalink":"/cursos/ingenieria-civil/2024-1/algebra-lineal/8-matrices-simetricas/formas-cuadraticas/","tags":["ExMAT1203"]}
---

# Concepto

Una función ($Q$) que se construye a través de matrices simétricas.

Extiende el concepto de una ecuación cuadrática en $\mathbb{R}$.

# Definición

Una función $Q$ en $\mathbb{R}^{n}$ a valores reales.

Se define de la siguiente forma:

$$
Q(x)=x^{T}Ax
$$

Donde $A$ es una [[Cursos/Ingeniería Civil/2024-1/Álgebra Lineal/8 Matrices simétricas/Matrices simétricas\|Matrices simétricas]].

## Propiedades

Los elementos el producto de los elementos de la diagonal inversa será el coeficiente que pertenece al producto de cada componente del vector.

Los elementos pertenecientes a la diagonal son los coeficientes de los cuadrados.

## Clasificación de formas cuadráticas

Se clasifican de las siguientes formas:

![Pasted image 20240624092017.png|200](/img/user/Cursos/Ingenier%C3%ADa%20Civil/2024-1/%C3%81lgebra%20Lineal/8%20Matrices%20sim%C3%A9tricas/attachments/Pasted%20image%2020240624092017.png)

Además, esta clasificación se lleva a la matriz que define la forma cuadrática.

> [!definition] Matriz positiva definida
> Una matriz $A_{n\times n}$ es positiva definida si es que la forma cuadrática $x^{T}Ax$ siempre será positiva. Esto se cumplirá siempre que todos los valores del espectro de $A$ (Valores propios) son todos positivos.
{ #da1c7f}


> [!definition] Clasificación de formas cuadráticas
> - Positiva definida $\iff \lambda>0$
> - Semi-positiva definida $\iff \lambda\geq 0$
> - Negativa definida $\iff \lambda<0$
> - Semi-negativa definida $\iff \lambda\leq 0$

## Teorema para formas cuadráticas con $\lvert \lvert \mathbf{x} \rvert \rvert=1$

> [!theorem] valor máximo y mínimo de una forma cuadrática para vectores unitarios
> Si se restringe la forma cuadrática $\mathbf{x}^{T}A\mathbf{x}$ a solo los vectores $\{ \mathbf{x}:\lvert \lvert \mathbf{x} \rvert \rvert=1 \}$, entonces se cumplirá que el valor mímino $m=\operatorname{mín}\{ \mathbf{x}^{T}\mathbf{x}:\lvert \lvert \mathbf{x} \rvert \rvert=1 \}$ será el menor valor propio de $A$, y el máximo $M=\operatorname{max}\{ \mathbf{x}^{T}\mathbf{x}:\lvert \lvert \mathbf{x} \rvert \rvert=1 \}$ será el valor propio mayor de $A$. El valor de $\mathbf{x}$ será el [[Cursos/Ingeniería Civil/2024-1/Álgebra Lineal/6 Valores y Vectores Propios de Matrices Simetricas/Vectores propios, valores propios y espacio propio#^1a33f2\|vector propio]] asociado
{ #28e8d9}


# Ejemplo
## Ejemplo 1: Sacar el cuadrado de la norma de un vector

Sea $A=I\in \mathbb{R}^{n}$, así:

$$
Q(x)=x^{T}Ix=x^{T}x=\lvert \lvert x \rvert \rvert ^{2}
$$
## Ejemplo 2

Sea:

$$
A=\begin{bmatrix}
4 & 0 \\
0 & 3
\end{bmatrix},Q(x)=x^{T}Ax \implies 4x_{1}^{2}+3x_{2}^{2}
$$
```mathematica-plot 
raster:
  dim: 3D
  background: None
  size:
    height: Automatic
    width: "250"
general:
  axes: "True"
  axesLabel: "{x, y}"
  frame: "False"
  boxed: "True"
graphs:
  - id: graph_0
    options: {}
    type: plot
    plot:
      expression: 3x^2+7y^2
      plotRange:
        x:
          min: "-4"
          max: "4"
        y:
          min: "-4"
          max: "4"
 
 ```

## Ejemplo 3

Sea:

$$
A=\begin{bmatrix}
3 & -2 \\
-2 
 & 7
\end{bmatrix},Q(x)=x^{T}Ax \implies Q(x)=3x_{1}^{2}+7x_{2}^{2}-4x_{1}x_{2}
$$
## Ejemplo 4: De forma cuadrática a matriz

Sea $x \in\mathbb{R}^{3}$ y $Q(x)=5x_{1}^{2}+3x_{2}^{2}+2x_{3}^{2}-x_{1}x_{2}+8x_{2}x_{3}$

Se considera la diagonal dado lo dicho de los coeficientes:

$$
A=\begin{bmatrix}
5 &  &  \\
 & 3 &  \\
 &  & 2
\end{bmatrix}
$$

Como las sumas de las componentes que dan $x_{2}x_{3}$ debe ser $8$, y esto se cumplirá en la diagonal inversa $a_{23}$ y  $a_{32}$:

$$
A=\begin{bmatrix}
5 &  &  \\
 & 3 & 4 \\
 & 4 & 2
\end{bmatrix}
$$

lo mismo con el $-1$:

$$
A=\begin{bmatrix}
5 &  -\frac{1}{2}&0  \\
 -\frac{1}{2}& 3 & 4 \\
0 & 4 & 2
\end{bmatrix}
$$

## Ejemplo 5: en $\mathbb{R}^{3\times 3}$
$$
x^{T}\begin{bmatrix}
1 & 0 & 2 \\
0 & 4 & -7 \\
2 & -7 & 0
\end{bmatrix}x=x_{1}^{2}+4x_{2}^{2}+(2+2)x_{1}x_{3}+(-7-7)x_{2}x_{3}
$$
