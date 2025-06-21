---
{"dg-publish":true,"permalink":"/cursos/ingenieria-civil/2025-1/calculo-iii/2-campos-vectoriales/campos-conservativos/tfc-en-integrales-de-linea/","tags":["I1MAT1630"]}
---

# Concepto
# Definición

Suponga que $\mathcal{C}$ es una curva parametrizada por $\vec{r}, a\leq t\leq b$, y que $f$ es un campo escalar [[Cursos/Ingeniería Civil/2025-1/Cálculo III/2 Campos vectoriales/Campos conservativos/Campo vectorial conservativo\|conservativo]] (que es continuamente derivable o $\mathcal{C}^{1}$). 

Se tiene que la composición $f(\vec{r}(t))$ que va  de $[a,b]\rightarrow\mathbb{R}$ es derivable con:
$$
\begin{align}
\frac{d}{dt} f(\vec{r}(t)) & =\frac{ \partial f }{ \partial x_{1} } \frac{ dx_{1} }{ dt } +\frac{ \partial f }{ \partial x_{2} } \frac{ dx_{2} }{ dt } +\dots+\frac{ \partial f }{ \partial x_{n} } \frac{ dx_{n} }{ dt }  \\
 & =\nabla f·\vec{r}'
\end{align}
$$
Al gradiente usualmente se le llama potencial de campo. Luego:
$$
\int _{\mathcal{C}}\nabla f \, d\vec{r}=\int _{a}^{b}\nabla f·\vec{r}' \, dt  =\int_{a}^{b} \frac{d}{dt} [f(\vec{r}(t))] \, dt
$$
Recordando el [[Cursos/Ingeniería Civil/2024-1/Cálculo I/4 La Integral/Teorema fundamental del cálculo (TFC) y propiedades\|TFC]]:
$$
\int_{a}^{b} \frac{d}{dt} [f(\vec{r}(t))] \, dt=f(\vec{r}(b))-f(\vec{r}(c))
$$
Si se tiene un $\mathcal{C}$ continua por trozos, se puede demostrar por medio de un resultado que es una suma telescópica, que el teorema se va a mantener completamente y no se necesita evaluar cada trozo.
# Ejemplo

Calcular el trabajo realizado

por 
$$
F= -\frac{mMG}{\lvert \lvert \vec{x} \rvert \rvert ^{3}}\vec{x}
$$
para una partícula que se mueve de $\langle 1,1,1 \rangle$ a $\langle -1,-1,-1 \rangle$ a lo largo de una curva suave que no pasa por el origen.

Se puede saber que si $f=\frac{mMG}{\lvert \lvert \vec{x} \rvert \rvert}$, entonces $\nabla f=F$. Luego:
$$
\begin{align}
W & =\int _{\mathcal{C}}F· \, d\vec{r}  =\int _{\mathcal{C}}\nabla f ·\, d\vec{r}   \\
 & = f(-1,-1,-1)-f(1,1,1) \\
 & =\frac{mMR}{\sqrt{ 3 }}-\frac{mMR}{\sqrt{ 3 }}=0
\end{align}
$$