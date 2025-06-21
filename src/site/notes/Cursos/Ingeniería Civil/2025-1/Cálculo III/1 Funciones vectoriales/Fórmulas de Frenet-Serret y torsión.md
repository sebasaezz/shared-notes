---
{"dg-publish":true,"permalink":"/cursos/ingenieria-civil/2025-1/calculo-iii/1-funciones-vectoriales/formulas-de-frenet-serret-y-torsion/","tags":["I1MAT1630"]}
---

Para una curva $S$.
$$
\boxed{\frac{ dT }{ ds } =\kappa(s)N(s)} \tag{1}
$$

Donde $\kappa$ es la [[Cursos/Ingeniería Civil/2025-1/Cálculo III/1 Funciones vectoriales/Curvatura y vector tangente unitario\|curvatura]] y $n(s)$ es el [[Cursos/Ingeniería Civil/2025-1/Cálculo III/1 Funciones vectoriales/Vectores normales y binormales\|vector normal]].

$$
\frac{ dB }{ ds } =\frac{d}{ds}(T\times N) =T'\times N+T\times N 
$$
Como $B$ tiene norma $1$ para todo $S$, tenemos que $\frac{ dB }{ ds }$ es perpendicular a $B$.
Por lo tanto, $\frac{ dB }{ ds }$ es proporcional a $N$.
Definimos la función $\tau(s)$ (torsión) por la ecuación:
$$
\boxed{\frac{ dB }{ ds } =-\tau(s)N(s)} \tag{3}
$$
La torsión se interpreta como que tanto se aleja la curva de una [[Cursos/Ingeniería Civil/2025-1/Cálculo III/1 Funciones vectoriales/Curvas planas\|curva plana]].
Calculemos $\frac{ dN }{ ds }$.
$$
\begin{align}
N & =B\times T \\
\frac{ dN }{ ds }  & =B'\times T+B\times T' \\
 & =-\tau N\times T+B\times\kappa N \\
 & =\tau B-\kappa T
\end{align}
$$
$$
\boxed{\frac{ dN }{ ds } =-\kappa T+\tau B}  \tag{2}
$$
Usando estas fórmulas se deduce entonces que en el caso de una curva en 3 dimensiones, la torsión se puede calcular como:
$$
\tau(t)=\frac{(\vec{r}'(t)\times \vec{r}''(t))·\vec{r}'''(t)}{\lvert \lvert \vec{r}'(t) \times \vec{r}''(t)\rvert \rvert ^{2}}
$$
