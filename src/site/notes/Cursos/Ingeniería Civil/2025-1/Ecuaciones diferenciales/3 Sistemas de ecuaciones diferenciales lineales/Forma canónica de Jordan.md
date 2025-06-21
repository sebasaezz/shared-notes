---
{"dg-publish":true,"permalink":"/cursos/ingenieria-civil/2025-1/ecuaciones-diferenciales/3-sistemas-de-ecuaciones-diferenciales-lineales/forma-canonica-de-jordan/","tags":["ExMAT1640"]}
---

# Concepto
[[Cursos/Ingeniería Civil/2024-1/Álgebra Lineal/6 Valores y Vectores Propios de Matrices Simetricas/Diagonalización de una matriz\|Diagonalizar]] una matriz no diagonal
# Definición

> [!definition] Forma de Jordan de una matriz
> Sea $A\in\mathbb{C}^{n\times n}$ una matriz cuadrada, entonces existe una matriz invertible $P^{-1}AP=J$ donde $P$ es una matriz de vectores propios generalizados y $J$ es una matriz en forma canónica de Jordan. Esto es una matriz **bloque-diagonal** compuesta por los bloques de Jordan $J_{k}(\lambda)$ de la siguiente forma:
> $$
> J=\begin{bmatrix}
> J_{k_{1}}(\lambda_{1}) & 0 & \cdots & 0 \\
> 0 & J_{k_{2}}(\lambda_{2}) & \cdots & 0 \\
> \vdots & \vdots & \ddots & \vdots \\
> 0 & 0 & \cdots & J_{k_{m}}(\lambda_{m})
> \end{bmatrix}
> $$
> Donde:
> $$
> J_{k}(\lambda)=\begin{bmatrix}
> \lambda & 1 & 0 & \cdots & 0 \\
> 0 & \lambda & 1 & \cdots & 0 \\
> \vdots & \ddots & \ddots & \ddots & \vdots \\
> 0 & \cdots & 0 & \lambda & 1 \\
> 0 & \cdots & \cdots & 0 & \lambda
> \end{bmatrix}
> $$
> $\lambda$ es un autovalor. Esta matriz es una generalización de la matriz diagonal para valores propios repetidos. Si ningún $\lambda$ se repite, se va a tener $D$.

# Ejemplo