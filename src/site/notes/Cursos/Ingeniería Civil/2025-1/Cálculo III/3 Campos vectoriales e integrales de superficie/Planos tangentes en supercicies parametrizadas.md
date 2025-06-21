---
{"dg-publish":true,"permalink":"/cursos/ingenieria-civil/2025-1/calculo-iii/3-campos-vectoriales-e-integrales-de-superficie/planos-tangentes-en-supercicies-parametrizadas/","tags":["I3MAT1630"]}
---

# Concepto

# Definición
Considerando dos vectores tangentes a una [[Cursos/Ingeniería Civil/2025-1/Cálculo III/3 Campos vectoriales e integrales de superficie/Superficies parametrizadas\|superficie parametrizada]] $\vec{r}$ en un punto $(s_{0},t_{0})$. Se toma la misma idea del [[Cursos/Ingeniería Civil/2024-2/Cálculo II/2 Funciones de varias variables/2.9 Definición de diferenciabilidad. Vector gradiente. Plano tangente. Aproximación lineal/Plano tangente a una superficie\|Plano tangente a una superficie]] normal, donde los vectores tangentes son:
$$
\begin{align}
\vec{r}_{s} & =\frac{ \partial \vec{r} }{ \partial s } (s_{0},t_{0}) \\
 & =\frac{ \partial x }{ \partial s } (s_{0},t_{0})\hat{\imath}+\frac{ \partial y }{ \partial s } (s_{0},t_{0})\hat{\jmath}+\frac{ \partial z }{ \partial s } (s_{0},t_{0})\hat{k}
\end{align}
$$
$$
\begin{align}
\vec{r}_{t} & =\frac{ \partial \vec{r} }{ \partial t } (s_{0},t_{0}) \\
 & =\frac{ \partial x }{ \partial t } (s_{0},t_{0})\hat{\imath}+\frac{ \partial y }{ \partial t } (s_{0},t_{0})\hat{\jmath}+\frac{ \partial z }{ \partial t } (s_{0},t_{0})\hat{k}
\end{align}
$$

El plano entonces es el [[Cursos/Ingeniería Civil/2024-1/Álgebra Lineal/1 Ecuaciones lineales en álgebra lineal/Combinaciones lineales y espacio generado\|generado]] por $\vec{r}_{s}$ y $\vec{r}_{t}$.

> [!definition] superficie parametrizada suave
> Diremos que la superficie es suave en $(s_{0},t_{0})$ si se cumple que:
> $$
> \vec{r}_{s}\times \vec{r}_{t}=0
> $$

# Ejemplo
Encuentre las ecuaciones paramétricas y normal del plano tangente al paraboloide $z=x^{2}+3y^{2}$ en un punto cualquiera $P_{0}=(x_{0},y_{0},z_{0})$.
Se parametriza como: $\langle x,y,x^{2}+3y^{2} \rangle$. Se tiene:
- $\frac{ \partial \vec{r} }{ \partial x }=\langle 1,0,2x \rangle$
- $\frac{ \partial \vec{r} }{ \partial y }=\langle 0,1,6y \rangle$
Entonces, la ecuación (vectorial) del plano tangente será:
$$
\pi(s,t)=\begin{bmatrix}
x_{0} \\
y_{0} \\
z_{0}
\end{bmatrix}+s\begin{bmatrix}
1 \\
0 \\
2x
\end{bmatrix}
+
t\begin{bmatrix}
0 \\
1 \\
6y
\end{bmatrix}:s,t,\in\mathbb{R}
$$
Para obtener la ecuación normal, se debe obtener un vector normal
$$
\begin{align}
\vec{n} & =\begin{vmatrix}
\hat{\imath} & \hat{\jmath} & \hat{k} \\
1 & 0 & 2x \\
0 & 1 & 6y
\end{vmatrix} \\
 & =\langle -2x,-6y,1 \rangle 
\end{align}
$$
Ahora, se debe cumplir en el punto $P_{0}$ para cualquier punto $P=(x,y,z)$:
$$
\begin{align}
\vec{n}·(P-P_{0}) & =0
\end{align}
$$
