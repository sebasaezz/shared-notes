---
{"dg-publish":true,"permalink":"/cursos/ingenieria-civil/2024-2/calculo-ii/1-integrales-impropias-y-series/1-6-series-alternantes/series-alternantes/","tags":["I1MAT1620"]}
---

# Concepto

Series que suman y se restan.

# Definición

> [!definition] serie alternante y propiedades
> $$
> \sum_{n=1}^{\infty}(-1)^{n-1}b_{n}=b_{1}-b_{2}+b_{3}-b_{4}+b_{5}-b_{6}+\cdots:b_{n}>0
> $$
> Si se cumple que
> 1. $b_{n+1}\leq b_{n} : \forall n$   (es decreciente)
> 2. $\lim_{ n \to \infty } b_{n}=0$
> Entonces ($\implies$) la serie converge, notar que $\cancel{ \iff }$
> ![Pasted image 20240823113505.png](/img/user/Cursos/Ingenier%C3%ADa%20Civil/2024-2/C%C3%A1lculo%20II/1%20Integrales%20Impropias%20y%20Series/1.4%20Series.%20Definici%C3%B3n%20de%20sumas%20parciales.%20Convergencia%20de%20series.%20Convergencia%20absoluta/attachments/Pasted%20image%2020240823113505.png)

# Estimación

> [!theorem] Estimación de series alternantes
> Si $s=\sum(-1)^{n-1}b_{n}$ es la suma de una serie alternante con:
> 
> 1. $b_{n+1} \leq b_{n}$ (es decreciente)
> 2. $\lim_{ n \to \infty } b_{n}=0$
> $$
> |R_{n}|=|s-s_{n}|\leq b_{n+1}
> $$

`\begin{proof}`

Se sabe que $s_{n}$ **crece**, ya que se va a tener un patrón de la forma

- $s_{1}=b_{1}>0$
- $s_{2}=b_{1}-b_{2}>0$
	- $s_{3}=(b_{1}-b_{2})+b_{3}>0$
Y así, entonces finalmente se podrá agrupar de la forma:
$$
s_{n}=b_{1}-\underbrace{ (b_{2}-b_{3})-(b_{4}-b_{5})-(b_{6}-b_{7}) }_{ >0 }\dots\leq b_{1}
$$

Así, se cumplirá que:

$$
|R_{n}|=|s-s_{n}|\leq b_{n+1}
$$
$$
s=\underbrace{ b_{1}-b_{2}+b_{3}-b_{4}+b_{5}-\dots+b_{n} }_{ s_{n} }-\underbrace{ b_{n+1}+b_{n+2}-\cdots }_{ R_{n} }
$$

`\end{proof}`

# Ejemplo

Sea la serie:

$$
\underbrace{ \sum_{n=1}^{\infty} (-1)^{n}\frac{1}{n} }_{ 1-\frac{1}{2}+\frac{1}{3}-\frac{1}{4}+\frac{1}{5}-\cdots }
$$
$$
b_{n}=\frac{1}{n} \begin{cases}
\rightarrow \text{decreciente} \\
\rightarrow\lim_{ n \to \infty } \frac{1}{n}=0
\end{cases}\begin{cases}
 \\
 \checkmark\\
 \\
\end{cases} \therefore \text{converge  😀}
$$
