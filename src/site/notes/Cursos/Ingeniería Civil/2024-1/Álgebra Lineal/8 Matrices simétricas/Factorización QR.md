---
{"dg-publish":true,"permalink":"/cursos/ingenieria-civil/2024-1/algebra-lineal/8-matrices-simetricas/factorizacion-qr/","tags":["ExMAT1203"]}
---

# Concepto

Dividir en una matriz común y corriente en una ortogonal y otra triangular superior con todas las entradas de se diagonal positivas.

Básicamente aplicar el [[Cursos/Ingeniería Civil/2024-1/Álgebra Lineal/7 Ortogonalidad/Proceso de Gram-Schmit\|Proceso de Gram-Schmit]] a la columnas de una matriz para obtener $Q$ (y normalizar) y después despejar $R$

# Definición

> [!theorem] factorización QR
> Sea $A_{m\times n}$, se podrá factorizar como $A=QR$, donde $Q$ es una matriz de $m\times n$ cuyas columnas forman una base orto**normal** para $\operatorname{Col}A$ y $R$ es una matriz [[Cursos/Ingeniería Civil/2024-1/Álgebra Lineal/1 Ecuaciones lineales en álgebra lineal/Resolviendo sistemas de ecuaciones lineales con matrices aumentadas y matrices convenientes#^84222b\|triangular superior]].

$$
Q^{T}Q=I
$$
$$
QR=A\implies \underbrace{ Q^{T}Q }_{ I }R=Q^{T}A\implies R=Q^{T}A
$$
# Ejemplo