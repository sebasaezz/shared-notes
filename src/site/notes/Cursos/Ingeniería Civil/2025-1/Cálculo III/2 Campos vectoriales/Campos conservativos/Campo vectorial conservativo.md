---
{"dg-publish":true,"permalink":"/cursos/ingenieria-civil/2025-1/calculo-iii/2-campos-vectoriales/campos-conservativos/campo-vectorial-conservativo/","tags":["I1MAT1630"]}
---



> [!definition] campo vectorial conservativo
> Un campo vectorial $F$ definido sobre $D$, tal que $\int _{C} F \, d\vec{r}$ es independiente de la trayectoria y $D$ es (discreto) **simplemente conexo** (no tiene hoyos). Entonces $F$ es conservativo, es decir, existe $f$ tal que:
> $$
> \nabla f=F
> $$
> Es decir, existe una función tal que el campo es el gradiente de ella.



> [!theorem]
> Si $F=\langle P,Q \rangle$ es un campo vectorial conservativo tal que $P$ y $Q$ tienen derivadas parciales continuas sobre $D$:
> $$
> \frac{ \partial P }{ \partial y } =\frac{ \partial Q }{ \partial x } 
> $$
> en $D$. Esto es un sí y solo si, si es que se está en un dominio simplemente conexo.
> Esto ya que $P$ y $Q$ son derivadas parciales, entonces las derivadas parciales mostradas son alternadas y deben ser iguales por el [[Cursos/Ingeniería Civil/2024-2/Cálculo II/2 Funciones de varias variables/2.8 Derivadas parciales de orden superior. Relación de Clairaut/Derivadas parciales de orden superior#^8db770\|teorema de Clairaut]] 

# Como demostrar que un campo es conservativo
Se puede integrar $\nabla f=F$ para obtener $f$. Esto ya que:
- $\partial_{x}f=P(x,y)$
- $\partial_{y}f=Q(x,y)$
Si la integral existe, entonces $F$ es conservativo.

# Ejemplo