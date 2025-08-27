---
{"dg-publish":true,"permalink":"/cursos/ingenieria-civil/2024-1/algebra-lineal/7-ortogonalidad/conjuntos-ortogonales/","tags":["ExMAT1203"]}
---

# Concepto

Un conjunto donde todos sus vectores sean ortogonales

# Definición

> [!definition] conjunto ortogonal
> Sea el conjunto $S=\{ u_{1},u_{2},\dots,u_{p} \}\in\mathbb{R}^{n}$, este será ortogonal si todo vector $u_{i},u_{j}\in S : i\neq j$ cumpla que $u_{i}·u_{j}=\mathbf{0}$.
{ #48c02e}


## Independencia lineal

Además se cumplirá lo siguiente para los conjuntos ortogonales:

> [!theorem] independencia lineal de un conjunto ortogonal
> Sea $S$ un [[#^48c02e|conjunto ortogonal]], entonces $S$ será un conjunto [[Cursos/Ingeniería Civil/2024-1/Álgebra Lineal/1 Ecuaciones lineales en álgebra lineal/Independencia y dependencia lineal#^6e8a52\|linealmente independiente]]. Esto significa que es [[Cursos/Ingeniería Civil/2024-1/Álgebra Lineal/5 Subespacios y Dimension/Base de un espacio vectorial#^6bc712\|base]] de un subespacio generado por $S$. 

A continuación, se muestra una representación en $\mathbb{R}^{3}$ de un c[](Independencia%20y%20dependencia%20lineal.md#^6e8a52) linealmente independientes.

![Pasted image 20240616234808.png](/img/user/Cursos/Ingenier%C3%ADa%20Civil/2024-1/%C3%81lgebra%20Lineal/7%20Ortogonalidad/attachments/Pasted%20image%2020240616234808.png)

## Encontrar un vector en un espacio generado por un conjunto ortogonal

Se quieren encontrar los pesos $c=\{ c_{1},c_{2},\dots,c_{p} \}$ tal que definan a un vector $y$ en un espacio, entonces se cumplirá que:

> [!theorem] pesos de un vector en un subespacio generado por un conjunto ortogonal
> Sea $S=\{ u_{1},u_{2},\dots,u_{p} \}$ un espacio ortogonal que genera al subespacio $W$ de $\mathbb{R}^{n}$, y sea el siguiente vector en $W$:
> $$y=c_{1}u_{1}+c_{2}u_{2}+\dots+c_{p}u_{p}\implies[y]_{S}=\begin{bmatrix}c_{1} \\c_{2} \\\vdots \\c_{n}\end{bmatrix}$$
> Entonces siempre se cumplirá que:
> $$c_{j}=\frac{y·u_{j}}{u_{j}·u_{j}}$$

- [x] demostrar  [completion:: 2025-04-20]

