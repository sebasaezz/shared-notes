---
{"dg-publish":true,"permalink":"/cursos/ingenieria-civil/2025-1/calculo-iii/2-campos-vectoriales/trabajo-de-un-campo-vectorial-o-integral-de-linea-de-un-campo-vectorial/","tags":["I1MAT1630"]}
---

# Concepto
# Definición
Sea $F$ un [[Cursos/Ingeniería Civil/2025-1/Cálculo III/2 Campos vectoriales/Campos vectoriales\|campo vectorial]], $\mathcal{C}$ una curva suave parametrizada para $\vec{r}(t)$. Se define el trabajo:
$$
W=\int _{\mathcal{C}}F·T \, ds 
$$
- donde $T$ es el vector tangente a la curva $C$.
Haciendo la [[Cursos/Ingeniería Civil/2025-1/Cálculo III/2 Campos vectoriales/Integrales de linea\|integral de línea]] con respecto a $t$:
$$
\begin{align}
W & =\int_{a}^{b} F(\vec{r}(t))· \underbrace{ \frac{\vec{r}'(t)}{ \lvert \lvert \vec{r}'(t)  \rvert \rvert  } }_{ \text{=$T$} } \underbrace{ \lvert \lvert \vec{r}'(t) \rvert \rvert }_{ \text{por $t$} } \, dt  \\
 & =\int_{a}^{b} F(\vec{r}(t))· \underbrace{ \vec{r}'(t)\, dt }_{ d\vec{r} } 
\end{align}
$$
Resulta similar a la definición de [[Cursos/Ingeniería Civil/2024-2/Dinámica - FIS1514/2 Dinámica de partículas/2.4 Trabajo y energía cinética/Trabajo mecánico\|Trabajo mecánico]], pero ahora considerando a la fuerza $F$ como un campo vectorial.

Si la curva se recorre al revés, va a haber un cambio de signo.
$$
\int _{-\mathcal{C}}\vec{F} \, d\vec{r} =-\int _{\mathcal{C}}\vec{F} \, d\vec{r} 
$$
Para un campo vectorial dado por $\vec{F}= \langle P,Q,R \rangle$, se tiene $\vec{r}=\langle x,y,z \rangle$:
$$
\begin{align}
\int _{\mathcal{C}}\vec{F} \, d\vec{r}  & =\int_{\mathcal{C}} P \, dx +Q\,dy+R\,dz \\
 & =\int_{\mathcal{C}} P x'\, dt +Qy'\,dt+Rx'\,dt
\end{align}
$$
# Fuerza constante

> [!theorem] trabajo con una fuerza constante
> Si una partícula tiene un trayecto cualquiera de $P$ a $Q$, entonces si $\vec{F}=cte$, a lo largo de todo el recorrido:
> $$
> W=\int _{\mathcal{C}}\vec{F} \, ds =\int_{\mathcal{C}} \vec{F} \, d\vec{r} =\vec{F}·\operatorname{dist}(PQ)
> $$

# Ejemplo