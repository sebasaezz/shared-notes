---
{"dg-publish":true,"permalink":"/cursos/ingenieria-civil/2024-1/quimica-para-ingenieria/7-acidos-y-bases/acidos-y-bases-poliproticos/","tags":["I2QIM100E"]}
---

# Ácidos polipróticos

_Para las bases es lo mismo pero al revés_

Pueden ceder más de un protón en un equilibrio ácido-base. Es decir, dos o más protones se disocian. Notar que hay ácidos que no son polipróticos y tienen más de un hidrógeno.

## Disociación de ácidos polipróticos 

Los ácidos polipróticos se disocian dos (o más, pero la mayoría es dipróticos) veces. Cada disociación tiene su propia $K_{a}$.

Ejemplo de ácido poliprótico: Ácido sulfúrico ($H_{2}SO_{4}$)

$$
\begin{array}{rcl}
 & H_{2}SO_{4}+H_{2}O  & \rightleftharpoons &  HSO_{4}^{-}+H_{3}O^{+} & K_{a_{1}}=\text{mucho} \\
 & HSO_{4}^{-} +H_{2}O & \rightleftharpoons  & SO_{4}^{2-}+H_{3}O^{+} & K_{a_{2}}=1,1·10^{-2}
\end{array}
$$

Por cada disociación, el ácido se comportará más como base, es decir, $K_{a_{1}}>K_{a_{2}}>K_{a_{3}}>\cdots$

"Es como que va a ser una base conjugada pero no le da"

### Ejemplo más explicado: La disociación del ácido fosfórico

$$\begin{array}{r l}{{\mathrm{(1)~~~H_{3}P O_{4}+H_{2}O\rightleftharpoons H_{3}O^{+}+H_{2}P O_{4}{}^{-}}}}&{{K_{a_{1}}=\frac{\mathrm{[H_{3}O^{+}][H_{2}P O_{4}^{-}]}}{\mathrm{[H_{3}P O_{4}]}}=7,1\times10^{-3}}}\\ {{\mathrm{(2)~H_{2}P O_{4}{}^{-}+H_{2}O\rightleftharpoons H_{3}O^{+}+H P O_{4}{}^{2-}}}}&{{K_{a_{2}}=\frac{\mathrm{[H_{3}O^{+}][H P O_{4}{}^{2-}]}}{\mathrm{[H_{2}P O_{4}^{-}]}}=6,3\times10^{-8}}}\\ {{\mathrm{(3)~~~~H P O_{4}{}^{2-}+H_{2}O\rightleftharpoons H_{3}O^{+}+P O_{4}{}^{3-}}}}&{{K_{a_{3}}=\frac{\mathrm{[H_{3}O^{+}][P O_{4}{}^{3-}]}}{\mathrm{[H P O_{4}{}^{2-}]}}=4,2\times10^{-13}}}\end{array}$$

Notar como $K_{a_{1}}\ggg K_{a_{2}}$, entonces se puede aproximar que casi todos los protones ($H_{3}O^+$) van a venir del primer ácido ($H_{3}PO_{4}$). Entonces $[H_{3}O^{+}]\approx [H_{2}PO_{4}^{-}]$. Esto implicará que $K_{a_{2}}\approx \frac{\cancel{ [H_{3}O^{+}] }[HPO_{4}^{2-}]}{\cancel{ [H_{2}PO_{4}^{-}] }}\approx[HPO_{4}^{2-}]$. (este aproximado es **muy** parecido al punto que es directamente igual)

#### Ejercicio

En base a las constante vistas:

Para una disolución de $H_{3}PO_{4}$ a $3.0 \pu{ M }$, calcule: 

1. $[H_{3}O^{+}]$
2. $[H_{2}PO_{4}^{-}]$
Dado lo dicho anteriormente, se puede pensar al $H_{2}PO_{4}$ como un ácido monoprótico, así se puede aplicar la tabla:
Se sabe que
$$
\frac{[H_{3}O^{+}][H_{2}PO_{4}^{-}]}{[H_{3}PO_{4}]}=7.1· 10^{-3}
$$

|        | $[H_{3}PO_{4}]$ | $[H_{3}O^{+}]$ | $[H_{2}PO_{4}^{-}]$ |
| ------ | --------------- | -------------- | ------------------- |
| Inicio | $3\pu{ M }$     | $0$            | $0$                 |
| Cambio | $-x$            | $+x$           | $+x$                |
| Final  | $3\pu{ M }-x$   | $x$            | $x$                 |

Ahora se tiene que:

$$
\frac{x^{2}}{(3\pu{ M }-x)}=7.1·10^{-3}
$$

Resolviendo se tiene que: $x=0,142\pu{ M }=[H_{3}O^{+}]=[H_{2}PO_{4}^{-}]$