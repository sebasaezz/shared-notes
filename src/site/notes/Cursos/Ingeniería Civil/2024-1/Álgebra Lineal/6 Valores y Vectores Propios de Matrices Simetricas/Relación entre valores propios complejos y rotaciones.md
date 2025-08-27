---
{"dg-publish":true,"permalink":"/cursos/ingenieria-civil/2024-1/algebra-lineal/6-valores-y-vectores-propios-de-matrices-simetricas/relacion-entre-valores-propios-complejos-y-rotaciones/","tags":["ExMAT1203"]}
---

# Comportamiento iterativo de una matriz de rotación

Sucede que las matrices de rotación, tales como la matriz $A= \begin{bmatrix}0 & -1 \\1 & 0\end{bmatrix}$, que rota un vector 90º en sentido antihorario, tienen un comportamiento iterativo, si se multiplica el mismo vector 4 veces se vuelve al mismo punto, por ejemplo, para vector $x=\begin{bmatrix}2 \\3\end{bmatrix}$:

$$
\begin{array}{cccl}
 & Ax & = & 
\begin{bmatrix}
0 & -1 \\
1 & 0
\end{bmatrix}\begin{bmatrix}
2 \\
3
\end{bmatrix} & = & \begin{bmatrix}
-3 \\
2
\end{bmatrix} \\
\implies & 
A^{2}
x & = & 
\begin{bmatrix}
0 & -1 \\
1 & 0 
\end{bmatrix}\begin{bmatrix}
-3 \\
2
\end{bmatrix} & = & \begin{bmatrix}
-2 \\
-3
\end{bmatrix} \\
\implies & A^{3}x & =  
& \begin{bmatrix}
0 & -1 \\
1 & 0
\end{bmatrix}\begin{bmatrix}
-2 \\
-3
\end{bmatrix} & = & \begin{bmatrix}
3 \\
-2
\end{bmatrix} \\
\implies  & A^{4}x & = & \begin{bmatrix}
0 & -1 \\
1 & 0
\end{bmatrix}\begin{bmatrix}
3 \\
-2
\end{bmatrix} & = & \begin{bmatrix}
2 \\
3
\end{bmatrix}  =  x
\end{array}


$$

Evidentemente, ningún vector distinto de cero se puede mapear sobre sí mismo entonces los vectores propios no pueden estar en $\mathbb{R}^{3}$. Es decir, $\not\exists x \in \mathbb{R}^{3}:Ax=\lambda x$.

Lo visto anteriormente, también nos lleva a que $A=A^{4k}:k\in\mathbb{Z}$. Si se aplica [[Cursos/Ingeniería Civil/2024-1/Álgebra Lineal/6 Valores y Vectores Propios de Matrices Simetricas/Diagonalización de una matriz\|Diagonalización de una matriz]], se tiene que:

$$
A=\begin{bmatrix}
x_{1} & x_{2}
\end{bmatrix}\begin{bmatrix}
\lambda_{1} & \lambda_{2}
\end{bmatrix}\begin{bmatrix}
x_{1} & x_{2}
\end{bmatrix}^{-1}
=
\begin{bmatrix}
x_{1} & x_{2}
\end{bmatrix}\begin{bmatrix}
\lambda_{1}^{4k} & \lambda_{2}^{4k}
\end{bmatrix}\begin{bmatrix}
x_{1} & x_{2}
\end{bmatrix}^{-1}:k\in\mathbb{Z}
$$

Entonces $\lambda=\lambda^{4k}: k\in\mathbb{Z}$, pero distinta a cualquier otra potencia (no es 0 ni 1). Esto no se puede cumplir con ningún $\lambda \in\mathbb{R}:\lambda\ne \{0,1\}$. Pero resulta que si se puede cumplir con un $\lambda \in\mathbb{C}$, ya que $i=i^{4k}:k \in\mathbb{Z}$.

Toda matriz iterativa está relacionada con una rotación, y esta dinámica se explica mejor con los complejos y sus propeidades

# Relación con los conjugados

