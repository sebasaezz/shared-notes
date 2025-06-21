---
{"dg-publish":true,"permalink":"/cursos/ingenieria-civil/2025-1/calculo-iii/2-campos-vectoriales/formas-vectoriales-del-teorema-de-green-y-flujo/","tags":["I3MAT1630"]}
---

Considerar a un campo vectorial conservativo $F=\langle P,Q \rangle$ como si estuviese en tres dimensiones $F=P\mathbf{i}+Q\mathbf{j}+0\mathbf{k}$.
Se va a tener que:
$$
\oint_{C}\mathbf{F}·d\mathbf{r}=\iint_{D}(\operatorname{rot}\mathbf{F})·\mathbf{k} dA
$$
Esto es la integral de lineal de la componente tangencial ($d\mathbf{r}=\mathbf{T}ds$). Si se toma la integral de línea de la componente normal, con $\mathbf{n}$ el vector normal unitario:
$$
\oint_{C}\mathbf{F}·\mathbf{n}\,ds=\iint_{D}\operatorname{div}\mathbf{F}(x,y)\, dA
$$
# Flujo
El valor de $\oint_{C}\mathbf{F}·\mathbf{n}\,ds$ se denomina flujo, y se puede interpretar que si se tiene una región cerrada dentro de un campo vectorial, entonces este valor toma "lo que entra" a la región menos "lo que sale".
- Si el flujo es positivo, el campo tiende de salir de la región.
- Si el flujo es negativo, el campo tiende a entrar a la región encerrada.
![output.png](/img/user/Cursos/Ingenier%C3%ADa%20Civil/2025-1/C%C3%A1lculo%20III/2%20Campos%20vectoriales/attachments/output.png)
# Ejemplo