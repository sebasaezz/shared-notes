---
{"dg-publish":true,"permalink":"/cursos/ingenieria-civil/2025-1/termodinamica/tareas/t3/tarea-opcional-3-termodinamica/"}
---

# Pregunta 1

> [!quote]
> Se le entregan isotérmicamente $500 \, \pu{ kJ}$ de calor a un estanque cerrado que contiene $2.3 \, \pu{ kg}$ de Aire a $20\, \pu{ ºC}$ y $1 \, \pu{bar}$. Posteriormente sufre un compresión adiabática y reversible hasta $300 \, \pu{°C}$. Considere que el Aire se comporta como un gas ideal. $Cp = 1.005 \, \pu{\frac{kJ}{kg·K}}$, $\gamma = 1.4$, $PM = 29 \, \pu{\frac{g}{mol}}$.

## Inciso a)

> [!quote]
> Calcule el volumen y presión inicial.

Se le llamará estado 0 al previo a la adición de calor y estado 1 al posterior.

### Estado 0

Al inicio, se asume la existencia de un gas ideal (aire). De este se tienen los siguientes datos:

- $m=2.3\, \pu{ kg}$
- $T_{0}=T_{1}=20\, \pu{ ºC}=293.15\, \pu{ K}$
- $P_{0}=1\, \pu{ bar}$

Esto es suficiente para caracterizar el sistema usando la ecuación de los gases ideales:

$$
\begin{align}
PV & =nRT \\
V_{0} & =nR\frac{T_{0}}{P_{0}} 
\end{align}
$$

Para obtener el número de moles $n$ se debe usar le peso molecular dado:

$$
n=\frac{m}{PM}=2.3\, \pu{ \cancel{ kg }}  · \frac{1000 \, \pu{ \cancel{ g }}} {1 \, \cancel{ \pu{ kg} }}· \frac{1}{29} \, \pu{ \frac{mol}{\cancel{ g }}}= 79.31 \, \pu{ mol}
$$

Ahora:

$$
\begin{align}
V_{0} & =79.31\, \pu{ \cancel{ mol }}· 8.314 \, \pu{ \frac{J}{\cancel{ mol }·\cancel{ K }}}· \frac{293.15\, \pu{ \cancel{ K }}}{100000 \, \pu{ Pa}} \\
 & =1.9330 \, \pu{ J} · \, \pu{  Pa^{-1}} \\
 & =1.9330 \, \pu{ \frac{\cancel{ kg } ·m^{2}}{\cancel{ s^{2} }}} · \, \pu{ \frac{m ·\cancel{ s^{2} }}{\cancel{ kg }}} \\
 & =1.9330\, \pu{ m^{3}}
\end{align}
$$

### Estado 1

Posteriormente, al agregar los $500 \, \pu{ kJ}$ de calor de **forma isotérmica**, se tiene un caso donde:

$$
\Delta U=0 \implies Q=-W
$$

Y al reemplazar la ecuación de los gases ideales en la ecuación del trabajo (visto en clases), se tiene que:

$$
\begin{align}
Q & =nRT\ln\left( \frac{V_{1}}{V_{0}} \right) \\
\frac{Q}{nRT} & =\ln \left( \frac{V_{1}}{V_{0}} \right)  \\
V_{1} & =V_{0}·\exp\left( \frac{Q}{nRT} \right) \\
V_{1} & = 1.9330\, \pu{ m^{3}} · \exp\left( \frac{500000\,\pu{\cancel{ J }}}{79.31 \, \pu{ \cancel{ mol }}·8.314 \, \pu{ \frac{\cancel{ J }}{\cancel{ mol }·\cancel{ K }}}·293.15\, \pu{ \cancel{ K }}} \right) \\
V_{1} & =1.9330\, \pu{ m^{3}}·e^{2.5867}=25.6815\, \pu{ m^{3}}
\end{align}
$$

Para calcular la presión, se usa una fórmula muy similar que aprovecha que $V_{i}=\frac{nRT}{P_{i}}$:

$$
\begin{align}
Q & =nRT\ln\left( \frac{P_{0}}{P_{1}} \right) \\
P_{1} & =P_{0}·\exp\left( -\frac{Q}{nRT}  \right) \\
P_{1} & =1\, \pu{ bar} · e^{-2.5867} \\
 & =0.07527\, \pu{ bar}
