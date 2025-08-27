---
{"dg-publish":true,"permalink":"/cursos/ingenieria-civil/2024-2/dinamica-fis-1514/2-dinamica-de-particulas/2-4-trabajo-y-energia-cinetica/trabajo-mecanico/","tags":["ExFIS1514"]}
---

# Concepto
Si bien se suele definir como una fuerza por un desplazamiento, ahora se definirá con diferenciales.
# Definición
Notar que $·$ es el [[Cursos/Ingeniería Civil/2024-1/Álgebra Lineal/7 Ortogonalidad/Producto punto o interior y propiedades\|producto punto]].
$$
\begin{align}
dW & =\vec{F}·d\vec{r} \\
 & =F \ dr\cos\alpha
\end{align}
$$
El trabajo de mide en $N·m$, y se interpreta como energía en $J$.

Si la componente de la fuerza en el desplazamiento tiene la misma dirección que el desplazamiento, entonces el trabajo será positivo.
## Propiedades del producto punto aplicadas al trabajo
Se pueden aplicar las propiedades del producto punto a el trabajo, por ejemplo:
### Propiedad distributiva
Dada la propiedad distributiva, se tiene:
$$
\begin{align}
dW_{\text{neta}} & =\vec{F}_{\text{neta}}·d\vec{s} \\
 & =(\vec{F}_{1}+\vec{F}_{2}+\vec{F}_{n})·d\vec{s} \\
 & =\vec{F}_{1}·d\vec{s}+\vec{F}_{2}·d\vec{s}+\dots+\vec{F}_{n}·d\vec{s}
\end{align}
$$
### Ortogonalidad y vectores paralelos
Se tiene que si $\vec{u}$ y $\vec{v}$ son ortogonales, entonces $\vec{u}·\vec{v}=\vec{0}$
De aquí, los [[Cursos/Ingeniería Civil/2024-2/Dinámica - FIS1514/1 Cinemática de partículas/1.2 Movimiento en dos y tres dimensiones/Vectores unitarios\|Vectores unitarios]] son ortogonales, entonces, por ejemplo, $\hat{i}·\hat{j}=0$.
Además, un vector unitario con sigo mismo da $1$.
Además, se t
Ahora, si se tiene los vectores:
$\vec{A}=A_{x}\hat{i}+A_{y}\hat{j}$
$\vec{B}=B_{x}\hat{i}+B_{y}\hat{j}$
Entonces:
$$
\begin{align}
\vec{A}·\vec{B} & =A_{x}\hat{i}B_{x}\hat{i}+\cancel{ A_{x}\hat{i}B_{y}\hat{j} }+\cancel{ A_{y}\hat{j}B_{x}\hat{i} }+A_{y}\hat{j}B_{y}\hat{j} \\
 & =A_{x}B_{x}+A_{y}B_{y}
\end{align}
$$
# Trabajo aplicado sobre una fuerza variable
Si la fuerza $\vec{F}$ ahora es en función de la posición, entonces el trabajo va a estar dado por la integral. (el _área_ de un gráfico $F\cos\alpha$ vs $s$).
$$
W_{1-2}=\int_{\vec{s}_{1}}^{\vec{s}_{2}} \vec{F} \, d\vec{s}= \int_{s_{1}}^{s_{2}} F\cos\alpha \, ds   
$$
![Pasted image 20241002100918.png|200](/img/user/Cursos/Ingenier%C3%ADa%20Civil/2024-2/Din%C3%A1mica%20-%20FIS1514/2%20Din%C3%A1mica%20de%20part%C3%ADculas/2.4%20Trabajo%20y%20energ%C3%ADa%20cin%C3%A9tica/attachments/Pasted%20image%2020241002100918.png)
## Fuerza constante
Se tiene que para toda posición $s$, $F\cos\alpha$ es constante:
$$
W_{1-2}=\int_{s_{1}}^{s_{2}} F\cos\alpha \, ds =F\cos\alpha \int_{s_{1}}^{s_{2}}  \, ds =F\cos\alpha \  \Delta s
$$
## Fuerza de gravedad
Considerando un $d\vec{s}=dx \hat{i}+dy \hat{j}+ dz \hat{k}$, y una fuerza de gravedad dada por $\vec{F}_{g}=-mg\hat{j}$:
$$
W_{1-2}=\int_{\vec{s}_{1}}^{\vec{s}_{2}} \vec{F}_{g} \, d\vec{s}=\int_{\vec{s}_{1}}^{\vec{s}_{2}} (-mg\hat{j})· (\hat{i}+dy \hat{j}+ dz \hat{k})
$$
Ahora se aplica producto punto considerando lo anterior ($\hat{j}·\hat{i}=0$ y $\hat{j}·\hat{k}=0$), además $\hat{j}·\hat{j}=1$
$$
\begin{align}
W_{1-2} & =\int_{y_{1}}^{y_{2}} (-mg) \, dy  \\
 & =-mgy \biggr\rvert_{y_{1}}^{y_{2} } \\
 & =-mg(y_{2}-y_{1}) \\
 & =-mg \ \Delta y
\end{align}
$$

> [!quote]
> "Si dos objetos parten desde la misma altura, y terminan en la misma altura, el trabajo es **siempre, siempre siempre siempre** cero"
> _(Alejandro Varas, 2024)_

# Ejemplo