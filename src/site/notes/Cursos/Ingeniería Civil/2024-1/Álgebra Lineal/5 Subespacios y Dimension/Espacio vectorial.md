---
{"dg-publish":true,"permalink":"/cursos/ingenieria-civil/2024-1/algebra-lineal/5-subespacios-y-dimension/espacio-vectorial/","tags":["I2MAT1203"]}
---

# Concepto

Un espacio $V$ es un conjunto de vectores (elementos de $V$), definidos por dos operaciones, la suma y la multiplicación por escalares. Estas dos sujetas a 10 axiomas.

# Definición

Los siguientes axiomas deben ser válidos para los vectores $u$, $v$ y $w$ en el espacio $V$.

1. Si $u+v\in V$
2. $u+v=v+u$
3. Propiedad asociativa de la suma $u+(v+w)=(u+v)+w$
4. Existe el vector $0$ tal que $u+0=u$
5. $\forall u \exists(-u):u+(-u)=0$
6. $cu\in V:c\in\mathbb{R}$
7. $c(u+v)=cu+cv$
8. $(c+d)u=cu+du:d\in\mathbb{R}$
9. $c(du)=(cd)u:d\in\mathbb{R}$
10. $1·u=u$
Notas:
- En el axioma $4$ el elemento nulo es único
# Ejemplo
- Los espacios $\mathbb{R}^{n}:n\geq 1$ son espacios vectoriales.
## Ejemplo geométrico

Sea $V$ el espacio formado por todas las flechas, se considera que dos flechas son iguales si tienen la misma longitud y dirección. Se define la suma como la flecha que conecta a las dos, y a la ponderación como la multiplicación del largo de la flecha.

Si se revisan todos los axiomas, se nota que todos se cumplen.

## Ejemplo de señales discretas

Se define el espacio $S$ todas las sucesiones doblemente infinitas de números.

es decir, vectores definidos por $\{ y_{k\in\mathbb{Z}}=\{ \dots, y_{-2},y_{-1},y_{0}  \} \}$

Se puede definir a otro elemento de $S$ de la misma forma. Así, se define la suma como la suma entre cada entrada de la sucesión. Así se revisan todos los axiomas y se nota que se cumplen todas.

## Ejemplo: Espacio de polinomios de grado $n$ o menor

Se define a un espacio $\mathbb{P}_{n}$ tal que sean los polinomios de grado $n$ o menor, es decir, dados por la función:

$$
p(t)=a_{0}+a_{2}t+a_{3}t^{2}+a_{n}t^{n}
$$

Se puede definir un polinomio $q(t)$ de la misma forma, y se van a cumplir todos los axiomas.

### ¿Se cumple si se define el espacio para $n=n$ y no $n\leq n$?

No, ya que la resta (o suma) de polinomios de grado $n$ puede dar un polinomio de grado menor a $n$. Por ejemplo:

$$
(2t-t^{2})+(2t+t^{2})
$$