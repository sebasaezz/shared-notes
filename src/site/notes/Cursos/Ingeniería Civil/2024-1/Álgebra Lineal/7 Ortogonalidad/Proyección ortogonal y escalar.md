---
{"dg-publish":true,"permalink":"/cursos/ingenieria-civil/2024-1/algebra-lineal/7-ortogonalidad/proyeccion-ortogonal-y-escalar/","tags":["ExMAT1203","I2MAT1620"]}
---

# Concepto

La sombra a $90º$ de un vector $y$ en una "recta" (espacio) generada por un vector $u$ se le llama proyección ortogonal de $y$ en $u$, y se denota $\hat{y}$

# Definición

Considerar el vector $u$ que se muestra en la figura:

![Pasted image 20240616235541.png|300](/img/user/Cursos/Ingenier%C3%ADa%20Civil/2024-1/%C3%81lgebra%20Lineal/7%20Ortogonalidad/attachments/Pasted%20image%2020240616235541.png)

- Su espacio generado se muestra en la recta horizontal.
- Se aprecia también al vector $y$ del cual se quiere buscar la proyección $\hat{y}$. Como $\hat{y}\in \operatorname{Gen}\{ u \}$, $\hat{y}=\alpha u:\alpha \in\mathbb{R}$.
- Además se quiere buscar otro vector $z$, denominado "componente de $y$ ortogonal a $u$"
	- Notar que $z=y-\hat{y}$ y siempre será ortogonal a $u$.
Finalmente, y lo más importante, notar que se cumplirá que:

$$
y=\hat{y}+z \tag{1}
$$
{ #540bbd}


De la ecuación [[#^540bbd]] y lo dicho anteriormente, se nota que $z=y-\alpha u$, además se nota que $z=y-\hat{y}$ es ortogonal a $u$ $\iff$

$$
\begin{align}
 &  & \mathbf{0} & =(y-\hat{y})· u  &  & \\
\implies & &  & =(y-\alpha u)·u \\
 &  &  & =y·u-(\alpha u)·u \\
 &  &  & =y·u-\alpha(u·u) \\
 \implies &  & \alpha & =\frac{y·u}{u·u} & /\times u \\
\implies &  & \hat{y} & =\boxed{\frac{y·u}{u·u}u} 
\end{al ⚡ign}
$$

Notar que como en este concepto, lo que importa es el $\operatorname{Gen}\{ u \}$, entonces $u$ se podrá escalar por un $c\in\mathbb{R}$ y se cumplirá que $\hat{y}$ no va a cambiar.

En términos de notación, como lo que importa es la recta generada por $u$, a esta recta se le llama $L$, y dice que $\hat{y}=\operatorname{proj}_{L}y$.

> [!definition] proyección ortogonal y escalar en rectas y espacios
> Sea $\mathbf{u}\in\mathbb{R}^{n}$ e $\mathbf{y}\in\mathbb{R}^{n}$, la proyección ortogonal de $\mathbf{y}$ sobre $\mathbf{u}$, $\mathbf{\hat{y}}$, para una recta definida por $\mathbf{u}$, $L=\operatorname{Gen}\{ \mathbf{u} \}$ está dada por:
> $$
> \mathbf{\hat{y}}=\operatorname{proj}_{L}\mathbf{y}=\frac{\mathbf{y}·\mathbf{u}}{\mathbf{u}·\mathbf{u}}\mathbf{u}=\frac{\mathbf{y}·\mathbf{u}}{\lvert \lvert \mathbf{u} \rvert \rvert^{2} }\mathbf{u}
> $$
> Notar también que se puede definir la proyección escalar de la siguiente forma:
> $$
> \lvert \rvert  \operatorname{proj}_{L}\mat ⚡hbf{y} \rvert \rvert=\mathbf{y}· \frac{\mathbf{u}}{\lvert \lvert \mathbf{u} \rvert \rvert } 
> $$
> De aquí se puede definir una proyección en $\mathbb{R}^{n}$, para $\{ \mathbf{y} , \mathbf{u}_{1}, \mathbf{u}_{2}, \dots\},\in\mathbb{R}^{n}$, sobre un espacio vectorial $V$ de base ortogonal $\{\mathbf{u}_{1},\mathbf{u}_{2},\mathbf{u}_{3},\dots\}$ (no necesariamente una recta).
> $$
> \hat{\mathbf{y}} =\operatorname{proj}_{L}\mathbf{y}= \frac{\mathbf{y}·\mathbf{u}_{1}}{\lvert \lvert \mathbf{u}_{1} \rvert \rvert }+\frac{\mathbf{y}·\mathbf{u}_{2}}{\lvert \lvert \mathbf{u}_{2} \rvert \rvert }+\dots
> $$
{ #9e4752}




^75c42c 

> [!definition] componente de un vector ortogonal a otro (de una proyección)
> Para una [[#^75c42c|proyección ortogonál]] de $\mathbf{y}\in\mathbb{R}^{n}$ en $\mathbf{u}\in\mathbb{R}^{n}$, se va a tener al vector $\mathbf{z}\in\mathbb{R}^{n}$ definido como la componente de $\mathbf{y}$ ortogonal a $\mathbf{u}$, y está dada por:
> $$
> \mathbf{z}=\mathbf{y}-\mathbf{\hat{y}}
> $$ 
{ #0065a8}

 
# Ejemplo

![Pasted image 20240617002343.png|400](/img/user/Cursos/Ingenier%C3%ADa%20Civil/2024-1/%C3%81lgebra%20Lineal/7%20Ortogonalidad/attachments/Pasted%20image%2020240617002343.png)