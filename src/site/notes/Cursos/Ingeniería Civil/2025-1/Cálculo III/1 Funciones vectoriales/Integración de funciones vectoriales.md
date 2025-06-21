---
{"dg-publish":true,"permalink":"/cursos/ingenieria-civil/2025-1/calculo-iii/1-funciones-vectoriales/integracion-de-funciones-vectoriales/","tags":["I1MAT1630"]}
---

# Concepto
Integrar las componentes.
# Definición
Para una función vectorial $\vec{r}=\langle f(t), g(t), h(t) \rangle$ con componentes integrables en $[a,b]$. Se define igual que en una [[Cursos/Ingeniería Civil/2024-1/Cálculo I/4 La Integral/Suma de Riemann\|Suma de Riemann]].
$$
\begin{align}
\int_{a}^{b} \vec{r} \, dt  & =\lim_{ n \to \infty } \sum_{i=1}^{n}\vec{r}(t_{i}^{*})\Delta t \\
 & =\lim_{ n \to \infty } \sum_{i=1}^{n}\langle f(t_{i}^{*}), g(t_{i}^{*}), h(t_{i}^{*}) \rangle\Delta t \\
 & =\langle\lim_{ n \to \infty } \sum_{i=1}^{n}f(t_{i}^{*})\Delta t,\lim_{ n \to \infty } \sum_{i=1}^{n}g(t_{i}^{*})\Delta t ,\lim_{ n \to \infty } \sum_{i=1}^{n}h(t_{i}^{*})\Delta t \rangle  \\
 & =\boxed{\left\langle \int_{a}^{b} f(t) \, dt, \int_{a}^{b} g(t) \, dt , \int_{a}^{b} h(t) \, dt\right\rangle } 
\end{align}
$$
Se aplican todas las reglas de integrales
## Calcular integral a partir de parámetros
Si el gráfico de $y(x)$ es parametrizable por:
- $x=f(t)$
- $y=g(t)$
Entonces:
$$
\frac{ dx }{ dt } =f'(t)\implies dx=f'(t)dt
$$
$$
\int_{a}^{b} y(x) \, dx =\int_{\alpha}^{\beta} g(t)f'(t) \, dt 
$$
donde:
- $x(\alpha)=a$
- $y(\beta)=b$
# Ejemplo