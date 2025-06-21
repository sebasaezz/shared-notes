---
{"dg-publish":true,"permalink":"/cursos/ingenieria-civil/2025-1/ecuaciones-diferenciales/1-edos-de-primer-orden/5-estudio-de-modelos-de-linealidad-y-estadistica/diagramas-de-fase-interpretacion-y-estabilidad-de-modelos-no-lineales/","tags":["I2MAT1640"]}
---

Las [[Cursos/Ingeniería Civil/2025-1/Ecuaciones diferenciales/1 Edos de primer orden/1 Ecuaciones diferenciales de primer orden/Introducción a las Ecuaciones diferenciales ordinaias\|EDOs]] se deben interpretar para el estudio de modelos. 
Para evaluar la estabilidad de una EDO, se puede ver si el límite de la derivada (dada por la ecuación) así como también su signo.
Si el límite tiende a $0$, la ecuación es estable en un punto (una recta).

> [!theorem] estabilidad de EDOs autónomas
> Todas las EDOs autónomas, es decir, donde su derivada no depende de la variable independiente, de la forma:
> $$
> \frac{ dy }{ dx } =f(y)
> $$
> y tendrán soluciones de equilibrio (estable o inestable)

# Ejemplo
## Ejemplo 1: Ley de enfriamiento de Newton
La [[Ley de enfriamiento de Newton\|Ley de enfriamiento de Newton]] está dada por la siguiente ecuación:
$$
\frac{ dT }{ dt } =-k(T-A):k>0
$$
La solución de la EDO es:
$$
T(t)=A+(T_{0}-A)e^{-kt}
$$
Para interpretar el significado de la EDO, se puede considerar el límite de la solución general.
$$
\lim_{ t \to \infty } T(t)=A
$$
Como toda solución tiende a $A$ (temperatura ambiente) la EDO es estable.
No se necesita tener la solución para concluir que la EDO converge a estabilidad. Ya que:
$$
\lim_{ t \to \infty } \frac{ dT }{ dt } =\lim_{ t \to \infty } -k(T-A)=0
$$
![Pasted image 20250401111843.png|400](/img/user/Cursos/Ingenier%C3%ADa%20Civil/2025-1/Ecuaciones%20diferenciales/1%20Edos%20de%20primer%20orden/5%20Estudio%20de%20modelos%20de%20linealidad%20y%20estad%C3%ADstica/attachments/Pasted%20image%2020250401111843.png)
