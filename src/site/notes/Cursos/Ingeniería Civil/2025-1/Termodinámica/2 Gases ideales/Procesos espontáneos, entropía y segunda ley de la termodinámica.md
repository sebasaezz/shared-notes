---
{"dg-publish":true,"permalink":"/cursos/ingenieria-civil/2025-1/termodinamica/2-gases-ideales/procesos-espontaneos-entropia-y-segunda-ley-de-la-termodinamica/","tags":["I2IIQ1003"]}
---

# Espontaneidad

Un proceso ==es espontaneo== si ocurre sin intervención externa **a pesar de su velocidad**.

Un proceso ==no es espontaneo== si requiere de intervención externa.

No existe una relación clara entre la entalpía y la espontaneidad. Sino que existe relación entre la **entropía** y la espontaneidad.

## Con energía libre

Se conoce la espontaneidad de una reacción únicamente utilizando la entropía y temperatura utilizando la [[Cursos/Ingeniería Civil/2024-1/Química para Ingeniería/4 Termoquímica. Energía y Quimíca/Energía libre de Gibbs (G)\|Energía libre de Gibbs (G)]]:

Si $\Delta G<0$ el proceso es espontáneo

Si $\Delta G>0$ el proceso no es espontáneo

Si $\Delta G=0$ el proceso está en equilibrio

# Entropía ($S$)

Característica de un proceso espontaneo, define el incremento de una propiedad termodinámica.

Se puede decir que la entropía mide las posibilidades de que suceda cierto proceso químico espontaneo. La dirección de los procesos siempre va hasta una configuración que tenga la menor posibilidad de cambio, mayor _desorden_, menor número de **micro-estados**.

Es una medida cuantitativa del número de **micro-estados disponibles** para una molécula de un sistema. Así siendo las formas en la que la energía de la molécula puede ser ordenada.

Una reacción ocurre por que es mucho más probable que ocurra, y es muy improbable que no ocurra.

## Entropía en estados de la materia
$$
S_{s}<S_{l}<S_{g}
$$

Los gases tienen un mayor número de posibles micro-estados que un sólido.

## Factores que inciden en la entropía
### Temperatura

En teoría, solo el calor afecta a la entropía

La siempre temperatura aumenta la entropía de un sistema. El aumento en la temperatura implica que $\Delta S_{\pu{ ambiente }}>0 \implies \Delta S_{\pu{ sistema }}\gg 0$.

Matemáticamente, se logra definir a la entropía como: $\boxed{\Delta S_{\pu{ ambiente }}=-\frac{q}{T}}$ 

y si $P$ es constante: $\boxed{\Delta S_{\pu{ ambiente }}=-\frac{\Delta H}{T}}$.

Así, la magnitud del cambio entrópico depende de la $T$ a la cual $Q$ es transferido.

Si $T$ es alta, el efecto es pequeño. Si $T$ es baja, el efecto es mayor.

## Unidad de la entropía

La entropía se mide en $\frac{J}{K}$, es decir, su dimensión es $ET^{-1}$.

## Predicciones cualitativas de Entropía en Reacciones químicas

Si se tiene una menor ==cantidad de moléculas== resultantes, entonces van a haber menores configuraciones posicionales en el resultado. Por ejemplo:

$$
N_{2}+3H_{2} \rightarrow 2NH_{3}
$$

Como se tiene una menor cantidad de moléculas, se infiere que $\Delta S<0$

También se puede inferir por lo ==estados de la materia==:

$$
H_{2}O_{(l)} \rightarrow H_{2}O_{(s)}
$$

La entropía disminuye dado que los sólidos tienen menor entropía, $\Delta S<0$.

## Entropía estandar ($\Delta Sº$)

Una función de estado que considera el cambio de entropía de una reacción en condiciones estándar:

$$
\Delta Sº=\sum_{}^{}n_{p} Sº(\pu{ productos})-\sum_{}^{}n_{r}Sº(\pu{ reactivos})
$$
# Entropía con propiedades medibles
#I2IIQ1003 
$$
dS=\frac{dQ_{\text{rev}}}{T}
$$
$$
\implies S=\int_{Q_{1}}^{Q_{2}} \frac{dQ}{T}  
$$
Recordar que con la [[Cursos/Ingeniería Civil/2025-1/Termodinámica/Unidad 1/5 Calorimetría/Calorimetría, capacidad calorífica y calor latente\|definicion de Cp]]:
$$
dQ=C_{p}dT
$$
Entonces, a presión constante:
$$
\Delta S_{12}=\int_{T_{1}}^{T_{2}} \frac{C_{p}}{T} \, dT 
$$

Luego:
$$
\Delta S_{12}=\underbrace{ C_{V}\ln \frac{T_{2}}{T_{1}} }_{ V=cte }=\underbrace{ C_{P}\ln \frac{T_{2}}{T_{1}} }_{ P=cte }
$$
En sólidos y líquidos, la entropía _casi_ no depende de la presión, entonces se puede usar $C_{p}$.

También se puede usar [[Cursos/Ingeniería Civil/2025-1/Termodinámica/Unidad 1/2 Comportamiento de sustancia puras y tablas termodinámicas/Calidad y regla de la palanca\|Calidad y regla de la palanca]]:
$$
x=\frac{S-S_{\text{L}}}{S_{\text{V}}-S_{\text{L}}}
$$
# Cambio de fase
Así como antes se tenía un $\Delta H_{\text{vap}}$, se puede usar para calcular la $\Delta S_{\text{vap}}$.
$$
\Delta S_{\text{vap}}=\frac{\Delta H_{\text{vap}}}{T^{\text{sat}}}
$$
# La segunda ley de la termodinámica

"En cualquier proceso espontaneo, siempre hay un **incremento** en la entropía del universo"

Recordando que:

$$
\Delta S_{u}=\Delta S_{\pu{ sistema }}+\Delta S_{\pu{ ambiente }}
$$
- Si $\Delta S_{u}>0$, la entropía del universo aumenta y el proceso es **espontaneo**.
- Si $\Delta S_{u}<0$, la entropía del universo disminuye y el proceso **no es espontaneo**, es decir, es espontaneo en la dirección opuesta. Este proceso no es real.
- Si $\Delta S_{u}=0$, el proceso está en reposo o equilibrio, es su valor máximo.

# Entropía de un baño térmico

Un baño térmico, que es un sistema tan grande que su temperatura no cambia pudiendo absorber y ceder energía, tiene una entropía dada por:
$$
\Delta S_{\text{baño}}=\frac{Q_{\text{baño}}}{T_{\text{baño}}}
$$
Ahora el cambio de entropía en un sistema dentro de un baño será el opuesto a la entropía del baño:
$$
\Delta S_{\text{sistema}}=-\frac{Q_{\text{baño}}}{T_{\text{baño}}}
$$


# Tercera ley de la termodinámica

Si bien siempre se consideran cambios en la termodinámica, pero resulta que la entropía es una característica absoluta (se tiene), por ejemplo, _la entropía de un cristal perfecto a $0K$ es 0_. Este es el enunciado de la tercera ley de la termodinámica.
