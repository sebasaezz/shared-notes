---
{"dg-publish":true,"permalink":"/cursos/ingenieria-civil/2025-1/ecuaciones-diferenciales/1-edos-de-primer-orden/4-modelos-de-poblacion/modelos-de-poblacion-con-ed-os-y-ecuacion-logistica/","tags":["ExMAT1640"]}
---

# Concepto
Se usan EDOs para modelar crecimiento de poblaciones dada una rasa de mortalidad $\delta(t)$ y una tasa de natalidad $\beta(t)$.
# Definición
Los modelos de población cumplen que:
$$
\frac{ dP }{ dt } =\underbrace{ (\beta-\delta) }_{ k }P
$$
$k$ puede ser un **factor de velocidad de crecimiento**, y la solución sera:
$$
P(t)=Ce^{kt}
$$
Esto se interpreta como que si $k$ es negativo, la población decrece y si $k$ es positivo esta va a crecer. Si $k=0$, se encuentra en equilibrio.
Si $k$ es constante, el modelo es poco realista, ya que las poblaciones crecen sin límite.
# Ecuación logística
Nace de tratar a $k$ como una función $k(t)=\beta(t)-\delta(t)$.
Asumiendo que $\delta=0$, es decir, no hay muertes, se peude esperar que la taza de natalidad $\beta$ disminuya con la población:
$$
\beta=a-bP:a,b>0
$$
Ahora la ecuación es:
$$
\frac{ dP }{ dt } =(a-bP)P
$$
Esta es la ecuación logística, usualmente mostrada como:
$$
\frac{ dP }{ dt } =b\left( \frac{a}{b}-P \right)P
$$
Mostrando a $\frac{a}{b}=M$, el punto de estabilidad y $b=k$.
$$
\frac{ dP }{ dt } =k(M-P)P
$$
Finalmente:
$$
P(t)=\frac{MP_{0}}{P_{0}+(M-P_{0})e^{-kMt}}
$$
Notar que:
$$
\lim_{ t \to \infty } \frac{MP_{0}}{P_{0}+(M-P_{0})e^{-kMt}}=M
$$
Esto es que la población se equilibra siempre en un punto dado por $M$, la **[[Cursos/Ingeniería Civil/2024-2/Biología de Organismos y Comunidades/3 Ecología y Cambio Global/Introducción a la ecología de poblaciones\|capacidad de carga]]**.
![Pasted image 20250327114124.png|400](/img/user/Cursos/Ingenier%C3%ADa%20Civil/2025-1/Ecuaciones%20diferenciales/1%20Edos%20de%20primer%20orden/4%20Modelos%20de%20poblaci%C3%B3n/attachments/Pasted%20image%2020250327114124.png)
## Casos en los que se puede usar
- Cuando al situación ambiental es limitada
- Cuando hay una situación de competencia
	- $\delta=kP-a$
- Cuando hay una situación proporcional a encuentros, por ejemplo un resfrío
	- $P=\# \text{ personas enfermas}$ 
	- $M-P=\# \text{ personas sanas}$ 
## Si la natalidad crece junto a la población
Ahora la ecuación será la misma pero inversa:
$$
\frac{ dP }{ dt } =k(P-M)P
$$
Ahora la solución será la misma pero con signos cambiados:
$$
P(t)=\frac{MP_{0}}{P_{0}+(M-P_{0})e^{kMt}}
$$
# Ejemplo