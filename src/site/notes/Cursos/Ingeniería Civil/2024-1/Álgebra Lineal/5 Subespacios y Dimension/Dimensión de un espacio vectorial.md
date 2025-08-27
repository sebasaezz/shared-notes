---
{"dg-publish":true,"permalink":"/cursos/ingenieria-civil/2024-1/algebra-lineal/5-subespacios-y-dimension/dimension-de-un-espacio-vectorial/","tags":["I3MAT1203"]}
---

# Concepto

Si se define un espacio vectorial. Se concluye que si se tiene un conjunto en ese espacio que tenga más vectores que la cantidad de su base, tiene que ser linealmente independiente.

> [!theorem] Dependencia lineal de un conjunto en un espacio vectorial
> Dado $V$ un espacio vectorial de base $B=\{ b_{1},b_{2},\dots,b_{n} \}$, entonces cualquier conjunto en $V$ que contenga más de $n$ vectores debe ser linealmente dependiente

## Dimensión finita

> [!definition] Dimensión finita e infinita
> Si $V$ es generado por un conjunto finito de vectores, entonces $V$ tiene dimensión $Dim(V)$ finita. Caso opuesto es infinita.

> [!theorem] Dimensión de un subespacio
> Sea $H$ un subespacio de $V$, tal que $V$ tenga dimensión finita. Se complirá que $$\text{dim }H \leq \text{dim }V$$
> Es decir: la dimensión de un subespacio no puede ser mayor que la del espacio en el que se encuentra

El espacio de los polinomios $\mathbb{P}_{n}$ tiene dimensión infinita

## Dimensión de $Nul(A)$ y $Col(A)$

La dimensión de $Nul(A)$ es la cantidad de variables libres de $A$.

La dimensión de $Col(A)$ y $Fila(A)$ es el número de columnas pivote de $A$.