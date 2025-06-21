---
{"dg-publish":true,"permalink":"/cursos/ingenieria-civil/2025-1/calculo-iii/2-campos-vectoriales/campos-conservativos/campos-independientes-de-trayectoria/","tags":["I1MAT1630"]}
---

# Definición

Se dice que una integral es independiente de la trayectoria si:
$$
\int _{\mathcal{C}_{1}}F· \, d\vec{r} =\int _{\mathcal{C}_{2}}F· \, d\vec{r} 
$$
para todo $\mathcal{C}_{1}$ y $\mathcal{C}_{2}$ con los mismo puntos finales e iniciales.

> [!theorem] independencia de trayectoria de un campo conservativo
> Todo campo conservativo $F=\nabla f$ garantiza que una integral sobre $\mathcal{C}$ será independiente de la trayectoria

> [!theorem] integral de una curva cerrada en un campo independiente de trayectoria
> Toda integral sobre una curva cerrada $\mathcal{C}$ (donde el punto final es el mismo que el inicial), en un campo independiente de trayectoria cumple ($\iff$) que su integral es $0$.
> Además, se puede concluir que un campo es independiente de trayectoria si es que su integral es $0$.

Resulta que los campos vectoriales conservativos son básicamente todos los campos que son independientes de trayectoria. Se puede concluir que el campo debe ser conexo para que se cumpla

> [!theorem]
> Suponga $F$ es continua en un conjunto abierto y conexo $D$. Si la integral de línea de $F$ es independiente de trayectoria en $D$, entonces $F$ es conservativo en $D$

# Ejemplo