---
{"dg-publish":true,"permalink":"/cursos/ingenieria-civil/2025-1/calculo-iii/3-campos-vectoriales-e-integrales-de-superficie/integral-de-superficie-de-campos-vectoriales/","tags":["I1MAT1630"]}
---

# Concepto
# Definición
Dado en campo vectorial $\vec{F}$ queremos definir la integral de $\vec{F}$ sobre una superficie $\mathcal{S}$. La cantidad físicamente relevante a integrar es el componente de $\vec{F}$ normal a la superficie. Para que la integral esté bien definida, requerimos que a definición del vector normal unitaroi a la superficie se comporte bien.
Una superficie se dice **orientable** si es posible asignar cada punto $P$ de $\mathcal{S}$ en vector normal unitario $\vec{n}$ de manera tal que el mapeo $F\rightarrow\vec{n}$ sea continua.

Un ejemplo de una superficie no orientable, es la [[Cinta de Möbius\|Cinta de Möbius]], donde se puede trazar un camino para llegar al mismo punto, pero alternando el vector normal para el otro lado. Se tienen dos vectores normales en un mismo punto.

![Pasted image 20250522091048.png|400](/img/user/Cursos/Ingenier%C3%ADa%20Civil/2025-1/C%C3%A1lculo%20III/3%20Campos%20vectoriales%20e%20integrales%20de%20superficie/attachments/Pasted%20image%2020250522091048.png)

# En qué dirección va el vector normal
Si una superficie es orientable, entonces, existen solo dos mapeos que cumplen con la condición de asignar de manera continua un vector unitario. Cada uno de los cuales se llama una orientación.

En otras palabras, uno puede asignar un vector hacia arriba o hacia abajo y no hay más.

![Pasted image 20250522091704.png|600](/img/user/Cursos/Ingenier%C3%ADa%20Civil/2025-1/C%C3%A1lculo%20III/3%20Campos%20vectoriales%20e%20integrales%20de%20superficie/attachments/Pasted%20image%2020250522091704.png)

Para una superficie en $\mathbb{R}^{3}$ $\vec{r}(s,t)$ la parametrización induce un vector orientación:
$$
\vec{n}=\frac{\vec{r}_{s}\times \vec{r}_{t}}{\lvert \lvert \vec{r}_{s}\times \vec{r}_{t} \rvert \rvert }
$$
Si se tiene la parametrización $z=g(x,y)$, entonces:
$$
\vec{n}=\frac{\langle g_{x}, g_{y}, 1  \rangle }{\sqrt{ 1+g_{x}^{2}+g_{y}^{2} }}
$$
La cual apunta hacia $z$ positiva.

La orientación positiva será la que el vector normal apunte hacia afuera de una región encerrada.

Ahora, la integral de flujo en $\mathbb{R}^{3}$ sobre una región $\mathcal{S}$ se define de la siguiente forma, con el mismo significado del [[Cursos/Ingeniería Civil/2025-1/Cálculo III/2 Campos vectoriales/Formas vectoriales del teorema de Green y flujo\|flujo en R2]]:
$$
\iint_\limits{\mathcal{S}} \vec{F}· \, \mathrm{d}\vec{s}=\iint_\limits{\mathcal{S}} \vec{F}·\vec{n} \, \mathrm{d}S  
$$
_Nota:_ esta integral también se denota $\oint_\limits{\mathcal{S}} \vec{F} \, \mathrm{d}\vec{s}$ si es cerrada.
Se tiene que $\mathrm{d}S=\lvert \lvert \vec{r}_{s}\times \vec{r}_{t} \rvert \rvert \,\mathrm{d}A$.
Entonces:
$$
\begin{align}
\iint_\limits{\mathcal{S}} \vec{F}·\vec{n} \, \mathrm{d}S  & =\iint_\limits{\mathcal{S}} \vec{F}· \frac{\vec{r}_{s}\times \vec{r}_{t}}{\lvert \lvert \vec{r}_{s}\times \vec{r}_{t} \rvert \rvert } \, \mathrm{d}S \\
 & =\iint_\limits{\mathcal{D}} \vec{F}·(\vec{r}_{s}\times \vec{r}_{t}) \, \mathrm{d}A  
\end{align}
$$
# Simplificación para $z=g(x,y)$
Si $\mathcal{S}$ es el gráfico de $z=g(x,y)$, entonces:
$$
\begin{align}
x & =x  & 
y & =y  & 
x & =g(x,y) 
\end{align}
$$
Entonces
$$
\vec{r}_{x}\times \vec{r}_{y}=\langle -\partial_{x}g,-\partial_{y} g,1\rangle 
$$
De modo que si $\vec{F}=\langle P,Q,R \rangle$ entonces:
$$
\iint_\limits{\mathcal{S}} \vec{F}· \, \mathrm{d}\vec{s}=\iint_\limits{\mathcal{D}} (-P\partial_{x}g-Q\partial_{y}g+R) \, \mathrm{d}A  
$$
# Ejemplo

Calcule el flujo de $\vec{F}=\langle y,x,z \rangle$ sobre superficie del paraboloide $z=1-x^{2}-y^{2}$ sobre el plano $z=0$:
Se va a tener $\mathcal{D}=\{ x^{2}+y^{2}\leq 1 \land 0\leq z\leq 1 \}$.
$$
\iint_\limits{\mathcal{S}} \vec{F}· \, \mathrm{d}\vec{s}=\iint_\limits{\mathcal{D}} (-y(-2x)-x(-2y)+(1-x^{2}-y^{2})) \, \mathrm{d}A  
$$
Ahora se pueden usar coordenadas polares para resolver y da $\frac{\pi}{2}$.



