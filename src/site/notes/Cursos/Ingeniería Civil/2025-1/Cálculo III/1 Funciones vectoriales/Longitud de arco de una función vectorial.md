---
{"dg-publish":true,"permalink":"/cursos/ingenieria-civil/2025-1/calculo-iii/1-funciones-vectoriales/longitud-de-arco-de-una-funcion-vectorial/","tags":["I1MAT1630"]}
---

# Concepto
Integrar la rapidez
# Definición
$$
\int_{a}^{b} \lvert \lvert \vec{r}'(t) \rvert \rvert   \, dt=\int_{a}^{b} \sqrt{ (f'(t))^{2}+(g'(t))^{2} } \, dt
$$
Uno también puede aproximar la longitud de arco por medio de una sumatoria de diferencias de puntos por paso del tiempo definiendo un intervalo $\Delta_{n}$
$$
\sum_{i=n}^{n} \frac{\lvert \vec{r}(t_{i-1})-\vec{r}(t_{i}) \rvert }{\Delta_{n}t} \Delta_{n}t
$$
# En función de $x$ (o $y$)
Además, si $f'$ es integrable (continua) en $(a,b)$:
$$
L=\int_{a}^{b} \sqrt{ 1+(f'(x))^{2} } \, dx 
$$
- [x] revisar  [scheduled:: 2025-03-20]  [due:: 2025-03-21]  [completion:: 2025-04-20]
# En coordenadas polares
Si $r=r(\theta)$, se puede parametrizar como:
- $x=r(\theta)\cos\theta$
- $y=r(\theta)\sin\theta$
y se cumplirá que:
$$
L=\int_{\theta_{0}}^{\theta_{1}} \sqrt{ \left( \frac{ dx }{ d\theta }  \right)^{2}+\left( \frac{ dy }{ d\theta }  \right)^{2} } \, d\theta=\int_{\theta_{0}}^{\theta_{1}} \sqrt{ \left( \frac{ dr }{ d\theta }  \right)^{2}+r(\theta)^{2} } \, d\theta 
$$
# Función longitud de arco
Finalmente, se puede definir la función longitud de arco como:

> [!theorem] función longitud de arco
> Si se tiene una función $f(x)$ o función parametrizada $\vec{r}(t)$ continua ($\vec{r}$ puede auto-intersecarse), se tiene que la función longitud de arco $s(t)$ será:
> $$
> s(t)=\int_{\alpha}^{t} \lvert \lvert \vec{r}'(u) \rvert \rvert  \, du =\int_{a}^{t} \sqrt{ 1+f'(x)^{2} } \, dx  
> $$

Observar que se $y=y(x)$, entonces, si $\vec{r}(t)=\langle f(t), g(t) \rangle$:
$$
\sqrt{ \left( \frac{ dx }{ dt }  \right)^{2}+\left( \frac{ dy }{ dt }  \right)^{2} }= \sqrt{  1+\frac{\frac{ dy }{ dt } }{\frac{ dx }{ dt } }}\frac{ dx }{ dt }= \sqrt{  1+\frac{ dy }{ dx } }\frac{ dx }{ dt }
$$
Entonces, si se aplica $\int  \, dt$ a los dos lados, se tiene que:
$$
s=\int_{\alpha}^{\beta} \sqrt{ \left( \frac{ dx }{ dt }  \right)^{2}+\left( \frac{ dy }{ dt }  \right)^{2} } \, dt=\int_{a}^{b} \sqrt{ 1+\frac{ dy }{ dt }  } \, dx  
$$
De viendo desde diferenciales:
$$
\sqrt{ \left( \frac{ dx }{ dt }  \right)^{2}+\left( \frac{ dy }{ dt }  \right)^{2} }dt=\sqrt{ 1+\left( \frac{ dy }{ dx }  \right) }dx=ds
$$
Lo que se puede escribir de la forma:
$$
ds^{2}=\left( \left( \frac{ dx }{ dt }  \right)^{2}+\left( \frac{ dy }{ dt }  \right)^{2} \right)dt^{2}
$$
Y finalmente:
$$
\boxed{ds^{2}=dx^{2}+dy^{2}} 
$$
# Ejemplo
Determine la longitud de $y^{2}=x$ desde $(-1,1)$ hasta $(1,1)$.
Notar que está $x$ en función $y$, entonces se puede derivar con respecto a $y$.
- $f'(y)=2y$
$y$ va desde $-1$ hasta $1$.
$$
\begin{align}
L & =\int_{-1}^{1} \sqrt{ 1+(2y)^{2} } \, dy 
\end{align}
$$
Integral trigonométrica, se reemplaza:
- $2y=\tan\theta$
- $\implies 4y^{2}+1=\tan ^{2}\theta+1=\sec ^{2}\theta$
$$
L=2\int_{0}^{\arctan (2)} \sec ^{3}\theta \, d\theta 
$$
- [x] revisar integral trigonométrica  [scheduled:: 2025-03-22]  [due:: 2025-04-02]  [completion:: 2025-04-20]