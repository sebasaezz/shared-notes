---
{"dg-publish":true,"permalink":"/cursos/ingenieria-civil/2024-1/algebra-lineal/6-valores-y-vectores-propios-de-matrices-simetricas/similitud-de-matrices/","tags":["I3MAT1203"]}
---

# Similitud de matrices

> [!definition] Matrices similares/semejantes/congruentes
> Dos matrices $A,B \in \mathbb{R}^{n\times n}$ son similares/semejantes/congruentes si y solo si: 
> $$\boxed{B=P^{-1}AP}  \implies A=PBP^{-1}$$
> Donde $P$ es una matriz invertible.
{ #3e15ad}


## Equivalencia de ecuaciones propias en matrices similares

> [!theorem] Equivalencia de ecuaciones propias en matrices similares/semejantes/congruentes
> Si se tienen dos matrices $A$ y $B$, tal que sean [[#^3e15ad|matrices similares]], entonces estas tienen el mismo [[Cursos/Ingeniería Civil/2024-1/Álgebra Lineal/6 Valores y Vectores Propios de Matrices Simetricas/Ecuación característica y polinomio característico#^7bf0cd\|polinomio característico]]. Es decir:
> $$
> \forall (A,B)\in\mathbb{R}^{n\times n} \exists P \in \mathbb{R}^{n\times n}:(\det P\neq 0 \land B=P^{-1}AP) \implies \det(A-\lambda I)=\det(B-\lambda I)\space\forall\lambda \in \mathbb{R}:(\exists (x \in \mathbb{R}^{n}):Ax=\lambda x \lor Bx=\lambda x)
> $$
> _Nota:_ se debe notar que la implicancia es unidireccional, si dos matrices tienen los mismo valores propios, no significa que sean similares

### Una demostración

`\begin{proof}`

Sea $B=P^{-1}AP$

Notar que:

$$
B-\lambda I=P^{-1}AP-\lambda(P^{-1}P)=P^{-1}(A-\lambda I)P
$$

Así:

$$
\det(B-\lambda I)=\det(P^{-1}(A-\lambda I)P)=\det(P^{-1})·\det(A-\lambda I)·\det(P)=\det(A-\lambda I)
$$
$$
\det(B-\lambda I)=\det(A-\lambda I)
$$

Se considera de [[Cursos/Ingeniería Civil/2024-1/Álgebra Lineal/4 Determinantes/Propiedades de determinantes\|Propiedades de determinantes]] que:

$\det(P^{-1})·\det(P)=1$

$\det(AB)=\det(A)·\det(B)$

`\end{proof}`