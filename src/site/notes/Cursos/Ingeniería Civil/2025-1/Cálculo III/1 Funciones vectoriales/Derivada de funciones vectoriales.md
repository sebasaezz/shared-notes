---
{"dg-publish":true,"permalink":"/cursos/ingenieria-civil/2025-1/calculo-iii/1-funciones-vectoriales/derivada-de-funciones-vectoriales/","tags":["I1MAT1630"]}
---

# Concepto
La de siempre, pero con [[Cursos/Ingeniería Civil/2025-1/Cálculo III/1 Funciones vectoriales/Curvas Paramétricas y funciones vectoriales\|funciones vectoriales]].
# Definición
> [!definition] derivada de funciones vectoriales
> $$
> \dot{\vec{r}}=\frac{ d\vec{r} }{ dt } =\lim_{ h \to 0 } \frac{\vec{r}(t+h)-\vec{r}(t)}{h}
> $$
> 

Como el límite de las funciones vectoriales cumple que es un vectorcon el límite en cada componente, entonces:
> [!theorem] derivada en funciones vectoriales (por componentes)
> Si $\vec{r}(t)=\langle f_{1}(t),f_{2}(t),\dots,f_{n}(t) \rangle$, y todas las funciones $f_{k}$ son derivables con respecto a $t$, entonces $\frac{ d\vec{r} }{ dt } =\langle f_{1}'(t),f_{2}'(t),\dots,f_{n}'(t) \rangle$
> 

Este vector es tangente a la [[Cursos/Ingeniería Civil/2025-1/Cálculo III/1 Funciones vectoriales/Curvas Paramétricas y funciones vectoriales\|curvas paramétricas]] y se puede parametrizar en el punto.

> [!definition] vector tangente unitario
> Si $\dot{\vec{r}}(t)\neq 0$, entonces el vector tangente unitario es:
> $$
> \hat{\dot{\vec{r}}}(t_{0})=T(t_{0})=\frac{\dot{\vec{r}(t_{0})}}{\lvert \lvert \dot{\vec{r}(t_{0})} \rvert \rvert }
> $$

Sea $\vec{u}$, $\vec{v}\in\mathbb{R}^{3}$ derivables,  $c\in\mathbb{R}$, $f$ una función real, entonces:
- $\frac{ d }{ dt }(\vec{u}+ \vec{v})=\frac{ du }{ dt }+\frac{ dv }{ dt }$
- $\frac{ d }{ dt }(c\vec{v})=c \vec{v}'$
- $\frac{ d }{ dt }(f(t)\vec{u})=f'·\vec{u}+f·\vec{u}'$
- $\frac{ d }{ dt }(\vec{u}·\vec{v})=\vec{u}'·\vec{v}+\vec{u}·\vec{v}'$
- $\frac{ d }{ dt }(\vec{u}\times\vec{v})=\vec{u}'\times\vec{v}+\vec{u}\times\vec{v}'$
- $\frac{d}{dt}\vec{u}(f(t))=\vec{u}'(f(t))·f'(t)$
# Ejemplo
Encuentre el VTU y recta tangente a la curva en $t=\frac{\pi}{4}$:
$$
\vec{r}(t)=\langle 2\cos t , 2\sin t \rangle 
$$
$$
\implies\dot{\vec{r}}(t)=\langle -2\sin t, 2\cos t \rangle\implies\dot{\vec{r}}\left( \frac{\pi}{4} \right) =\langle -\sqrt{ 2 }, \sqrt{ 2 } \rangle 
$$
Su norma es $2$. Entonces:
$$
T\left( \frac{\pi}{4} \right)=\left\langle - \frac{\sqrt{ 2 }}{2 }  , \frac{\sqrt{ 2 }}{2}\right\rangle 
$$

Ecuación de la recta:
$$
\text{recta}=\langle \sqrt{ 2 }, \sqrt{ 2 } \rangle +\left\langle - \frac{\sqrt{ 2 }}{2 }  , \frac{\sqrt{ 2 }}{2}\right\rangle 
$$
