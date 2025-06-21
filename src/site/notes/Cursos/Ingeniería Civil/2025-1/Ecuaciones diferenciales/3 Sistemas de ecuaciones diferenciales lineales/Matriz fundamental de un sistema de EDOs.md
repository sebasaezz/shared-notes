---
{"dg-publish":true,"permalink":"/cursos/ingenieria-civil/2025-1/ecuaciones-diferenciales/3-sistemas-de-ecuaciones-diferenciales-lineales/matriz-fundamental-de-un-sistema-de-ed-os/","tags":["ExMAT1640"]}
---

# Concepto
Matriz formada por las soluciones de una edo
# Definición
Si $\vec{y}_{1}, \vec{y}_{2}, \dots,\vec{y}_{n}$ son soluciones de un [[Cursos/Ingeniería Civil/2025-1/Ecuaciones diferenciales/3 Sistemas de ecuaciones diferenciales lineales/Sistemas de EDOs\|Sistemas de EDOs]], entonces:
$$
\Phi=\begin{bmatrix}
\vec{y}_{1} & \vec{y}_{2} & \cdots &\vec{y}_{n} 
\end{bmatrix}
$$
Esta matriz es una función, y hay infinitas matrices fundamentales.
# Matriz fundamental principal
Para un [[Cursos/Ingeniería Civil/2025-1/Ecuaciones diferenciales/3 Sistemas de ecuaciones diferenciales lineales/Sistemas de EDOs lineales homogéneos con coeficientes constantes\|sistema homogéneo]], se tiene la matriz fundamental principal:
$$
\Psi=\mathrm{e}^{ Mt }
$$
Resulta que:
$$
\Psi=\Phi(t)\Phi^{-1}(0)
$$
# Ejemplo