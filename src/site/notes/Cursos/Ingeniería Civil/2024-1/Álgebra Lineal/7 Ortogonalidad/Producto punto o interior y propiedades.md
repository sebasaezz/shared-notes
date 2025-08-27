---
{"dg-publish":true,"permalink":"/cursos/ingenieria-civil/2024-1/algebra-lineal/7-ortogonalidad/producto-punto-o-interior-y-propiedades/","tags":["ExMAT1203","I2MAT1620"]}
---


> [!definition] producto punto o producto interior o producto escalar
> Para dos vectores $a,b\in\mathbb{R}^{n}$, se define el producto punto como $a^{T}b=ab^{T}$
> $$
> a=\begin{bmatrix}
> a_{1} \\
> a_{2} \\
> \vdots \\
> a_{n}
> \end{bmatrix},b=
> \begin{bmatrix}
> b_{1} \\
> b_{2} \\
> \vdots \\
> b_{n}
> \end{bmatrix} \implies a·b=a^{T}b=ba ^{T}=a_{1}b_{1}+a_{2}b_{2}+\dots+a_{n}b_{n}
> $$
> El resultado será un escalar, es decir, $(a·b)\in\mathbb{R}$
> Además se cumple que:
> $$a·b=\lvert \lvert a \rvert \rvert \lvert \lvert b \rvert \rvert \cos(\theta)$$
> Donde $\theta$ es el ángulo entre $a$ y $b$. Esto se cumplirá en $\mathbb{R}^{2}$ y $\mathbb{R}^{3}$.
> Ahora también surge lógicamente que:
> $$\vec{u}·\vec{u}=\lvert \lvert \vec{u} \rvert \rvert^{2} $$
> El producto punto de unverctor con sigo mismo es su [[Cursos/Ingeniería Civil/2024-1/Álgebra Lineal/7 Ortogonalidad/Longitud o norma de un vector, vector unitario y distancia entre vectores\|norma]] al cuadrado




{ #7997eb}


> [!corollary] propiedades del producto punto o interior
> Sean $u,v,w\in\mathbb{R}^{n}$ y $c\in\mathbb{R}$ entonces, para el [[#^7997eb]] se tiene:
> - $\mathbf{u}·\mathbf{v}=\mathbf{v}·\mathbf{u}$ 
> - $(\mathbf{u}+\mathbf{v})·\mathbf{w}=\mathbf{u}·\mathbf{w}+\mathbf{v}·\mathbf{w}$
> - $\mathbf{u}·\mathbf{v}·c=(\mathbf{u}·\mathbf{v})·c=\mathbf{u}·(\mathbf{v}· c)$
> 
> Es decir, se presentan las propiedades: conmutativa, distributiva y asociativa.
> Además, se tiene la siguiente propiedad:
> - $\mathbf{u}·\mathbf{u}\geq 0$
> - $\mathbf{u}·\mathbf{u}=0 \iff \mathbf{u}=\mathbf{0}$

# Ejemplo

Calcule el producto interior entre 

$$\mathbf{u}=\left[{\begin{array}{r}{2}\\ {-5}\\ {-1}\end{array}}\right]\mathbf{y}\ \mathbf{v}=\left[{\begin{array}{r}{3}\\ {2}\\ {-3}\end{array}}\right]$$

$$
\mathbf{u}·\mathbf{v}=2·3-5·2+1·3= -1
$$
