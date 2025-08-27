---
{"dg-publish":true,"permalink":"/cursos/ingenieria-civil/2024-1/algebra-lineal/5-subespacios-y-dimension/numeros-vectores-y-matrices-complejos/","tags":["ExMAT1203"]}
---

## Números complejos

> [!definition] número complejo
> un número complejo $z$ se define como 
> $$z\in\mathbb{C}\iff z=a+bi:a,b\in \mathbb{R} \land i=\sqrt{ -1 }$$ 
{ #889a66}


## Vector complejo

> [!definition] vector complejo
> Un vector $\vec{z} \in\mathbb{C}^{n}$ es complejo si sus entradas $\{ z_{1},z_{2},\dots,z_{n} \}\in\mathbb{C}$. Este vector se puede mostrar en la forma $z=a+bi$, al igual que un [[Números complejos\|número complejo]].
> Sea:
> $$
> \vec{z}=\begin{bmatrix}
> a_{1}+b_{1}i \\
> a_{2}+b_{2}i \\
> \vdots \\
> a_{n}+b_{n}i
> \end{bmatrix}
> =
> \begin{bmatrix}
> a_{1} \\
> a_{2} \\
> \vdots  \\
> a_{n}
> \end{bmatrix}
> +
> \begin{bmatrix}
> b_{1} \\
> b_{2} \\
> \vdots \\
> b_{n}
> \end{bmatrix}i=\vec{a}+\vec{b}i
> :\vec{a},\vec{b}\in\mathbb{R}^{n}$$
{ #aa2db5}


## Matriz compleja

> [!definition] matriz compleja
> Una matriz $A\in \mathbb{C}^{m\times n}$ es compleja si es que está compuesta de [[#^aa2db5|vectores complejos]] $\mathbf{z}=\{ \mathbf{z}_{1},\mathbf{z}_{2},\cdots,\mathbf{z}_{n} \}$.

## Complejo conjugado

> [!definition] conjugado
> Sea $z\in\mathbb{C}=a+bi:c,b\in\mathbb{R}$, entonces se tiene que el complejo conjugado 
> $$\bar{z}=z^{*}= a-bi=\mathrm{Re}(z)-\mathrm{Im}(z)i$$
> Sea $\mathbf{z}\in\mathbb{C}^{n}=\mathbf{a}+\mathbf{b}i:\mathbf{a},\mathbf{b}\in\mathbb{R}^{n}$, entonces se tiene que el complejo conjugado 
> $$\bar{\mathbf{z}}=\mathbf{z}^{*}= \mathbf{a}-\mathbf{b}i=\mathrm{Re}(\mathbf{z})-\mathrm{Im}(\mathbf{z})i$$
> Sea $Z\in\mathbb{C}^{m\times n}=A+Bi:A,B\in\mathbb{R}^{m\times n}$, entonces se tiene el complejo conjugado
> $$\bar{Z}=Z^{*}=A-Bi=\mathrm{Re}(Z)-\mathrm{Im}(Z)i$$
{ #5aa82b}


> [!corollary] propiedad de multiplicación de conjugados
> Sea $\overline{r}$ conjugado de $r\in\mathbb{C}$, $\overline{x}$ el de $x \in\mathbb{C}^{n}$ y para las matrices $\overline{A}$ el de $A\in\mathbb{C}^{m\times n}$ y $\overline{B}$ el de $B\in\mathbb{C}^{n\times p}$. Se tendrá que:
> $$
> \overline{rx}=\bar{r}\bar{x},\overline{Bx}=\bar{B}\bar{x},\overline{BC}=\bar{B}\bar{C}, \overline{rB}=\bar{r}\bar{B}
> $$
> En resumen, para todos los casos se cumplirá que el conjugado de una multiplicación será la multiplicación de los conjugados
{ #3b73a8}

