---
{"dg-publish":true,"permalink":"/cursos/ingenieria-civil/2025-1/calculo-iii/2-campos-vectoriales/integrales-de-linea/","tags":["I1MAT1630"]}
---

# Concepto
En vez de integrar sobre una región, se integra sobre una linea.
# Definición
$$
\int _{C} f\, ds=\lim_{ n \to \infty } \sum_{i=0}^{n}f(F_{i}^{*})\Delta s_{i}
$$
Finalmente:
$$\int_{C}f(x,y)\,d s=\int_{a}^{b}f{\big(}x(t),y(t){\big)}\,{\sqrt{\left({\frac{d x}{d t}}\right)^{2}\,+\,\left({\frac{d y}{d t}}\right)^{2}}}\,d t$$
Esto es independiente de la parametrización elegida. Siempre y cuando la parametrización no recorra la curva más de una vez (no hay ninguna repetición) de inicio a fin.

Da lo mismo al dirección del intervalo C, ya que representa la misma región:
$$
\int _{C}f(x,y) \, ds =\int _{-C}f(x,y) \, ds 
$$
# Con respecto a $x$ o $y$
$$
\int _{C}f(x,y) \, dx =\int_{a}^{b} f(\vec{r}(t))x'(t) \, dt 
$$
El mismo para cualquier variables. También en $\mathbb{R}^{3}$.
En estas definiciones no se puede invertir $C$.
# Ejemplo
Calcule $\int _{C} xy^{4} \, dx$ donde $C$ es el lado derecho del circulo $x^{2}+y^{2}=16$.
Primero se busca una parametrización de $C$.
$$
\vec{r}(t)=\langle 4\cos t, 4\sin t \rangle :-\frac{\pi}{2}\leq t\leq \frac{\pi}{2}
$$
Ahora los límites de $t$ serán los límites de integración, y se debe expresar al integrando en función de $t$. Se sabe que:
- $x=4\cos t$
- $y=4\sin t$
Además, se sabe que:
$$
\lvert \lvert \vec{r} \rvert \rvert =\sqrt{ 16 }=4
$$
Finalmente, la integral sera:
$$
\int_{-\frac{\pi}{2}}^{\frac{\pi}{2}} (4\cos t)(4\sin t)^{4} \lvert \lvert \vec{r} \rvert \rvert  \, dt=\int_{-\frac{\pi}{2}}^{\frac{\pi}{2}} 4^{6}\cos t\sin ^{4}t \, dt 
$$
Esto es un problema de cálculo I 🙁.


