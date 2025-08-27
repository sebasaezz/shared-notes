---
{"dg-publish":true,"permalink":"/cursos/ingenieria-civil/2024-2/calculo-ii/2-funciones-de-varias-variables/2-2-producto-vectorial-ecuaciones-vectoriales-de-rectas-y-planos-en-el-espacio/productos-triples/","tags":["I2MAT1620"]}
---

# Producto triple escalar
Dado por la forma$(\mathbf{u}\times \mathbf{v})·\mathbf{w}$.
Sigue la siguiente propiedad:
$$
\mathbf{w}·(\mathbf{u}\times \mathbf{v})=(\mathbf{w}\times\mathbf{u})·\mathbf{v}
$$
Recordando que el [[Cursos/Ingeniería Civil/2024-1/Álgebra Lineal/7 Ortogonalidad/Producto punto o interior y propiedades\|producto punto]] es conmutativo:
$$
\mathbf{w}·(\mathbf{u}\times \mathbf{v})=\mathbf{v}·(\mathbf{w}\times \mathbf{u})=\mathbf{u}·(\mathbf{v}\times \mathbf{w})
$$
## Uso para calcular el volumen de un paralelepípedo
Digamos que se quiere calcular el siguiente volumen:
![Pasted image 20240929010946.png|300](/img/user/Cursos/Ingenier%C3%ADa%20Civil/2024-2/C%C3%A1lculo%20II/2%20Funciones%20de%20varias%20variables/2.2%20Producto%20vectorial.%20Ecuaciones%20vectoriales%20de%20rectas%20y%20planos%20en%20el%20espacio/attachments/Pasted%20image%2020240929010946.png)
Va a ser base por altura, es decir el área de abajo por la norma del vector que define a la línea roja.
## Área del paralelogramo:
Si bien se sabe que se puede usar [[Cursos/Ingeniería Civil/2024-1/Álgebra Lineal/4 Determinantes/Determinantes como área o volumen\|Determinantes como área o volumen]], otro método para calcular un área como la que se muestra:
![Pasted image 20240929011144.png|300](/img/user/Cursos/Ingenier%C3%ADa%20Civil/2024-2/C%C3%A1lculo%20II/2%20Funciones%20de%20varias%20variables/2.2%20Producto%20vectorial.%20Ecuaciones%20vectoriales%20de%20rectas%20y%20planos%20en%20el%20espacio/attachments/Pasted%20image%2020240929011144.png)
es notar que va a ser base por altura. Y si se considera a $v$ como la base, entonces la altura es $\lvert \lvert u \rvert \rvert \sin\theta$. Ahora, aplicando propiedades del [[Cursos/Ingeniería Civil/2024-2/Cálculo II/2 Funciones de varias variables/2.2 Producto vectorial. Ecuaciones vectoriales de rectas y planos en el espacio/Producto cruz\|Producto cruz]]:
$$
(base)(altura)=\lvert \lvert v \rvert \rvert \ \lvert \lvert u\rvert \rvert \cos\theta=\lvert \lvert v\times u \rvert \rvert=\lvert \lvert u\times v \rvert \rvert  
$$
## Volumen final
Notar que la altura se puede obtener como la [[Cursos/Ingeniería Civil/2024-1/Álgebra Lineal/7 Ortogonalidad/Proyección ortogonal y escalar#^9e4752\|proyección escalar]] de $w$ sobre $u\times v$. Finalmente:
$$
(area\ base)(altura)=\cancel{ \lvert \lvert u\times v \rvert \rvert } w·\frac{(u\times v)}{\cancel{ \lvert \lvert u\times w \rvert \rvert } }=w·(u\times v)
$$
# Producto triple vectorial y regla BAC-CAB

El producto triple vectorial se define y cumple que:
$$
\mathbf{A}\times(\mathbf{B}\times \mathbf{C}) =\mathbf{B}(\mathbf{A}·\mathbf{C})-\mathbf{C}(\mathbf{A}·\mathbf{B})
$$