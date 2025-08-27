---
{"dg-publish":true,"permalink":"/cursos/ingenieria-civil/2025-1/calculo-iii/3-campos-vectoriales-e-integrales-de-superficie/teorema-de-stokes/","tags":["I1MAT1630"]}
---

# Concepto
Es como el [[Cursos/Ingeniería Civil/2025-1/Cálculo III/2 Campos vectoriales/Campos conservativos/Teorema de Green\|Teorema de Green]] pero para superficies que se pueden extender a $\mathbb{R}^{3}$.
# Definición
Suponga que se tiene una superficie $\mathcal{S}$ que tiene como frontera a una curva $\mathcal{C}$, es decir $\mathcal{C}$ acota a $\mathcal{S}$. Entonces dada una orientación en $\mathcal{S}$, esta induce como orientación positiva de $\mathcal{C}$ a aquella en la que $\mathcal{S}$ se encuentra en la dirección que define $\mathcal{C}$ por la mano de derecha (o a donde apunte $\vec{n}\times \vec{T}$).
![b49d37f7038146667440ad20306a8a9f63ef4f1d.png|400](/img/user/Cursos/Ingenier%C3%ADa%20Civil/2025-1/C%C3%A1lculo%20III/3%20Campos%20vectoriales%20e%20integrales%20de%20superficie/attachments/b49d37f7038146667440ad20306a8a9f63ef4f1d.png)
Entonces:

> [!theorem] teorema de Stokes
> $$
> \boxed{\oint_\limits{\mathcal{C}}\vec{F}· \mathrm{d}\vec{r}=\iint_\limits{\mathcal{\mathcal{S}}}\underbrace{  \nabla \times \vec{F} }_{ \, \pu{ rot}\vec{F} } · \mathrm{d}\vec{s} } 
> $$
{ #b5769e}


Si la superficie es cerrada, entonces $\oint_{\mathcal{C}} \vec{F}\cdot \, \mathrm{d}\vec{r}=0$:

> [!corollary]
> Si $\mathcal{S}$ es una superficie cerrada:
> $$
> \oint_\limits{\mathcal{S}}( \nabla \times \vec{F}) \, \cdot \mathrm{d}\vec{s} =0
> $$

Recordar que $\mathrm{d}\vec{s}=\vec{n}\,\mathrm{d}S= (\vec{r}_{u}\times \vec{r}_{v})  \, \mathrm{d}A$.
Análogo a que: $\mathrm{d}\vec{r}=\vec{T}\,\mathrm{d}s= r'(t) \, \mathrm{d}t$.
Es decir, la integral de trabajo de la región es equivalente a la integral de superficie sobre el.
![Pasted image 20250527093145.png|300](/img/user/Cursos/Ingenier%C3%ADa%20Civil/2025-1/C%C3%A1lculo%20III/3%20Campos%20vectoriales%20e%20integrales%20de%20superficie/attachments/Pasted%20image%2020250527093145.png)
Figura: $\mathcal{C}=\partial \Sigma$ y $\mathcal{S}=\Sigma$.
# Ejemplo
Evalúe la integral de $\vec{F}=\langle -y^{2} ,x,z^{2}\rangle$ sobre la curva de intersección del plano $y+z=2$ y el cilindro $x^{2}+y^{2}=1$ con orientación antihoraria mirado desde arriba. 
Se puede encontrar una parametrización de la curva, pero esto es más difícil. El teorema de Stokes permite integrar cualquier superficie donde $\mathcal{C}$ sea un borde.
Calculando el rotacional de $\vec{F}$:
$$
\begin{align}
\nabla \times \vec{F} & =\begin{vmatrix}
\hat{\imath} & \hat{\jmath} & \hat{k} \\
\partial_{x} & \partial_{y} & \partial_{z} \\
-y^{2} & x & z^{2} 
\end{vmatrix} \\
 & =\langle 0,0,1+2y \rangle 
\end{align}
$$
La superficie más simple es el mismo plano $y+z=2$ con dominio de la proyección del cilindro en $xy$.
Hay que parametrizar esta superficie:
$$
\Pi:\{ \vec{r}(x,y)=\langle x,y,2-y \rangle  :\mathcal{D}=\{ x^{2}+y^{2}\leq 1 \}\}
$$
$$
\begin{align}
\vec{r}_{x}\times \vec{r}_{y} & =\begin{vmatrix}
\hat{\imath} & \hat{\jmath} & \hat{k} \\
1 & 0 & 0 \\
0 & 1 & -1
\end{vmatrix} \\
 & =\langle 0,1,1 \rangle 
\end{align}
$$
$$
\begin{align}
\oint_{\mathcal{C}}\vec{F}·\mathrm{d}\vec{r} & =\iint_\limits{\mathcal{S}} \underbrace{ \langle 0,0,1+2y \rangle }_{ \operatorname{rot}\vec{F} } · \, \mathrm{d}\vec{s} \\
 & =\iint_\limits{\mathcal{D}} \langle 0,0,1+2y \rangle ·\langle 0,1,1 \rangle  \, \mathrm{d}A   \\
 & =\iint_\limits{\mathcal{D}} 1+2y \, \mathrm{d}A  \\
 & =\int_{0}^{1}  \int_{0}^{2\pi} (1+2r\sin \theta)r \, \mathrm{d}\theta \mathrm{d}r \\
  & =\pi
\end{align}
$$
![Pasted image 20250529092425.png|300](/img/user/Cursos/Ingenier%C3%ADa%20Civil/2025-1/C%C3%A1lculo%20III/3%20Campos%20vectoriales%20e%20integrales%20de%20superficie/attachments/Pasted%20image%2020250529092425.png)
