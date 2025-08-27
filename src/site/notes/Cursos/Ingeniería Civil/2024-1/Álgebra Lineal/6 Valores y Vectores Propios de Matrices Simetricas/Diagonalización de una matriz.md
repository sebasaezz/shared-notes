---
{"dg-publish":true,"permalink":"/cursos/ingenieria-civil/2024-1/algebra-lineal/6-valores-y-vectores-propios-de-matrices-simetricas/diagonalizacion-de-una-matriz/","tags":["I3MAT1203"]}
---

# Concepto

Forma fácil de representar y calcular potencias de matrices

# Definición

> [!definition] Diagonalización de una matriz
> Para ciertas matrices $A$, existe la siguiente factorización:
> $$A=PDP^{-1}$$
> Donde $D$ es una [[#^45a07e]] hecha de $n$ valores propios de $A$, y $P$ es una matriz hecha de $n$ [[Cursos/Ingeniería Civil/2024-1/Álgebra Lineal/6 Valores y Vectores Propios de Matrices Simetricas/Vectores propios, valores propios y espacio propio#^fa3dee\|vectores propios]] en orden respectivo a los valores propios
{ #ac5696}


> [!definition] Matriz diagonal
>  Una matriz diagonal $D$ está definida por una matriz cuadrada con entradas exclusivamente en la diagonal:
>  $$
> D=\begin{bmatrix}
> * & 0 & \dots & 0 \\
> 0 & * & \dots & 0 \\
> \vdots & \vdots & \ddots & \vdots \\
> 0 & 0 & \dots & *
> \end{bmatrix}
> $$
{ #45a07e}


> [!theorem] Potencia de la diagonalización de una matriz
> Dada una matriz $A$ [[#^47792f|diagonalizable]], y su [[#^ac5696|diagonalización]] $PDP^{-1}$, se cumple que:
> $$
> A^{n}=(PDP^{-1})^{n}=PD^{n}P^{-1} 
> $$

# Diagonalizabilidad

> [!theorem] Teorema de diagonalización
> Una matriz $A_{n\times n}$ es diagonalizable, si y solo si $A$ tiene $n$ vectores propios linealmente independientes.
> Entonces $A=PDP^{-1}$, con $D$ una matriz diagonal, si y solo si las columnas de $P$ son $n$ vectores propios linalmente independientes.
{ #47792f}


> [!corollary] Teorema de diagonalización
> Una matriz $A$ es diagonalizable si y solo si los vectores propios forman una base de $\mathbb{R}^{n}$

## Para valores propios distintos entre ellos

> [!theorem] Teorema de diagonalización por valores propios
> Una matriz $A_{n\times n}$ siempre será diagonalizable si es que tiene $n$ vectores propios diferentes

## Para valores propios no distintos entre ellos
- [x] Hacer ejercicios de diagonalizabilidad, tipo valores de $h$ para que $A$ sea diagonalizable.  [completion:: 2025-04-20]

Básicamente, lo más importante es que se si repite un valor propio (multiplicidad $>1$), entonces este valor propio debe estar asignado a la misma cantidad de vectores propios linealmente independientes (dimensión de espacio propio). O que $\text{Mult}(\lambda)=\text{dim}(\text{Nul}(A-\lambda I))$.

> [!theorem] Teorema de diagonalización para valores propios con multiplicidad mayor a 1
> Dada una matriz $A$, con valores proprios $\lambda=\{ \lambda_{1},\lambda_{2},\dots,\lambda_{r} \}$ tal que exista un $\lambda$ con multiplicidad mayor a $1$, para que $A$ sea diagonalizable se debe cumplir que:
> - $\forall \lambda\text{, multiplicidad de }\lambda=\text{dim}(\text{nul}(A-\lambda I))$ 

# Ejemplo
