---
{"dg-publish":true,"permalink":"/cursos/ingenieria-civil/2025-1/ecuaciones-diferenciales/3-sistemas-de-ecuaciones-diferenciales-lineales/linealizacion-y-liberalizacion-de-un-sistema-de-ed-os-autonomo/","tags":["ExMAT1640"]}
---

# Concepto
Parecido a la [[Cursos/Ingeniería Civil/2024-1/Cálculo I/3 Aplicaciones de la Derivada/Aproximaciones lineales y diferenciales\|linealización]] pero en [[Cursos/Ingeniería Civil/2025-1/Ecuaciones diferenciales/3 Sistemas de ecuaciones diferenciales lineales/Sistemas de EDOs\|Sistemas de EDOs]].
# Linealización
Si se tiene un punto de equilibrio $(x_{0},y_{0})$, en un sistema, entonces:
$$
\begin{bmatrix}
x' \\
y'
\end{bmatrix}=J_{(x_{0},y_{0})}\begin{bmatrix}
x-x_{0} \\
y-y_{0}
\end{bmatrix}
$$
Con esto se aplican las mismas reglas de [[Cursos/Ingeniería Civil/2025-1/Ecuaciones diferenciales/3 Sistemas de ecuaciones diferenciales lineales/Sistemas de ecuaciones diferenciales autónomas\|Sistemas de ecuaciones diferenciales autónomas]]

# Liberalización
Tomar la linealización, y hacer el cambio de variable $\tilde{x}=x-x_{0}$ y $\tilde{y}=y-y_{0}$
Esto ya que $\tilde{x}'=x'$ y $\tilde{y}'=y'$. Entonces:
$$
\begin{bmatrix}
x' \\
y'
\end{bmatrix}=J_{(x_{0},y_{0})}\begin{bmatrix}
\tilde{x} \\
\tilde{y}
\end{bmatrix}
$$
# Ejemplo