\end{align}
$$

En resumen, al agregar los $500\, \pu{ kJ}$:

- $V_{1}=25.6815 \, \pu{ m^{3}}$
- $P_{1}=0.07527 \, \pu{ bar}$

<div class="page-break" style="page-break-before: always;"></div>

## Inciso b)

> [!quote]
> Calcule el volumen y presión final.

Se tienen los siguientes datos:

- Compresión adiabática reversible
- $T_{2}=300\, \pu{ ºC}=573.15\, \pu{ K}$
- $Cp_{\text{aire}}=1.005 \, \pu{ \frac{kJ}{kg·K}}$
- $\gamma=1.4=\frac{Cp}{Cv}$

En los procesos adiabáticos reversibles con gases ideales se cumple lo siguiente por lo visto en clases:

$$
\frac{P_{2}}{P_{1}}=\left( \frac{T_{2}}{T_{1}} \right)^{C_{P}/R} \iff\frac{V_{1}}{V_{2}}=\left( \frac{T_{2}}{T_{1}} \right)^{C_{P}/R - 1}
$$

Entonces:

$$
\begin{align}
P_{2} & = P_{1} · \left( \frac{T_{2}}{T_{1}} \right)^{Cp/R} \\
 & =0.07527\, \pu{ bar}·\left( \frac{573.15\, \pu{ \cancel{ K }}}{293.15\, \pu{ \cancel{ K }}} \right)^{1005 \, \pu{ \frac{\cancel{ J }}{\cancel{ kg }·\cancel{ K }}}·2.3\, \pu{ \cancel{ kg }}·\frac{1}{8.314} \, \pu{ \frac{\cancel{ mol }·\cancel{ K }}{\cancel{ J }}}·\frac{1}{79.31 \, \pu{ \cancel{ mol }}}} \\
 & =0.07527\, \pu{ bar}·10.489 \\
 P_{2}& =0.7895\, \pu{ bar}
\end{align}
$$

Ahora para $V_{2}$:

$$
\begin{align}
V_{2} & =V_{1} \left( \frac{T_{2}}{T_{1}} \right)^{-(Cp/R-1)} \\
 & =25.6815 \, \pu{ m^{3}} · \left( \frac{573.15\, \pu{ \cancel{ K }}}{293.15\, \pu{ \cancel{ K }}} \right)^{-\left( 1005 \, \pu{ \frac{\cancel{ J }}{\cancel{ kg }·\cancel{ K }}}·2.3\, \pu{ \cancel{ kg }}·\frac{1}{8.314} \, \pu{ \frac{\cancel{ mol }·\cancel{ K }}{\cancel{ J }}}·\frac{1}{79.31 \, \pu{ \cancel{ mol }}}-1 \right)} \\
 & =25.6815\, \pu{ m^{3}}·0.1864 \\
 V_{2}& =4.7869\, \pu{ m^{3}}
\end{align}
$$
<div class="page-break" style="page-break-before: always;"></div>

## Inciso c)

> [!quote]
> Calcule el trabajo requerido en el segundo proceso

Se sabe que $Cv=\left( \frac{ \partial U }{ \partial T } \right)_{V}$, y si es adiabático, $\Delta U=W$, entonces:

$$
\Delta U=\int_{T_{1}}^{T_{2}} Cv \, dT =W
$$

Ahora, para obtener $Cv$ se puede usar el valor de $\gamma=\frac{Cp}{Cv}$ y el valor de $Cp$:

$$
Cv= \frac{Cp}{\gamma}=\frac{1.005}{1.4} \, \pu{ \frac{kJ}{kg·K}}=0.7178\, \pu{ \frac{kJ}{kg·K}}
$$

Reemplazando:

$$
\begin{align}
W & =\int_{T_{1}}^{T_{2}} Cv · m \, dT  \\
 & =Cv·m·(T_{2}-T_{1}) \\
 & =0.7178 \, \pu{ \frac{kJ}{\cancel{ kg }·K}}·2.3 \, \pu{ \cancel{ kg }}·(573.15\, \pu{ K}-293.15\, \pu{ K}) \\
 & =1.6512 \, \pu{ \frac{kJ}{\cancel{ K }}}·280\, \pu{ \cancel{ K }} \\
 W& =462.3\, \pu{ kJ}
