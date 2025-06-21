---
{"dg-publish":true,"permalink":"/cursos/ingenieria-civil/2025-1/calculo-iii/3-campos-vectoriales-e-integrales-de-superficie/integral-de-superficie-de-campos-escalares/","tags":["I1MAT1630"]}
---


Sobre una superficie $\mathcal{S}$ parametrizada por $\vec{r}(s,t)$, se define una función $f$. Es decir, $f: \mathbb{R}^{3}\rightarrow \mathbb{R}$.
Esto se denomina:
$$
\iint_{\mathcal{S}}f\,\text{d}S=\lim_{ i,j \to \infty } \sum_{i,j}^{}f(P_{ij})\Delta S_{ij}
$$
Donde $P_{ij}$ es un punto en la subdivisión $d_{ij}$ con área $\Delta S_{ij}$. De forma que $S$ tiene un dominio $\mathcal{D}$ sobre el que se está integrando.

Entonces la integral será:
$$
\iint_{\mathcal{S}}f\,\text{d}S=\iint_{\mathcal{D}}f(\vec{r}(s,t))·\lvert \lvert \vec{r}_{s}\times \vec{r}_{t} \rvert \rvert \,\text{d}A
$$
De otra forma, $\mathrm{d}S=\lvert \lvert \vec{r}_{s}\times \vec{r}_{t} \rvert \rvert\,\mathrm{d}s\,\mathrm{d}t$.
Si $\mathcal{S}=\mathcal{S}_{1} \cup \mathcal{S}_{2} \cup\dots \cup \mathcal{S}_{n}$, entonces definimos:
$$
\iint_{\mathcal{\mathcal{S}}} f \, \mathrm{d}S =\iint_{\mathcal{\mathcal{S_{1}}}} f \, \mathrm{d}S+\iint_{\mathcal{\mathcal{S}}_{2}} f \, \mathrm{d}S+\dots+\iint_{\mathcal{\mathcal{S}}_{n}} f \, \mathrm{d}S
$$
# Simplificaciones del producto cruz
Si es que $\vec{r}$ es un $z=f(x,y)$.
$$
\lvert \lvert \vec{r}_{x}\times \vec{r}_{y} \rvert \rvert =\sqrt{ 1+(f_{x})^{2}+(f_{y})^{2} }
$$
# Ejemplo