Dadas las [[Cursos/Ingeniería Civil/2024-1/Álgebra Lineal/5 Subespacios y Dimension/Números, vectores y matrices complejos#^3b73a8\|propiedades de multiplicación de conjugados]], se tiene que al definir una matriz $A\in\mathbb{R}^{n\times n}$, es decir, la matriz tiene todas sus entradas reales, con $x$ vector propio asociado a su valor propio $\lambda$:

$$
A\bar{x}=\overline{Ax}=\overline{\lambda x}=\bar{\lambda}\bar{x}
$$

Así, se concluye que $\bar{\lambda}$ es valor propio de $A$ tal como lo es $\lambda$. Esto demuestra que para una matriz $A$ **con entradas reales**, sus valores propios complejos siempre se encontrarán en forma de pares conjugados, y los vectores propios también.

# Rotación generalizada en $\mathbb{R}^{2}$

Resulta que esta matriz nace del análisis complejo de la siguiente matriz:

$$
C=\begin{bmatrix}
a & -b \\
b & a
\end{bmatrix}:a,b\neq 0
$$

Si se calculan los valores propios:

$$
|C-\lambda I|=0\implies (a-\lambda)^{2}-b^{2}\implies\lambda^{2}-2\lambda a+a^{2}-b^{2}=0
$$
$$
\lambda=\frac{2a\pm \sqrt{ 4a^{2}-4(a^{2}-b^{2}) }}{2}=a\pm \frac{\sqrt{ -4b^{2} }}{2}=\boxed{a\pm bi} 
$$

Ahora de la matriz se puede extraer una variable $r$ tal que $r=|\lambda|=\sqrt{ a^{2}+b^{2} }$ (notar que el signo de $b$ da lo mismo). Este es el módulo del número complejo, y su representación polar estaría dada por $\lambda=(r,\pm\varphi)$.

Además, se tiene que 

- $\cos \varphi= \frac{a}{r}$
- $\sin\varphi=\frac{b}{r}$
Dada la siguiente interpretación gráfica:
![Pasted image 20240613213543.png|300](/img/user/Cursos/Ingenier%C3%ADa%20Civil/2024-1/%C3%81lgebra%20Lineal/6%20Valores%20y%20Vectores%20Propios%20de%20Matrices%20Simetricas/attachments/Pasted%20image%2020240613213543.png)
Finalmente, al factorizar este factor $r$:
$$
\begin{bmatrix}
a & -b \\
b & a
\end{bmatrix}=r\begin{bmatrix}
\frac{a}{r} & -\frac{b}{r} \\
\frac{b}{r} & \frac{a}{r}
\end{bmatrix}=r\begin{bmatrix}
\cos\varphi  & -\sin\varphi  \\
\sin\varphi & \cos\varphi
\end{bmatrix}
$$

Pero ya se demostró que la matriz de rotación en $\mathbb{R}^{2}$ es la siguiente:


<div class="transclusion internal-embed is-loaded"><a class="markdown-embed-link" href="/cursos/ingenieria-civil/2024-1/algebra-lineal/1-ecuaciones-lineales-en-algebra-lineal/matriz-de-rotacion-por-un-angulo/#0a2514" aria-label="Open link"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="svg-icon lucide-link"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path></svg></a><div class="markdown-embed">



$
A=\begin{bmatrix}
\cos(\varphi) & -\sin(\varphi) \\
\sin(\varphi) & \cos(\varphi)
\end{bmatrix}
$

</div></div>


## Conclusión

Para matrices en $\mathbb{R}^{2}$ de la forma $\begin{bmatrix}a & -b \\b & a\end{bmatrix}$, se establece una rotación por el ángulo $\varphi=\sec\left( \frac{a}{|\lambda|} \right)=\csc\left( \frac{b}{|\lambda |} \right)$ y escalamiento por $r=\sqrt{ a^{2}+b^{2} }=|\lambda|$.

![Pasted image 20240613221632.png](/img/user/Cursos/Ingenier%C3%ADa%20Civil/2024-1/%C3%81lgebra%20Lineal/6%20Valores%20y%20Vectores%20Propios%20de%20Matrices%20Simetricas/attachments/Pasted%20image%2020240613221632.png)

# Forma $A=PCP^{-1}$

Hay matrices que hacen rotaciones pero en formas diferentes a una circunferencia, tales como una [[Elipse\|Elipse]]. Estas se puede representar en una forma $PCP^{-1}$, donde $P$ es una matriz que define a la rotación de forma circular, mientras que $P$ le da la otra forma. Esto se puede interpretar como un cierto **cambio de variable**.

![Pasted image 20240614001759.png](/img/user/Cursos/Ingenier%C3%ADa%20Civil/2024-1/%C3%81lgebra%20Lineal/6%20Valores%20y%20Vectores%20Propios%20de%20Matrices%20Simetricas/attachments/Pasted%20image%2020240614001759.png)

Ahora, siempre se cumplirá lo siguiente:

> [!theorem] representación de una matriz iterativa con cambio de base y matriz de rotación
> Sea $A \in \mathbb{R}^{2\times 2}$ una matriz real de $2\times 2$, con un valor propio complejo $\lambda=a\pm bi:b\neq 0$ y un vector propio asociado $\mathbf{v}\in\mathbb{C}^{2}$, entonces se podrá factorizar la matriz de la siguiente forma:
> $$
> A=PCP^{-1}:P=\begin{bmatrix}
> \mathrm{Re}(\mathbf{v})  & \mathrm{Im}(\mathbf{v})
> \end{bmatrix},C=\begin{bmatrix}
> a & -b \\
> b & a
> \end{bmatrix}
> $$