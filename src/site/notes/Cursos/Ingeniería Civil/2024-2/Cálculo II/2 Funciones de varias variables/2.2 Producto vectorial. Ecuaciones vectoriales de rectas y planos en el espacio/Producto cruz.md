---
{"dg-publish":true,"permalink":"/cursos/ingenieria-civil/2024-2/calculo-ii/2-funciones-de-varias-variables/2-2-producto-vectorial-ecuaciones-vectoriales-de-rectas-y-planos-en-el-espacio/producto-cruz/","tags":["I2MAT1620"]}
---

# Concepto
Solo funciona para vectores en [[Cursos/Ingeniería Civil/2024-2/Cálculo II/2 Funciones de varias variables/2.1 Vectores y geometría del plano y del espacio. Producto punto/Espacio cartesiano\|$\mathbb{R}^{3}$]].
Resulta en un vector ortogonal al plano [[Cursos/Ingeniería Civil/2024-1/Álgebra Lineal/1 Ecuaciones lineales en álgebra lineal/Combinaciones lineales y espacio generado\|generado]] por otros dos [[Cursos/Ingeniería Civil/2025-2/Dinámica de Sistemas Mecánicos/1 Cinemática/Vectores\|vectores]].
# Algoritmo
Para calcular el producto cruz $\vec{v}=\vec{u}\times \vec{w}$ de dos vectores $\vec{u}=(u_{1},u_{2},u_{3})$ y otro $\vec{w}=(w_{1},w_{2},w_{3})$ se deben multiplicar considerando vectores unitarios. Ahora, la técnica más común es calcular un determinante en base a estos vectores unitarios:
$$
\begin{align}
\vec{v} & =\vec{u}\times \vec{w}  \\
& =\det\begin{bmatrix}
\hat{i} & \hat{j} & \hat{k} \\
u_{1} & u_{2} & u_{3} \\
w_{1} & w_{2} & w_{3}
\end{bmatrix}  \\
 & =\hat{i}(u_{2}w_{3}-u_{3}w_{2})-\hat{j}(u_{1}w_{3}-u_{2}w_{1})+\hat{k}(u_{1}w_{2}-w_{1}u_{2}) \\
 & =\begin{bmatrix}
u_{2}w_{3}-u_{3}w_{2} \\
u_{2}w_{1}-u_{1}w_{3} \\
u_{1}w_{2}-w_{1}u_{2}
\end{bmatrix}
\end{align}
$$
# Propiedades y significado
Dirección: [[Cursos/Ingeniería Civil/2024-1/Álgebra Lineal/7 Ortogonalidad/Ortogonalidad entre vectores\|Ortogonal]] a los dos vectores (al [[Cursos/Ingeniería Civil/2024-2/Cálculo II/2 Funciones de varias variables/2.2 Producto vectorial. Ecuaciones vectoriales de rectas y planos en el espacio/Planos en R3\|plano]] generado)
Sentido: Sigue una regla de mano derecha.
- $\hat{i}\times \hat{j}=\hat{k}$
- $\mathbf{u}\times \mathbf{v}=-\mathbf{v}\times \mathbf{u}$
	- Esto se relaciona con la [[Cursos/Ingeniería Civil/2024-1/Álgebra Lineal/4 Determinantes/Propiedades de determinantes#^7c7a66\|propiedad de cambio de fila]] de determinantes.
Magnitud/módulo: $\lvert \lvert \mathbf{u} \rvert \rvert \ \lvert \lvert \mathbf{w} \rvert \rvert\sin\theta:0\leq\theta\leq\pi$
## Otras propiedades
Sean $\mathbf{u}, \mathbf{v}, \mathbf{w}$ vectores en $\mathbb{R}^{3}$, y $c\in\mathbb{R}$, se cumplirá para el producto cruz:
- NO ES ASOCIATIVO (_en general_), eso es: $(\mathbf{u}\times \mathbf{v})\times \mathbf{w}\neq \mathbf{u}\times(\mathbf{v}\times \mathbf{w})$
- Asociatividad escalar: $c(\mathbf{u}\times \mathbf{v})=(c\mathbf{u})\times \mathbf{v}=\mathbf{u}\times(c\mathbf{v})$ 
- Distributividad: $\mathbf{u}\times(\mathbf{v}+\mathbf{w})=u\times \mathbf{v}+\mathbf{u}\times \mathbf{w}$
- $\boxed{\mathbf{u}·(\mathbf{v}\times \mathbf{w})=(\mathbf{u}\times \mathbf{v})·\mathbf{w}}$
# Ejemplo