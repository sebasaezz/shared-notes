---
{"dg-publish":true,"permalink":"/cursos/ingenieria-civil/2024-2/calculo-ii/2-funciones-de-varias-variables/2-15-metodo-de-los-multiplicadores-de-lagrange/metodo-de-los-multiplicadores-de-lagrange/","tags":["I3MAT1620"]}
---

# Concepto
Técnica matemática que permite resolver problemas de [[Cursos/Ingeniería Civil/2024-2/Cálculo II/2 Funciones de varias variables/2.14 Máximos y mínimos para regiones acotadas/Mínimos y máximos para regiones acotadas en funciones de varias variables\|Mínimos y máximos para regiones acotadas en funciones de varias variables]].
Por ejemplo, si se tiene un problema en el cual se quiere buscar el volumen máximo de una caja si tapa construida con  $12m^2$ de cartón, se analizará la función $V=xyz$ con la restricción $2xz+2yx+xy=12$.

## Idea en dos variables
Imaginandose dos funciones de dos variables, $f(x,y)$ y una restricción $g(x,y)=k$, se puede tomar a esta restricción como una curva de nivel de $g$ en la altura $k$. Buscar el máximo o mínimo de $f$ restringida en $g$ es equivalente a buscar una intersección de la curva de nivel de $f$ con la de $g$ que sea tal que las dos líneas sean tangentes. En la image, se habla de buscar el valor para el que las curvas se intersequen en el punto azul.
![Pasted image 20241103191853.png](/img/user/Cursos/Ingenier%C3%ADa%20Civil/2024-2/C%C3%A1lculo%20II/2%20Funciones%20de%20varias%20variables/2.15%20M%C3%A9todo%20de%20los%20multiplicadores%20de%20Lagrange/attachments/Pasted%20image%2020241103191853.png)
Si las dos curvas son tangentes, entonces sus perpendiculares en ese punto son paralelas, y esto es precisamente el [[Cursos/Ingeniería Civil/2024-2/Cálculo II/2 Funciones de varias variables/2.11 Derivadas direccionales/Derivadas direccionales y vector gradiente\|vector gradiente]]. Así, se va a querer buscar la siguiente condición:
$$
\nabla f(x_{0},y_{0})=\lambda \nabla g(x_{0},y_{0})
$$
# Definición
Para una función $f(x,y,z)$ sujeta a la restricción $g(x,y,z)=k$. (suponiendo que los valores existen y que $\nabla g \neq 0$)
Encontrar un máximo y mínimo es equivalente a resolver el problema en el que se encuentran $x$, $y$, $z$ tales que:
$$
\nabla f(x,y,z)=\lambda \nabla g(x,y,z)
$$
El requerimiento que pide este problema es que los gradientes sean paralelos. Eso sucede si es que el corte ($k$) de la restricción es tangente al máximo o mínimo.
![Pasted image 20241025152126.png|200](/img/user/Cursos/Ingenier%C3%ADa%20Civil/2024-2/C%C3%A1lculo%20II/2%20Funciones%20de%20varias%20variables/2.15%20M%C3%A9todo%20de%20los%20multiplicadores%20de%20Lagrange/attachments/Pasted%20image%2020241025152126.png)
Lo que uno hace es construir la función de Lagrange $l$ que representa la igualdad ya vista.
# Ejemplo
## Ejemplo 1
Encuentre e mínimo y el máximo de $f(x,y)=x^{2}y$ sujeta a $x^{2}+2y^{2}=6$.
La función de lagrange será:
$$
l(x,y,\lambda)=x^{2}y+\lambda(x^{2}+2y^{2}-6)
$$
Que se cumpla la condición vista en la definición es equivalende a decir que las derivadas parciales de $l$ son $0$.
$$
l_{x}=2xy+2\lambda y=0\implies 2x(y-\lambda)=0\implies \begin{cases}
x=0 \\
y=-\lambda
\end{cases}
$$
Se tienen también los siguientes requerimientos:
$$
l_{y}=x^{2}+2\lambda y=0
$$
$$
l_{\lambda}=x^{2}+2y^{2}-6
$$
Uno se da cuenta que $x=0$ puede ser una solución, ya que implicaría que $\lambda=0 \land y=\pm \sqrt{ 3 }$

Si $y=-\lambda \implies$
$$
x^{2}=-4\lambda y\implies x^{2}=4\lambda^{2}\implies x=\pm \sqrt{ 4\lambda^{2} }\implies x=\pm2\lambda
$$
Ahora, reemplazando esta condición en una de las ecuaciones de llega a que $\lambda=\pm1$
De aquí y con estos dos valores de $\lambda$ se llegan a seis puntos:
$$
\lambda=1\begin{cases}
P_{1}(2,-1) \\
P_{2}(-2,-1)
\end{cases}
$$
$$
\lambda=-1\begin{cases}
P_{3}(2,1) \\
P_{4}(-2,1)
\end{cases}
$$
$$
\lambda=0\begin{cases}
P_{5}(0,\sqrt{ 3 }) \\
P_{6}(0,-\sqrt{ 3 })
\end{cases}
$$
Ahora solo se evalúa y se determina cuales son máximos y mínimos.
## Producción
Se tiene una funciónd de producción $P=bL^{\alpha}K^{1-\alpha}$ 