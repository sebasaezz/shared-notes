---
{"dg-publish":true,"permalink":"/cursos/ingenieria-civil/2024-1/algebra-lineal/1-ecuaciones-lineales-en-algebra-lineal/reduccion-por-filas-forma-escalonada-y-forma-escalonada-reducida-y-pivotes/"}
---

# El pivote

Entrada ==**distinta de 0** ==que se ocupa para disminuir a cero una entrada de otra fila en la misma columna. Es la primera desde la izquierda en una fila.

# La matriz escalonada

Una [[Cursos/Ingeniería Civil/2024-1/Álgebra Lineal/1 Ecuaciones lineales en álgebra lineal/Resolviendo sistemas de ecuaciones lineales con matrices aumentadas y matrices convenientes#^84222b\|forma escalonada]] , y también escalonada reducida, es una matriz en forma de "escalón", que avanza hacia abajo. Formalmente se podría definir como una matriz donde cada pivote ($\neq 0$) se encuentra más a la derecha del pivote de su fila superior. 

Las siguientes matrices se encuentran de forma escalonada. Los cuadrados son pivotes y los asteriscos pueden tomar cualquier valor.

![Pasted image 20240706142724.png](/img/user/Cursos/Ingenier%C3%ADa%20Civil/2024-1/%C3%81lgebra%20Lineal/1%20Ecuaciones%20lineales%20en%20%C3%A1lgebra%20lineal/attachments/Pasted%20image%2020240706142724.png)

## La matriz escalonada reducida

> [!definition] forma escalonada reducida
> Es una [[Cursos/Ingeniería Civil/2024-1/Álgebra Lineal/1 Ecuaciones lineales en álgebra lineal/Resolviendo sistemas de ecuaciones lineales con matrices aumentadas y matrices convenientes#^84222b\|forma escalonada]] , pero que todos los pivotes son 1, y todas las entradas superiores a los pivotes son 0.
{ #f3d075}


![Pasted image 20240706142733.png](/img/user/Cursos/Ingenier%C3%ADa%20Civil/2024-1/%C3%81lgebra%20Lineal/1%20Ecuaciones%20lineales%20en%20%C3%A1lgebra%20lineal/attachments/Pasted%20image%2020240706142733.png)

# Reducción por fila

Se le llama a la reducción por filas al procedimiento, mediante el cual, por medio de [[Cursos/Ingeniería Civil/2024-1/Álgebra Lineal/1 Ecuaciones lineales en álgebra lineal/Operaciones elementales de fila en matrices\|Operaciones elementales de fila en matrices]], se llega a diferentes matrices escalonadas.

> [!theorem] unicidad de la forma escalonada reducida
> Toda matriz tiene **solo una** representación en [[#^f3d075|forma escalonada reducida]].