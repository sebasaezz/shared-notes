---
{"dg-publish":true,"permalink":"/cursos/ingenieria-civil/2025-1/ecuaciones-diferenciales/3-sistemas-de-ecuaciones-diferenciales-lineales/sistemas-de-ecuaciones-diferenciales-autonomas/","tags":["ExMAT1640"]}
---

# Concepto

# Definición
$$
\begin{cases}
x' & =F(x,y) \\
y' & =G(x,y)
\end{cases}
$$

Se va a tener que:

$$
\begin{align}
\frac{y'}{x'} & =\frac{\frac{ \mathrm{d}y }{ \mathrm{d}t } }{\frac{ \mathrm{d}x }{ \mathrm{d}t } } \\
 \frac{ \mathrm{d}y }{ \mathrm{d}x }  & =\frac{G(x,y)}{F(x,y)}
\end{align}
$$

Se tiene que los puntos donde $F=0$ y $G=0$ son indeterminados y se llaman puntos críticos.

## Solución de equilibrio

Observar que si $x_{*}$ e $y_{*}$ es solución (punto crítico) entonces nos induce una solución de la EDO. Esto es que $F(x_{*},y_{*})=G(x_{*},y_{*})=0$.

Esta solución se le llama solución de equilibrio.

### Clasificación de soluciones de equilibrio

Se clasifican por tres cosas:

| Tipo de geometría                                 | Tipo de estabilidad | Tipo de convergencia                      |
| ------------------------------------------------- | ------------------- | ----------------------------------------- |
| Centro Nodal<br>    Nodo propio<br>	Nodo impropio | Estables/inestables | Convergente<br>Asint. Conv.<br>Divergente |
| Centro Estable                                    | Centro-estable      | Neutralmente Conv.                        |
| Centro Espiral                                    | Estable/insetable   | Convergente<br>Asint. Conv.<br>Divergente |

Centro nodal: Converge a un punto.

- Nodo Impropio: Soluciones caen al punto.
- Nodo Propio: Soluciones pasan por el punto de forma tangencial.
Centro estable: Permanecen cerca pero no caen, girar al rededor el punto.
Centro espiral: Caen en espiral al punto.
![output(1).png|400](/img/user/Cursos/Ingenier%C3%ADa%20Civil/2025-1/Ecuaciones%20diferenciales/3%20Sistemas%20de%20ecuaciones%20diferenciales%20lineales/attachments/output(1).png)

## Sistemas 2x2
$$
\begin{cases}
x' =ax+by \\
y' =cx+dy
\end{cases}\iff \begin{bmatrix}
x' \\
y'
\end{bmatrix}=\begin{bmatrix}
a & b \\
c & d
\end{bmatrix}\begin{bmatrix}
x \\
y
\end{bmatrix}
$$

Se calculan los valores propios:

$$
\begin{align}
\begin{vmatrix}
a-\lambda & b \\
c & d-\lambda 
\end{vmatrix} & =(a-\lambda)(d-\lambda)-bc=0 \\
\lambda^{2}-\underbrace{ (a+b) }_{ \operatorname{tr}A }\lambda +\underbrace{ (ad-bc) }_{ \det A } & =0
\end{align}
$$

Los valores que aparecen se llama [[Cursos/Ingeniería Civil/2025-1/Ecuaciones diferenciales/3 Sistemas de ecuaciones diferenciales lineales/Traza de una matriz\|traza de la matriz]], $\operatorname{tr}A$ (suma de la diagonal) y el determinante $\det A$.

Entonces la ecuación característica es:

$$
\lambda^{2}-\operatorname{tr}(A)\lambda+\det A=0
$$

Además, se puede definir el discriminante $\Delta$ de la ecuación cuadrática:

$$
\Delta=(\operatorname{tr}A)^{2}-4\det A
$$

Se va a cumplir lo siguiente:

- $\det A=\lambda_{1}·\lambda_{2}$
- $\operatorname{tr}A=\lambda_{1}+\lambda_{2}$
- $\Delta$ determina:
	- Reales distintos ($\Delta>0$)
	- Reales repetidos ($\Delta=0$)
	- Complejos conjugados ($\Delta<0$)

![SmartSelect_20250604_111129_Samsung Notes.jpg|400](/img/user/Cursos/Ingenier%C3%ADa%20Civil/2025-1/Ecuaciones%20diferenciales/3%20Sistemas%20de%20ecuaciones%20diferenciales%20lineales/attachments/SmartSelect_20250604_111129_Samsung%20Notes.jpg)

Si la traza da 0, se tiene que $\operatorname{Re}\lambda=0$ para todo valor propio. Esto dará elipses (centro estable).

# Linealización