\end{align}
$$
## Inciso d)

> [!quote]
> Calcule la variación de Entalpía del segundo proceso

De la misma forma que antes, se tiene que $Cp=\left( \frac{ \partial H }{ \partial T } \right)_{P}$, entonces:

$$
\begin{align}
\Delta H & =\int_{T_{1}}^{T_{2}} Cp·m \, dT \\
 & =Cp·m·(T_{2}-T_{1}) \\
 & =1.005\, \pu{ \frac{kJ}{\cancel{ kg }·\cancel{ K }}}·2.3\, \pu{ \cancel{ kg }}·280\, \pu{ \cancel{ K }} \\
 \Delta H& =647.22\, \pu{ kJ}
\end{align}
$$
<div class="page-break" style="page-break-before: always;"></div>

# Problema 2

> [!quote]
> $10$ moles de un gas están contenidos en un contenedor rígido. Inicialmente el gas se encuentra a $0.5 \, \pu{ bar}$ y $300\, \pu{ K}$, además el contenedor también esta a $300\, \pu{ K}$. Se introduce el contenedor dentro de un horno muy grande a $600 \, \pu{ K}$. El contenedor se deja hasta que tanto el gas como el contenedor alcanzan el equilibrio térmico con los alrededores. El gas se puede considerar como un gas ideal con $Cv = 2.5R$. El contenedor en si tiene una masa de $10 \, \pu{ kg}$ (sin considerar la masa del gas en su interior) y con una capacidad calorífica de $1.5 \, \pu{ \frac{J}{g·K}}$.

## Inciso a)

> [!quote]
> Calcule la cantidad de calor añadida al gas.

Como nos encontramos en un proceso isocórico (contenedor rígido), se puede usar que:

$$
Cv=\left( \frac{ \partial U }{ \partial T }  \right)_{V}
$$

Usando los datos entregados:

- $n=10\, \pu{ mol}$
- $T_{1}=300\, \pu{ K}$
- $T_{2}=600\, \pu{ K}$
- $Cv=2.5R$

Entonces:
$$
\begin{align}
\Delta U_{\text{gas}}=Q_{\text{gas}} & =n\int_{T_{1}}^{T_{2}} Cv \, dT  \\
 & =n·Cv(T_{2}-T_{1}) \\
 & =10\, \pu{ \cancel{ mol }}·2.5·8.314 \, \pu{ \frac{\cancel{ J }}{\cancel{ mol }·\cancel{ K }}}·(600-300)\, \pu{ \cancel{ K }} · \frac{1\, \pu{ kJ}}{1000\, \pu{ \cancel{ J }}} \\
 & =62.355\, \pu{ kJ}
\end{align}
$$

Entonces el calor que entra al sistema es de $Q_{\text{gas}}=62.355\, \pu{ kJ}$.

<div class="page-break" style="page-break-before: always;"></div>

## Inciso b)

> [!quote]
> Calcule la cantidad de calor añadida al contenedor.

Con los datos para el contenedor:

- $T_{1}=300\, \pu{ K}$
- $T_{2}=600\, \pu{ K}$
- $C_{\text{cont}}=1.5\, \pu{ \frac{J}{g·K}}$
- $m_{\text{cont}}=10\, \pu{ kg}=10000\, \pu{ g}$

Se usan los mismos conceptos ya vistos, pero aplicados a la capacidad calorífica del contenedor:
$$
\begin{align}
Q_{\text{cont}} & =C_{\text{cont}}·m·\Delta T \\
 & =1.5 \, \pu{ \frac{\cancel{ J }}{\cancel{ g }·\cancel{ K }}}·10000\, \pu{ \cancel{ g }}·(600-300)\, \pu{ \cancel{ K }} · \frac{1\, \pu{ kJ}}{1000\, \pu{ \cancel{ J }}} \\
 & =4500\, \pu{ kJ}
\end{align}
$$
## Inciso c)

> [!quote]
> Calcule el cambio de entropía para el gas.

En un proceso isocórico, la entropía está dada por:

