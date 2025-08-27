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
El rotacional también se puede definir como la integral de línea sobre una curva cerrada la superficie encerrada por ella cuando esta superficie tiende a cero. Este valor entrega únicamente la componente normal del rotacional a la superficie elegida.
$$
(\nabla \times \vec{F})\hat{n}=\lim_{ S \to 0 } \frac{\oint_{C} \vec{F}· \, \mathrm{d}\vec{r} }{S}
$$
Si se multiplica la ecuación por $S$ considerando una cantidad infinitesimal integrada, entonces se obtiene el teorema de stokes:


<div class="transclusion internal-embed is-loaded"><a class="markdown-embed-link" href="/cursos/ingenieria-civil/2025-1/calculo-iii/3-campos-vectoriales-e-integrales-de-superficie/teorema-de-stokes/#b5769e" aria-label="Open link"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="svg-icon lucide-link"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path></svg></a><div class="markdown-embed">



> [!theorem] teorema de Stokes
> $
> \boxed{\oint_\limits{\mathcal{C}}\vec{F}· \mathrm{d}\vec{r}=\iint_\limits{\mathcal{\mathcal{S}}}\underbrace{  \nabla \times \vec{F} }_{ \, \pu{ rot}\vec{F} } · \mathrm{d}\vec{s} } 
> $

</div></div>


# Ejemplo