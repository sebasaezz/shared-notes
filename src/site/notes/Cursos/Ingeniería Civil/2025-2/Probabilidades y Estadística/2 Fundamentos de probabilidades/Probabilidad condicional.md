---
{"dg-publish":true,"permalink":"/cursos/ingenieria-civil/2025-2/probabilidades-y-estadistica/2-fundamentos-de-probabilidades/probabilidad-condicional/","tags":["I1EYP1113"]}
---

# Concepto
Cuando un evento depende del resultado de otro
# Definición
Se define a la probabilidad que ocurra un evento $E_{1}$ bajo el supuesto de que otro evento $E_{2}$ ocurre con certeza:
$$
P(E_{1}|E_{2})= \frac{P(E_{1} \cap E_{2})}{P(E_{2})} \tag{1}
$$
## Corolarios
Si $\overline{E_{1}}$ es el complemente de $E_{1}$, y se condicionan los eventos a $E_{2}$:
$$
\begin{align}
P(E_{1}|E_{2}) & = \frac{P(E_{1} \cap E_{2})}{P(E_{2})}   & P(\overline{E_{1}}|E_{2}  ) & = \frac{P(\overline{E_{1}}\cap E_{2})}{P(E_{2})} 
\end{align}
$$
Como $P(E_{1} \cap E_{2})+P(\overline{ E_{1}}\cap E_{2})=P(E_{2})$, al sumas las ecuaciones se tiene:
$$
P(\overline{E_{1}}|E_{2})=1-P(E_{1}|E_{2})
$$
## Ejemplo
Ejemplo: Sacar un 5 en un dado ($E_{1}$), considerando que salió un número impar ($E_{2}$).
- $P(E_{1})=\frac{1}{6}$
- $P(E_{2})=\frac{1}{2}$
- $P(E_{1} \cap E_{2})=P(E_{1})=\frac{1}{6}$
$$
P_{E_{2}}(E_{1})=P(E_{1}|E_{2})= \frac{\frac{1}{6}}{\frac{1}{2}}=\frac{1}{3}
$$
Esta nueva probabilidad cumple los [[Cursos/Ingeniería Civil/2025-2/Probabilidades y Estadística/2 Fundamentos de probabilidades/Elementos de teoría de conjuntos en probabilidad y axiomas de la probabilidad\|axiomas de probabilidad]].
# Ley multiplicativa
Se puede sacar de la Ecuación 1, que:
$$
P(E_{1} \cap E_{2})=P(E_{1}|E_{2})\cdot P(E_{2})
$$
Para 3 eventos:
$$
P(E_{1} \cap E_{2} \cap E_{3})=\begin{cases}
P(E_{3} | E_{1} \cap E_{2})\cdot \underbrace{ P(E_{1} |E_{2})\cdot P(E_{2}) }_{ P(E_{1} \cap E_{2}) } \\
P(E_{1} \cap E_{2} |E_{3})\cdot  P(E_{3})
\end{cases}
$$
Ojo que lo de arriba pudo ser $P(E_{3}|E_{1}\cap E_{2})\cdot P(E_{2}|E_{1})\cdot P(E_{1})$, ya que la intersección es conmutativa.
# Independencia estadística
Se dice que dos eventos son estadísticamente independientes si la ocurrencia de uno no depende de la ocurrencia (o no ocurrencia) de otro. Matemáticamente:
$$
\begin{align}
P(E_{1}|E_{2})=P(E_{1}) &  &  \text{o}& &  P(E_{2}|E_{1})=P(E_{2})
\end{align}
$$
Aplicando esto a la ley multiplicativa, se tiene que para eventos$E_{1}$ y $E_{2}$ independientes:
$$
P(E_{1} \cap E_{2})=P(E_{1})· P(E_{2})
$$
## Independencia mutua

Ahora se puede tomar este requerimiento de la ley multiplicativa para asegurar independencia. Pero no es tan simple como asegurar que todas las probabilidades de un conjunto de eventos multiplicadas sea la probabilidad de la unión. Se necesita asegurar que cada subconjutno de eventos también cumpla este requerimiento.

Considerando eventos $E_{1},E_{2},\dots,E_{n}$. Se dice que etos eventos son mutualmente independientes si y solo si para cualquier sub-colección de eventos $E_{i_{1}},E_{i_{2}},\dots,E_{i_{m}}$ se cumple que:
$$
P(E_{i_{1}}\cap E_{i_{2}}\cap\dots \cap E_{i_{m}})=P(E_{i_{1}})\times P(E_{i_{2}})\times\dots  \times P(E_{i_{m}})
$$
Otra forma de decirlo es que si $\mathcal{E}=\{ E_{1},E_{2},\dots,E_{n} \}$, se dice que los eventos de $\mathcal{E}$ son mutualmente independientes si y solo si: 
$$
\forall I \subseteq \{ 1,2,\dots ,n \}, P\left( \bigcap_{i\in I}^{}E_{i} \right)=\prod_{i\in I}^{}P(E_{i})
$$

## Propiedades de la independencia
- Si $E_{1}$ y $E_{2}$ son independientes, entonces $\overline{E_{1}}$ y $\overline{E_{2}}$ también los son.
- Si $E_{1}$ y $E_{2}$ son independientes dado un evento $A$, entonces:
$$
P(E_{1} \cup E_{2}|A)=P(E_{1}|A)\times P(E_{2}|A)
$$
Esta última propiedad se ve así para eventos cualquiera:
$$
P(E_{1} \cup E_{2} |A)=P(E_{1}|A)+P(E_{2}|A)-P(E_{1} \cap E_{2} |A)
$$
# Ejemplo