$$
\begin{align}
\Delta S_{\text{gas}} & =n\int_{T_{1}}^{T_{2}} \frac{Cv}{T} \, dT \\
 & =n·Cv ·\ln\left( \frac{T_{2}}{T_{1}} \right) \\
 & =10\, \pu{ \cancel{ mol }}·2.5·8.314 \, \pu{ \frac{\cancel{ J }}{\cancel{ mol }·K}}·\ln\left( \frac{600\, \pu{ \cancel{ K }}}{300\, \pu{ \cancel{ K }}} \right) · \frac{1\, \pu{ kJ}}{1000\, \pu{ \cancel{ J }}}  \\
 & =0.1441\, \pu{ \frac{kJ}{K}}
\end{align}
$$
<div class="page-break" style="page-break-before: always;"></div>

## Inciso d)

> [!quote]
> Calcule el cambio de entropía del universo

Para esto, primero se debe calcular la diferencia de entropía del contenedor. Esto se hace de manera similar al gas, ya que es un cuerpo que se calienta a presión constante.

$$
\begin{align}
\Delta S_{\text{cont}} & =m·C_{\text{cont}}·\ln\left( \frac{T_{2}}{T_{1}} \right) \\
 & =10000\, \pu{ \cancel{ g }}·1.5\, \pu{ \frac{\cancel{ J }}{\cancel{ g }·K}}·\ln\left( \frac{600\, \pu{ \cancel{ K }}}{300\, \pu{ \cancel{ K }}} \right)· \frac{1\, \pu{ kJ}}{1000\, \pu{ \cancel{ J }}}  \\
 & =10.3972\, \pu{ \frac{kJ}{K}}
\end{align}
$$

Ahora que se tiene la entropía del contenedor, se puede calcular la del sistema.

$$
\begin{align}
\Delta S_{\text{sistema}} & =\Delta S_{\text{gas}}+\Delta S_{\text{cont}} \\
 & =0.1441\, \pu{ \frac{kJ}{K}}+10.3972\, \pu{ \frac{kJ}{K}} \\
 & =10.5413\, \pu{\frac{kJ}{K}}
\end{align}
$$

Se define el cambio de entropía del universo como la suma del cambio de entropía del sistema con el del entorno. Para calcular $\Delta S_{\text{entorno}}$ se considera un baño a temperatura constante ($600\, \pu{ K}$), donde:

$$
\Delta S_{\text{entorno}}=\frac{-Q_{\text{sistema}}}{T_{\text{baño}}}
$$

Para calcular $Q_{\text{sistema}}$, se suman los calores del contenedor y del gas.

$$
\begin{align}
Q_{\text{sistema}} & =Q_{\text{gas}}+Q_{\text{cont}} \\
 & =62.355\, \pu{ kJ}+4500\, \pu{ kJ} \\
 & =4562.355\, \pu{ kJ}
\end{align}
$$

Ahora:

$$
\Delta S_{\text{entorno}}=\frac{-4562.355\, \pu{ kJ}}{600\, \pu{ K}}=-7.6039\, \pu{ \frac{kJ}{K}}
$$

Finalmente:

$$
\begin{align}
\Delta S_{\text{universo}} & =\Delta S_{\text{sistema}}+\Delta S_{\text{entorno}} \\
 & =10.5413\, \pu{ \frac{kJ}{K}}-7.6039\, \pu{ \frac{kJ}{K}} \\
 & =2.9374\, \pu{ \frac{kJ}{K}}
\end{align}

$$

## Inciso e)

> [!quote]
> ¿Es este proceso reversible? ¿A qué se puede deber que sea reversible/irreversible?

Para responder esta pregunta, se debe analizar el cambio de entropía del universo, y se tiene que:

$$
\Delta S_{\text{universo}}=2.9374\, \pu{ \frac{kJ}{K}}>0
$$

Lo que indica que el proceso es espontaneo e irreversible. Para que el proceso sea reversible, se debe tener que $\Delta S_{\text{universo}}=0$.

El proceso es irreversible ya que al intercambiar calor con el entorno, es inevitable que parte de la energía se disipe y ya no pueda aprovecharse para realizar trabajo útil, lo que impide revertir el proceso sin dejar efectos en el entorno.