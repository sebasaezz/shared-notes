---
{"dg-publish":true,"permalink":"/cursos/ingenieria-civil/2025-1/calculo-iii/2-campos-vectoriales/rotacional/","tags":["I3MAT1630"]}
---

# Definición
Si $F=\langle P,Q,R \rangle$ es un campo vectorial, entonces el rotacional de $F$ es:
$$
\operatorname{rot}\vec{F}=\left\langle  \frac{ \partial R }{ \partial y } -\frac{ \partial Q }{ \partial z } , \frac{ \partial P }{ \partial z } -\frac{ \partial R }{ \partial x } ,\frac{ \partial Q }{ \partial x } -\frac{ \partial P }{ \partial y }   \right\rangle 
$$

De forma nemotécnica, se toma al siguiente operador diferencial vectorial $\nabla$ [[Cursos/Ingeniería Civil/2024-2/Cálculo II/2 Funciones de varias variables/2.11 Derivadas direccionales/Derivadas direccionales y vector gradiente\|gradiente]]:
$$
\nabla=\left\langle  \frac{ \partial  }{ \partial x }  ,\frac{ \partial  }{ \partial y }  ,\frac{ \partial  }{ \partial z } \right\rangle 
$$
Si esto se opera sobre una función escalar, se obtiene su gradiente, y se puede obtener el rotacional sacando su producto cruz con el campo vectorial.
$$
\operatorname{rot}\vec{F}=\nabla \times \vec{F}=\begin{vmatrix}
\hat{\imath} & \hat{\jmath} & \hat{k} \\
\partial_{x} & \partial_{y} & \partial_{z} \\
P & Q & R
\end{vmatrix}
$$

> [!theorem]
> Si una función $f$ tiene derivadas parciales continuas de segundo orden, entonces:
> $$
> \operatorname{rot}\nabla f=0
> $$
> Esto sucede por el Teorema de Clairaut

Así, se puede verificar que un campo $\vec{F}$ es conservativo en un dominio simplemente conexo sabiendo que:
$$
\operatorname{rot}\vec{F}=0
$$
# Ejemplo