<div class="transclusion internal-embed is-loaded"><a class="markdown-embed-link" href="/cursos/ingenieria-civil/2025-1/ecuaciones-diferenciales/3-sistemas-de-ecuaciones-diferenciales-lineales/linealizacion-y-liberalizacion-de-un-sistema-de-ed-os-autonomo/" aria-label="Open link"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="svg-icon lucide-link"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path></svg></a><div class="markdown-embed">




# Concepto
Parecido a la [[Cursos/Ingeniería Civil/2024-1/Cálculo I/3 Aplicaciones de la Derivada/Aproximaciones lineales y diferenciales\|linealización]] pero en [[Cursos/Ingeniería Civil/2025-1/Ecuaciones diferenciales/3 Sistemas de ecuaciones diferenciales lineales/Sistemas de EDOs\|Sistemas de EDOs]].
# Linealización
Si se tiene un punto de equilibrio $(x_{0},y_{0})$, en un sistema, entonces:
$
\begin{bmatrix}
x' \\
y'
\end{bmatrix}=J_{(x_{0},y_{0})}\begin{bmatrix}
x-x_{0} \\
y-y_{0}
\end{bmatrix}
$
Con esto se aplican las mismas reglas de [[Cursos/Ingeniería Civil/2025-1/Ecuaciones diferenciales/3 Sistemas de ecuaciones diferenciales lineales/Sistemas de ecuaciones diferenciales autónomas\|Sistemas de ecuaciones diferenciales autónomas]]

# Liberalización
Tomar la linealización, y hacer el cambio de variable $\tilde{x}=x-x_{0}$ y $\tilde{y}=y-y_{0}$
Esto ya que $\tilde{x}'=x'$ y $\tilde{y}'=y'$. Entonces:
$
\begin{bmatrix}
x' \\
y'
\end{bmatrix}=J_{(x_{0},y_{0})}\begin{bmatrix}
\tilde{x} \\
\tilde{y}
\end{bmatrix}
$
# Ejemplo

</div></div>


# Ejemplo
## Ejemplo 1
$$
\begin{cases}
x' & =-x \\
y' & =-ky
\end{cases}
$$

Se tiene el punto crítico $(0,0)$. El campo de isoclinas va a estar dado por $\frac{ \mathrm{d}y }{ \mathrm{d}x }=k \frac{y}{x}$.

Las soluciones son:

$$
\begin{align}
x & =x_{0}\mathrm{e}^{ -t } & y & =y_{0}\mathrm{e}^{ -kt }
\end{align}
$$

entonces:

$$
\begin{align}
y & =\underbrace{ \frac{y_{0}}{x_{0}} }_{ \alpha }(x_{0} \mathrm{e}^{ -t })^{k} \\
 & =\alpha x^{k}
\end{align}
$$

Si $k=1$, se van a tener rectas que convergen en el origen ($y=\alpha x$). 

<iframe width='600' height='500' src='https://www.wolframcloud.com/obj/1a3fb917-1375-4dfd-9368-9d3845689973' frameborder='0'></iframe>

## Ejemplo 2
$$
\begin{cases}
x' & =x \\
y' & =y
\end{cases}
$$
El punto crítico es único, $(0,0)$, entonces la solución e equilibrio es:
$$
\begin{align}
x(t) & =0 & y(t) & =0
\end{align}
$$
Se va a tener:
$$
\frac{ \mathrm{d}y }{ \mathrm{d}x } =\frac{y}{x}
$$
## Ejemplo 3: Masa resorte
Se tiene el [[Cursos/Ingeniería Civil/2025-1/Ecuaciones diferenciales/2 EDOS de orden superior/Sistema masa-resorte\|Sistema masa-resorte]]:
$$
mx''+cx'+kx=0
$$
Se hace un sistema lineal.
$$
\begin{align}
x & =x & y & =x'
\end{align}
$$
$$
x''=y'=\frac{-cx'-kx}{m}
$$
$$
\begin{cases}
x'  =y \\
y'= \frac{-cy-kx}{m}
\end{cases}
$$
Ahora se buscan los puntos críticos considerando que:
$$
\frac{ \mathrm{d}y }{ \mathrm{d}x } =\frac{x'}{y'}=\frac{-cy-kx}{my}
$$
Se aprecia que la solución de equilibrio es $x=y=0$.
Ahora se van a clasificar las soluciones.
### Método de auto-valores
La ecuación es:
$$
mr^{2}+cr+k=0
$$
1. Valores reales distintos (negativos)
2. Valores propios reales repetidos ($-p$)
3. Valores propios complejos conjugados ($\alpha\pm i\beta,\alpha \leq 0$)
	1. Caso $\alpha=0$
En el primer caso, las soluciones son:
$$
\begin{align}
x & = \mathrm{e}^{ -r_{1}t } & y & =\mathrm{e}^{ -r_{2}t }
\end{align}
$$
con $r_{1}$ y $r_{2}$ positivos. La masa tiende a estar quieta, se va a tener un nodo propio convergente.

En el segundo caso:

$$
x=(A+tB)\mathrm{e}^{ -pt }
$$

con $p$ positivo

Esta será una solución nodal impropia convergente

En el tercer caso:

$$
x(t)=A\cos \beta t+B\sin\beta t
$$

Esta será una solución centro estable.

En el caso donde hay un $\alpha \neq 0$, se tiene:

$$
x(t)=\mathrm{e}^{ -\alpha t }(A\cos\beta t+B\sin\beta t)
$$

Este caso será un espiral convergente.

<iframe width='600' height='500' src='https://www.wolframcloud.com/obj/2aea339c-3025-4edc-b70c-e1f59e0692d8' frameborder='0'></iframe>

## Ejemplo 4
$$
\begin{cases}
x'=-2x+y \\
y'=x-2y
\end{cases}
$$

Se define:

$$
M=\begin{bmatrix}
-2 & 1 \\
1 & -2
\end{bmatrix}
$$

Los valores propios son:

$$
\begin{align}
(-2-\lambda)^{2}-1 & =0 \\
\lambda^{2}+4\lambda+3 & =0 \\
(\lambda+3)(\lambda+1) & =0
\end{align}
$$

Entonces $\lambda_{1}=-3$ y $\lambda_{2}=-1$.

- $\operatorname{tr}M=-4$
- $\det M=3$
- $\Delta=4^{2}-4·3=16-12=4$
Entonces es un nodo propio convergente.
```mathematica-plot 
raster:
  dim: 2D
  background: None
  size:
    height: Automatic
    width: "250"
general:
  axes: "True"
  axesLabel: "{x, y}"
  frame: "False"
  boxed: "True"
graphs:
  - id: graph_0
    options: {}
    type: vectorPlot
    vectorPlot:
      components:
        - -2 x + y
        - x-2 y
      domain:
        x:
          min: "-2"
          max: "2"
        y:
          min: "-2"
          max: "2"
        z:
          min: ""
          max: ""
 
 ```

## Ejemplo 5: caso no lineal
$$
\begin{cases}
x'=2x-y-2 \\
y'=3x-2y-2
\end{cases} \iff \begin{bmatrix}
x' \\
y'
\end{bmatrix}=\begin{bmatrix}
2 & -1 \\
3 & -2
\end{bmatrix}\begin{bmatrix}
x \\
y
\end{bmatrix}+\begin{bmatrix}
-2 \\
-2
\end{bmatrix}
$$

Como $\det M=-1$, es un punto silla.

Se puede apreciar que el punto está en $(2,2)$.

Con cambio de coordenadas:

$$
J=\begin{bmatrix}
F_{x} & F_{y} \\
G_{x} & G_{y}
\end{bmatrix}=\begin{bmatrix}
2 & -1 \\
3 & -2
\end{bmatrix}
$$

Es la misma matriz, ya que el vector no lineal era constante.

## Ejemplo 6
$$
\begin{cases}
x'=x-3y+2xy \\
y'=4x-6y-xy
\end{cases}
$$
$$
J=\begin{bmatrix}
1+2y & -3+2x \\
4-y & -6-x
\end{bmatrix}
$$

Ahora se encuentran los puntos críticos, uno es $(0,0)$, entonces la matriz jacoviana de ese punto es:

$$
J_{(0,0)}=\begin{bmatrix}
1 & -3 \\
4 & -6
\end{bmatrix}
$$
- $\det J_{(0,0)}=-6+12=6$ 
- $\operatorname{tr}J_{(1,1)}=-5$
- $\Delta=25-4·6=1$
Es un nodo propio convergente. 

También se nota que otro punto crítico es $\left( \frac{2}{3}, \frac{2}{5} \right)$.

Para este punto se tiene:

$$
J_{\left( \frac{2}{3}, \frac{2}{5} \right)}=\begin{bmatrix}
\frac{9}{5} & -\frac{5}{3} \\
\frac{18}{5} & -\frac{20}{3}
\end{bmatrix}
$$
- $\det J_{\left( \frac{2}{3}, \frac{2}{5} \right)}= -12+6=-12$
Entonces es un punto silla

![Pasted image 20250605120427.png|500](/img/user/Cursos/Ingenier%C3%ADa%20Civil/2025-1/Ecuaciones%20diferenciales/3%20Sistemas%20de%20ecuaciones%20diferenciales%20lineales/attachments/Pasted%20image%2020250605120427.png)