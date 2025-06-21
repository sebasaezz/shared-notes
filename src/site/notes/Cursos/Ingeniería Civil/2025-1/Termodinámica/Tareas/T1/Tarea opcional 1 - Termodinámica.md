---
{"dg-publish":true,"permalink":"/cursos/ingenieria-civil/2025-1/termodinamica/tareas/t1/tarea-opcional-1-termodinamica/","tags":["I1IIQ1003"]}
---

# Pregunta 1
**Datos para estado 1:**
Pistón:
- $m=100kg$
- $d=2r=150\pu{ cm }$
- $x_{1}=0.4$
- $P_{1}=101kPa$
- $h_{1}=150\pu{ cm }\implies V_{1}=\pi·(0.75\pu{ m})^{2}·1.50\pu{ cm}=2.65 \pu{ m^{3} }$
- $\bar{V}_{1}=\frac{2.65 \pu{ m^{3}}}{m_{a}}$
## Inciso a)
Por regla de la palanca, se sabe que la calidad de la mezcla líquido-vapor sigue la siguiente equivalencia.
$$
x_{1}=0.4=\frac{\frac{2.65m^{3}}{m_{a}}-V_{L}}{V_{V}-V_{L}}
$$
Ahora se puede verificar las tablas a la presión indicada de $100 \ \pu{ kPa}\approx1.014 \ \pu{ Bar}$, llegando a que:
![Pasted image 20250324170133.png|500](/img/user/Cursos/Ingenier%C3%ADa%20Civil/2025-1/Termodin%C3%A1mica/Tareas/T1/attachments/Pasted%20image%2020250324170133.png)
- $V_{V}=1.67 \pu{ \frac{m^{3}}{kg} }$
- $V_{L}=1.04 ·10^{-3} \pu{ \frac{m^{3}}{kg} }$
Con esto ya se tienen los valores necesarios para despejar la masa de agua $m_{a}$.
$$
\begin{align}
0.4 & =\frac{\frac{2.65 \pu{ m^{3}}}{m_{a}}-1.04·10^{-3} \pu{ \frac{m^{3}}{kg} }}{1.67\pu{ \frac{m^{3}}{kg} }-1.04·10^{-3} \pu{ \frac{m^{3}}{kg} }} \\
0.4\left( 1.67\pu{ \frac{m^{3}}{kg} }-1.04·10^{-3} \pu{ \frac{m^{3}}{kg} } \right) & =\frac{2.65 \pu{ m^{3}}}{m_{a}}-1.04·10^{-3} \pu{ \frac{m^{3}}{kg} } \\
0.67 \pu{ \frac{m^{3}}{kg} } & =\frac{2.65 \pu{ m^{3}}}{m_{a}}-1.04·10^{-3} \pu{ \frac{m^{3}}{kg} } \\
0.67\pu{ \frac{m^{3}}{kg} } & =\frac{2.65 \pu{ m^{3}}}{m_{a}} \\
m_{a} & \approx\frac{2.65}{0.67} \pu{ kg}=3.96 \pu{ kg}
\end{align}
$$
## Inciso b
Con lo obtenido en el inciso a, se puede calcular el volumen específico del agua en el estado $1$.
- $\bar{V}_{1}=\frac{2.65\pu{ m^{3}}}{3.96\pu{ kg}}=0.67 \, \pu{ \frac{m^{3}}{kg}}$
### Estado 1
Como ya se vio en la tabla, la temperatura debe ser de $100ºC$ para esta presión en el estado líquido-vapor.
- $P_{1}=100\pu{ kPa}$
- $T_{1}=100ºC$ 
- $V_{1}=2.65\pu{ m^{3}};\bar{V}_{1}=0.67 \, \pu{ \frac{m^{3}}{kg}}$ (ya calculado)
- $U_{1}=?$
Para calcular $U_{1}$, se puede usar la regla de la palanca de la misma forma que se ocupó anteriormente con los siguientes valores de energías internas de la tabla:
- $\bar{U}_{L}=418.94 \, \pu{ \frac{kJ}{kg}}$ 
- $\bar{U}_{V}= 2506.5 \, \pu{ \frac{kJ}{kg}}$ 
$$
\begin{align}
0.4 & =\frac{\bar{U}_{1}-\bar{U}_{L}}{\bar{U}_{V}-\bar{U}_{L}} \\
\bar{U}_{1} & =0.4(\bar{U}_{V}-\bar{U}_{L}) +\bar{U}_{L} \\
\bar{U}_{1} & =0.4 \left( 2506.5 \, \pu{ \frac{kJ}{kg}} -418.94 \, \pu{ \frac{kJ}{kg}}\right) +418.94 \, \pu{ \frac{kJ}{kg}} \\
\bar{U}_{1} & =1253.96 \, \pu{ \frac{kJ}{kg}}
\end{align}
$$
Finalmente, se sabe ahora que,
$$U_{1}=\bar{U}_{1}·m_{a}=1253.96 \, \pu{ \frac{kJ}{kg}}·3.96 \, \pu{ kg}=4965.70$$
### Estado 2
- $h_{2}=150\, \pu{ cm}-45 \, \pu{ cm}=105\, \pu{ cm}$
- $\implies V_{2}=\pi(0.75\, \pu{ m})^{2}·1.05\, \pu{ m}\approx1.86\, \pu{ m^{3}}$
- $\implies \bar{V}_{2}=\frac{1.86 \, \pu{ m^{3}}}{3.96\, \pu{ kg}}=0.47 \, \pu{ \frac{m^{3}}{kg}}$
Como su estado es vapor saturado, se debe buscar el valor respectivo de este volumen específico en la tabla para obtener su temperatura y presión.
A continuación se muestran resaltados los valores entre los que se encuentra la temperatura.
![Pasted image 20250330223401.png](/img/user/Cursos/Ingenier%C3%ADa%20Civil/2025-1/Termodin%C3%A1mica/Tareas/T1/attachments/Pasted%20image%2020250330223401.png)


| $T\, \pu{ ºC}$ | $\bar{V}\, \pu{ \frac{m^{3}}{kg}}$ |
| -------------- | ---------------------------------- |
| $140$          | $0.51$                             |
| $T_{2}$        | $0.47$                             |
| $150$          | $0.39$                             |
Ahora se debe hacer una interpolación:
$$
\begin{align}
T_{2} & =140\, \pu{ ºC}+\frac{0.47\, \pu{ \frac{m^{3}}{kg}}-0.51\, \pu{ \frac{m^{3}}{kg}}}{0.39\, \pu{ \frac{m^{3}}{kg}}-0.51\, \pu{ \frac{m^{3}}{kg}}}(150\, \pu{ ºC}-140\, \pu{ ºC}) \\
T_{2} & =143.33\, \pu{ ºC}
\end{align}
$$
Ahora para la presión:

| $P\, \pu{ bar}$ | $\bar{V} \, \pu{ \frac{m^{3}}{kg}}$ |
| --------------- | ----------------------------------- |
| $3.61$          | $0.51$                              |
| $P_{2}$         | $0.47$                              |
| $4.76$          | $0.39$                              |
$$
\begin{align}
P_{2} & =3.61\, \pu{ bar}+\frac{0.47\, \pu{ \frac{m^{3}}{kg}}-0.51\, \pu{ \frac{m^{3}}{kg}}}{0.39\, \pu{ \frac{m^{3}}{kg}}-0.51\, \pu{ \frac{m^{3}}{kg}}}(4.76\, \pu{ bar}-3.61\, \pu{ bar})  \\
P_{2} & =3.99 \, \pu{ bar}
\end{align}
$$
Ahora se repite el mismo procedimiento para la energía interna específica:

| $\bar{U}\, \pu{ \frac{kJ}{kg}}$ | $\bar{V} \, \pu{ \frac{m^{3}}{kg}}$ |
| ------------------------------- | ----------------------------------- |
| $2550$                          | $0.51$                              |
| $U_{2}$                         | $0.47$                              |
| $2559.5$                        | $0.39$                              |

$$
\begin{align}
\bar{U}_{2} & =2550\, \pu{ \frac{kJ}{kg}}+\frac{0.47\, \pu{ \frac{m^{3}}{kg}}-0.51\, \pu{ \frac{m^{3}}{kg}}}{0.39\, \pu{ \frac{m^{3}}{kg}}-0.51\, \pu{ \frac{m^{3}}{kg}}}\left( 2559.5\, \pu{ \frac{kJ}{kg}}-2550\, \pu{ \frac{kJ}{kg}} \right)  \\
\bar{U}_{2} & =2553.17 \, \pu{ \frac{kJ}{kg}}
\end{align}
$$
Ahora se debe ponderar por la masa:
$$
U_{2}=\bar{U}_{2}·m_{a}=2553.17 \, \pu{ \frac{kJ}{kg}}·3.96\, \pu{ kg}=10110.55 \, \pu{ kJ}
$$
En resumen:
- $V_{2}=1.86\, \pu{ m^{3}}$
- $T_{2}=143.33\, \pu{ ºC}$
- $P_{2}=3.99\, \pu{ bar}$
- $U_{2}=10110.55\, \pu{ kJ}$
### Estado 3
"El sistema se calienta a presión constante (proceso 2-3) hasta que el pistón choque con los topes a una altura de 170 cm."
Como es presión constante:
- $P_{3}=P_{2}=3.99 \, \pu{ bar}$
- $h_{3}=170\, \pu{ cm}$
- $\implies V_{3}=\pi·(0.75\, \pu{ m})^{2}·1.70\, \pu{ m}\approx3.00\, \pu{ m^{3}}$
- $\implies \bar{V}_{3}= \frac{3\, \pu{ m^{3}}}{3.96\, \pu{ kg}}\approx0.76 \, \pu{ \frac{m^{3}}{kg}}$
Ahora para buscar los valores se busca la presión en la tabla. Sin embargo, se nota que el volumen específico $\bar{V}_{3}$ es mayor a los límites que se muestran en la tabla. Esto significa que $x_{3}>0$ y nos encontramos en un vapor sobrecalentado.
![Pasted image 20250401101853.png|600](/img/user/Cursos/Ingenier%C3%ADa%20Civil/2025-1/Termodin%C3%A1mica/Tareas/T1/attachments/Pasted%20image%2020250401101853.png)
Ahora se deben usar tablas de vapor sobrecalentado cercanas a $4\, \pu{ bar}$.
![Pasted image 20250401103614.png|300](/img/user/Cursos/Ingenier%C3%ADa%20Civil/2025-1/Termodin%C3%A1mica/Tareas/T1/attachments/Pasted%20image%2020250401103614.png)
![Tabla 1 editada.png|300](/img/user/Cursos/Ingenier%C3%ADa%20Civil/2025-1/Termodin%C3%A1mica/Tareas/T1/attachments/Tabla%201%20editada.png)
_Nota._ Esta tabla está modificada de la tabla A4 para mostrar los ejes.
![Pasted image 20250401103714.png|300](/img/user/Cursos/Ingenier%C3%ADa%20Civil/2025-1/Termodin%C3%A1mica/Tareas/T1/attachments/Pasted%20image%2020250401103714.png)
Ahora se debe hacer una interpolación doble.
#### Temperatura

| $3 \, \pu{ bar}$ |                                      |     | $5 \, \pu{ bar}$ |                                      |
| ---------------- | ------------------------------------ | --- | ---------------- | ------------------------------------ |
| $T\, [\pu{ ºC}]$ | $\bar{V}\, [\pu{ \frac{m^{3}}{kg}}]$ |     | $T\, [\pu{ ºC}]$ | $\bar{V}\, [\pu{ \frac{m^{3}}{kg}}]$ |
| $200$            | $0.72$                               |     | $500$            | $0.71$                               |
|                  | $0.76$                               |     |                  | $0.76$                               |
| $240$            | $0.78$                               |     | $600$            | $0.80$                               |
Para una interpolación doble, se debe llegar a una tabla intermedia usando las presiones. Se parte interpolando las temperaturas superior e inferior de los límites.

| $T\,[ \pu{ ºC}]$ | $P \, [\pu{ bar}]$ |
| ---------------- | ------------------ |
| $200$            | $3$                |
| $T_{s}$          | $3.99$             |
| $500$            | $5$                |
Ahora, se interpola:
$$
\begin{align}
T_{s} & =200 \, \pu{ ºC}+\frac{3.99 \, \pu{ bar}-3 \,\pu{ bar}}{5\,\pu{ bar}-3\,\pu{ bar}}(500\, \pu{ ºC}-200\, \pu{ ºC}) \\
T_{s} & =348.5 \, \pu{ ºC}
\end{align}
$$
Ahora la temperatura inferior:

| $T\,[ \pu{ ºC}]$ | $P \, [\pu{ bar}]$ |
| ---------------- | ------------------ |
| $240$            | $3$                |
| $T_{i}$          | $3.99$             |
| $600$            | $5$                |
$$
\begin{align}
T_{i} & =240 \, \pu{ ºC}+\frac{3.99 \, \pu{ bar}-3 \,\pu{ bar}}{5\,\pu{ bar}-3\,\pu{ bar}}(600\, \pu{ ºC}-240\, \pu{ ºC}) \\
T_{i} & = 418.2\, \pu{ ºC}
\end{align}
$$
Ahora se interpolan los límites del volumen:

| $\bar{V} \, \pu{ [ \frac{m^{3}}{kg}}]$ | $P \, [\pu{ bar}]$ |
| -------------------------------------- | ------------------ |
| $0.72$                                 | $3$                |
| $\bar{V}_{s}$                          | $3.99$             |
| $0.71$                                 | $5$                |

$$
\begin{align}
\bar{V}_{s} & =0.72 \, \pu{ \frac{m^{3}}{kg}}+\frac{3.99 \, \pu{ bar}-3 \,\pu{ bar}}{5\,\pu{ bar}-3\,\pu{ bar}}(0.71\, \pu{ \frac{m^{3}}{kg}}-0.72 \, \pu{ \frac{m^{3}}{kg}}) \\
\bar{V}_{s} & = 0.72\, \pu{ \frac{m^{3}}{kg}}
\end{align}
$$
Ahora el límite inferior:

| $\bar{V} \, \pu{ [ \frac{m^{3}}{kg}}]$ | $P \, [\pu{ bar}]$ |
| -------------------------------------- | ------------------ |
| $0.78$                                 | $3$                |
| $\bar{V}_{s}$                          | $3.99$             |
| $0.80$                                 | $5$                |

$$
\begin{align}
V_{i} & =0.78  \, \pu{ \frac{m^{3}}{kg}} +\frac{3.99 \, \pu{ bar}-3 \,\pu{ bar}}{5\,\pu{ bar}-3\,\pu{ bar}}(0.80\, \pu{ \frac{m^{3}}{kg}}-0.78 \,\pu{ \frac{m^{3}}{kg}}) \\
V_{i} & = 0.79\, \pu{ \frac{m^{3}}{kg}}
\end{align}
$$

Ahora se puede armar la tabla para $4\, \pu{ bar}$.

| $T\, [\pu{ ºC}]$ | $\bar{V}\, [\pu{ \frac{m^{3}}{kg}}]$ |
| ---------------- | ------------------------------------ |
| $348.50$         | $0.72$                               |
| $T_{3}$          | $0.76$                               |
| $418.20$         | $0.79$                               |
Finalmente, se interpola la temperatura $3$.
$$
\begin{align}
T_{3} & =348.5\, \pu{ ºC}+\frac{0.76 \,\pu{ \frac{m^{3}}{kg}}-0.72\,\pu{ \frac{m^{3}}{kg}}}{0.79\,\pu{ \frac{m^{3}}{kg}}-0.72\,\pu{ \frac{m^{3}}{kg}}}(418\, \pu{ ºC}-348.5\, \pu{ ºC}) \\
T_{3} & =388.21\, \pu{ ºC}
\end{align}
$$
#### Energía interna
Se hace lo mismo de la temperatura, pero con los siguientes datos sacados de la misma tabla:

| $3 \, \pu{ bar}$                     |                                      |     | $5 \, \pu{ bar}$                     |                                      |
| ------------------------------------ | ------------------------------------ | --- | ------------------------------------ | ------------------------------------ |
| $\bar{U} \, [ \pu{ \frac{kJ}{kg}} ]$ | $\bar{V}\, [\pu{ \frac{m^{3}}{kg}}]$ |     | $\bar{U} \, [ \pu{ \frac{kJ}{kg}} ]$ | $\bar{V}\, [\pu{ \frac{m^{3}}{kg}}]$ |
| $2650.7$                             | $0.72$                               |     | $3128.4$                             | $0.71$                               |
|                                      | $0.76$                               |     |                                      | $0.76$                               |
| $2947.3$                             | $0.78$                               |     | $3299.6$                             | $0.80$                               |
Se pueden usar los mismos valores de $\bar{V}_{s}$ y $\bar{V}_{i}$.
Ahora se debe calcular $\bar{U}_{s}$ y $\bar{U}_{i}$.
Para $\bar{U}_{s}$ se usan los valores:

| $T\,[ \pu{ ºC}]$ | $P \, [\pu{ bar}]$ |
| ---------------- | ------------------ |
| $2650.7$         | $3$                |
| $T_{s}$          | $3.99$             |
| $3128.4$         | $5$                |
$$
\begin{align}
\bar{U}_{s} & =2650.7 \, \pu{ \frac{kJ}{kg}}+\frac{3.99 \, \pu{ bar}-3 \,\pu{ bar}}{5\,\pu{ bar}-3\,\pu{ bar}}(3128.4\, \pu{ \frac{kJ}{kg}}-2650.7\, \pu{ \frac{kJ}{kg}}) \\
\bar{U}_{s} & =2887.16 \, \pu{ \frac{kJ}{kg}}
\end{align}
$$
Para el valor de $\bar{U}_{i}$

| $T\,[ \pu{ ºC}]$ | $P \, [\pu{ bar}]$ |
| ---------------- | ------------------ |
| $2947.3$         | $3$                |
| $T_{s}$          | $3.99$             |
| $3299.6$         | $5$                |
$$
\begin{align}
\bar{U}_{i} & =2947.3 \, \pu{ \frac{kJ}{kg}}+\frac{3.99 \, \pu{ bar}-3 \,\pu{ bar}}{5\,\pu{ bar}-3\,\pu{ bar}}(3299.6\, \pu{ \frac{kJ}{kg}}-2947.3\, \pu{ \frac{kJ}{kg}}) \\
\bar{U}_{i} & =3121.69 \, \pu{ \frac{kJ}{kg}}
\end{align}
$$
Ahora, usando los valores ya mencionados y el mismo procedimiento:

| $\bar{U}\, [\pu{ ºC}]$ | $\bar{V}\, [\pu{ \frac{m^{3}}{kg}}]$ |
| ---------------------- | ------------------------------------ |
| $2887.16$              | $0.72$                               |
| $T_{3}$                | $0.76$                               |
| $3121.69$              | $0.79$                               |
$$
\begin{align}
\bar{U}_{3} & =2887.16\, \pu{ \frac{kJ}{kg}}+\frac{0.76 \,\pu{ \frac{m^{3}}{kg}}-0.72\,\pu{ \frac{m^{3}}{kg}}}{0.79\,\pu{ \frac{m^{3}}{kg}}-0.72\,\pu{ \frac{m^{3}}{kg}}}(3121.69\, \pu{ \frac{kJ}{kg}}-2887.16\, \pu{ \frac{kJ}{kg}}) \\
\bar{U}_{3} & =3021.18\, \pu{ \frac{kJ}{kg}}
\end{align}
$$
Ahora se obtiene $U_{3}$:
$U_{3}=\bar{U}_{3}·m_{a}=3021.18 \, \pu{ \frac{kJ}{kg}}·3.96\, \pu{ kg}=11963.87 \, \pu{ kJ}$

En resumen:
- $V_{3}=3.00\, \pu{ m^{3}}$
- $\bar{V}_{3}\approx0.76 \, \pu{ \frac{m^{3}}{kg}}$
- $T_{3}=388.21\, \pu{ ºC}$
- $P_{3}=3.99\, \pu{ bar}$
- $U_{3}=11963.87\, \pu{ kJ}$
### Estado 4
"Luego el calentamiento continúa hasta que la presión llega a 15 bar"
Si la presión aumenta a 15 bar, y el volumen no cambia ya que es un proceso isocórico ("hasta que el pistón choque con los topes"), se pueden buscar los datos en tablas usando el volumen y la presión.
- $\bar{V}_{4}=\bar{V}_{3}=0.76\, \pu{ \frac{m^{3}}{kg}}$ 
- $P_{4}=15\, \pu{ bar}$
![Pasted image 20250402001723.png|600](/img/user/Cursos/Ingenier%C3%ADa%20Civil/2025-1/Termodin%C3%A1mica/Tareas/T1/attachments/Pasted%20image%2020250402001723.png)
Como el volumen $0.76 \, \pu{ \frac{m^{3}}{kg}}$ es mayor al del vapor saturado, se deben usar las tablas de vapor sobrecalentado a $15\, \pu{ bar}$.
![Cursos/Ingeniería Civil/2025-1/Termodinámica/Tareas/T1/attachments/Sin título 1.png](/img/user/Cursos/Ingenier%C3%ADa%20Civil/2025-1/Termodin%C3%A1mica/Tareas/T1/attachments/Sin%20t%C3%ADtulo%201.png) 
*Nota.* Imagen adaptada del libro para mostrar ejes.

Para obtener valores de la temperatura, se debe hacer una extrapolación con las dos últimas filas. Se ocupará la misma formula de la interpolación, pero con valores externos al intervalo.


| $T[ \pu{ ºC}]$ | $\bar{V}  \left[ \pu{\frac{m^{3}}{kg}} \right]$ |
| -------------- | ----------------------------------------------- |
| $600$          | $0.27$                                          |
| $640$          | $0.28$                                          |
| $T_{4}$        | $0.76$                                          |
$$
\begin{align}
T_{4} & =600\, \pu{ ºC}+\frac{0.76 \, \pu{ \frac{m^{3}}{kg}}-0.27\pu{ \frac{m^{3}}{kg}}}{0.28\pu{ \frac{m^{3}}{kg}}-0.27\pu{ \frac{m^{3}}{kg}}}(640\, \pu{ ºC}-600\, \pu{ ºC}) \\
T_{4} & =2560 \, \pu{ ºC}
\end{align}
$$
Se aplica el mismo procedimiento para la energía interna:

| $\bar{U}\left[  \pu{\frac{kj}{kg}} \right]$ | $\bar{V}  \left[ \pu{\frac{m^{3}}{kg}} \right]$ |
| ------------------------------------------- | ----------------------------------------------- |
| $3293.9$                                    | $0.27$                                          |
| $3364.8$                                    | $0.28$                                          |
| $T_{4}$                                     | $0.76$                                          |
$$
\begin{align}
\bar{U}_{4} & =3293.9\, \pu{\frac{kJ}{kg}}+\frac{0.76 \, \pu{ \frac{m^{3}}{kg}}-0.27\pu{ \frac{m^{3}}{kg}}}{0.28\pu{ \frac{m^{3}}{kg}}-0.27\pu{ \frac{m^{3}}{kg}}}(3364.8\, \pu{\frac{kJ}{kg}}-3293.9\, \pu{\frac{kJ}{kg}}) \\
\bar{U}_{4} & =6768.00  \, \pu{\frac{kJ}{kg}}
\end{align}
$$
Ponderado por $m_{a}$: 
$$
\bar{U}_{4}·m_{a}=U_{4}=6768.00 \, \pu{ \frac{kJ}{kg}}·3.96\, \pu{ kg}=26801.28 \, \pu{ kJ}
$$
En resumen:
- $V_{4}=3.00\, \pu{ m^{3}}$
- $\bar{V}_{4}\approx0.76 \, \pu{ \frac{m^{3}}{kg}}$
- $T_{4}=2560\, \pu{ ºC}$
- $P_{4}=15\, \pu{ bar}$
- $U_{4}=26801.28\, \pu{ kJ}$
## Inciso c)
![Pasted image 20250402021400.png|400](/img/user/Cursos/Ingenier%C3%ADa%20Civil/2025-1/Termodin%C3%A1mica/Tareas/T1/attachments/Pasted%20image%2020250402021400.png)
## Inciso d)
Es posible encontrar la cantidad de arena en el piston, ya que hay una etapa donde este se encuentra en equilibrio de presiones y el enunciado entrega la masa del pistón. Esta etapa es la Etapa 2 y se encuentra a $3.99\, \pu{ bar}$.
El área de la sección transversal del piston es $\pi r^{2}=\pi·(0.75\, \pu{ m})^{2}\approx1.77\, \pu{ m^{2}}$.
Con esto, se tiene que:
Se aproxima la presión atmosférica a $1.01\, \pu{bar}$
$$
\begin{align}
P_{2}=\frac{F}{A}+atm & =9.8 \, \pu{ \frac{m}{s^{2}}}·\frac{(m_{\text{piston}}+m_{\text{arena}})}{1.77 \, \pu{ m^{2}}}+1.01\, \pu{ bar} \\
\frac{3.99\, \pu{ bar}-1.01 \, \pu{ bar}}{9.8\, \pu{ \frac{m}{s^{2}}}} ·1.77\, \pu{ m^{2}}&=m_{\text{piston}}+m_{\text{arena}}  \\
(399\, \pu{ kPa}-101 \, \pu{ kPa}) ·0.18\, \pu{ m·s^{2}}&=100\, \pu{ kg}+m_{\text{arena}}  \\
298\, \pu{ kPa} ·0.18\, \pu{ m·s^{2}}-100\, \pu{ kg}&=m_{\text{arena}}  \\
298 \, \pu{ \frac{kN}{m^{\cancel{ 2 }}}}·0.18\, \pu{ \cancel{ m }}·\, \pu{s^{2}}-100\, \pu{ kg } & =m_{\text{arena}} \\
298000 \, \pu{ \frac{1}{\cancel{ m }} }\, \pu{ \frac{\cancel{ m }·kg}{\cancel{ s^{2} }}}·0.18\, \pu{ \cancel{ s^{2} }}-100\, \pu{ kg } & =m_{\text{arena}} \\
53540\, \pu{ kg}=53.54\, \pu{ t} & =m_{\text{arena}}
\end{align}
$$

En conclusión, se añadieron $53.54$ toneladas de arena al pistón.
# Ejercicio 2
Un sistema que consiste en 0.9 kg de de agua experimenta un ciclo de potencia compuesto por los siguientes procesos.
## Estado 2
No se puede caracterizar inmediatamente el estado 1, pero se usará el proceso 4-1 para hacerlo.
Calentamiento a presión constante a $10 \, \pu{ bar}$ hasta alcanzar vapor saturado
Como el proceso sucede hasta alcanzar la fase de vapor saturado. Para obtener el valor de $\bar{V}_{1}$ se debe buscar en la tabla el volumen de vapor saturado a esta presión.
![Pasted image 20250402181751.png|500](/img/user/Cursos/Ingenier%C3%ADa%20Civil/2025-1/Termodin%C3%A1mica/Tareas/T1/attachments/Pasted%20image%2020250402181751.png)
Como se aprecia en la línea destacada, se tiene un valor de:
- $T_{2}=180\, \pu{ ºC}$
- $\bar{V}_{2}=0.19\, \pu{ \frac{m^{3}}{kg}}$
- $\implies V_{2}=0.19\, \pu{ \frac{m^{3}}{kg}}·0.9\, \pu{ kg}=0.17\, \pu{ m^{3}}$
- Fase: Vapor saturado
- $\bar{U}_{2}=2583.7 \, \pu{ \frac{kJ}{kg}}$
- $\implies U_{2}=2583.7\, \pu{ \frac{kJ}{kg}}·0.9\, \pu{ kg}=2325.33 \, \pu{ kJ}$
- $\bar{h}_{2}=2778.2 \, \pu{ \frac{kJ}{kg}}$
- $\implies h_{2}=2778.2 \, \pu{ \frac{kJ}{kg}}·0.9\, \pu{ kg}=2500.38\, \pu{ kJ}$
## Proceso 2-3 y estado 3
Enfriamiento a volumen constante hasta $P_{3}=5\, \pu{ bar}$.
Se sabe que $\bar{V}_{3}=\bar{V}_{2}=0.19 \, \pu{ \frac{m^{3}}{kg}}$ ya que es isocórico.
Ahora se debe buscar el valor de presión en la tabla de presión.
![Pasted image 20250402183628.png|500](/img/user/Cursos/Ingenier%C3%ADa%20Civil/2025-1/Termodin%C3%A1mica/Tareas/T1/attachments/Pasted%20image%2020250402183628.png)
Para obtener todos los valores se puede usar la calidad.
$$
\begin{align}
x_{3} & =\frac{0.19\, \pu{ \frac{m^{3}}{kg}}-1.09·10^{-3}\, \pu{ \frac{m^{3}}{kg}}}{0.37\, \pu{ \frac{m^{3}}{kg}}-1.09·10^{-3}\, \pu{ \frac{m^{3}}{kg}}} \\
x_{3} & =0.51
\end{align}
$$
La regla de la palanca permite usar la calidad obtenida para resolver otras variables.
$$
\begin{align}
x_{3} & =\frac{\bar{U}_{3}-\bar{U}_{L}}{\bar{U}_{V}-\bar{U}_{L}} \\
 \bar{U}_{3} & =\bar{U}_{L }+x_{3}(\bar{U}_{V}-\bar{U}_{L}) \\
\bar{U}_{3} & =639.68 \, \pu{ \frac{kJ}{kg}}+0.51(2561.2\, \pu{ \frac{kJ}{kg}}-639.68\, \pu{ \frac{kJ}{kg}}) \\
\bar{U}_{3} & =1619.65\, \pu{ \frac{kJ}{kg}}
\end{align}
$$
Ahora para la entalpía:
$$
\begin{align}
\bar{h}_{3} & =\bar{h}_{L}+x_{3}(\bar{h}_{V}-\bar{h}_{L}) \\
\bar{h}_{3} &=640.23 \, \pu{ \frac{kJ}{kg}} +0.51(2748.7\, \pu{ \frac{kJ}{kg}}-640.23\, \pu{ \frac{kJ}{kg}}) \\
\bar{h}_{3} & =1725.55\, \pu{ \frac{kJ}{kg}}
\end{align}
$$
Finalmente, en resumen:
- $P_{3}=5\, \pu{ bar}$
- $T_{3}=151.9\, \pu{ ºC}$
- $\bar{V}_{3}=0.19\, \pu{ \frac{m^{3}}{kg}}$
- $\implies V_{3}=0.19\, \pu{ \frac{m^{3}}{kg}}·0.9\, \pu{ kg}=0.17\, \pu{ m^{3}}$
- Fase: Mezcla líquido vapor
- $\bar{U}_{3}=1619.65 \, \pu{ \frac{kJ}{kg}}$
- $\implies U_{3}=1619.65 \, \pu{ \frac{kJ}{kg}}·0.9\, \pu{ kg}=1457.68\, \pu{ kJ}$
- $\bar{h}_{3}=1725.55 \, \pu{ \frac{kJ}{kg}}$
- $\implies h_{3}=1725.55\, \pu{ \frac{kJ}{kg}}·0.9\, \pu{ kg}=1552.99\, \pu{ kJ}$
En lo que respecta al calor, se tiene: 
$$
\begin{align}
\Delta U_{23} & =U_{3}-U_{2} \\
 & =1457.68 \, \pu{kJ}-2325.33\, \pu{kJ} \\
 & =-867.65\, \pu{ kJ}
\end{align}
$$
Además, ya que el proceso es isocórico (no hay cambio de volumen $\implies$ no hay trabajo)
$$
\Delta U_{23}=Q_{23}+\cancelto{ 0 }{ W_{23} }
$$
Finalmente, se tiene:
- $Q_{23}=-867.65\, \pu{ kJ}$
## Proceso 3-4; estado 4
Compresión isotérmica con $Q_{34} = -600 \, \pu{ kJ}$.
Se dice que le proceso es isotérmico, entonces $T_{3}=T_{4}=151.9\, \pu{ ºC}$. Mientras el proceso se mantenga dentro de la fase líquido-vapor, la temperatura fija a la presión, entonces $P_{3}=5\, \pu{ bar}$.
Además, se sabe que en procesos isobáricos:
$$
\begin{align}
\Delta h_{34} & =h_{4}-h_{3}=Q_{34} \\
 h_{4}-1552.99\, \pu{ kJ}& =-600 \, \pu{ kJ} \\
h_{4} & =1552.99\, \pu{ kJ}-600\, \pu{ kJ}  \\
h_{4} & = 952.99 \, \pu{ kJ}
\end{align}
$$
De aquí:
- $\overline{h}_{4}=\frac{952.99\,\pu{ kJ}}{0.9\, \pu{ kg}}=1058.88 \, \pu{ \frac{kJ}{kg}}$
Como se mantiene a la misma presión y temperatura, lo único que cambia es la calidad. Se debe usar la misma tabla.
![Pasted image 20250402183628.png|500](/img/user/Cursos/Ingenier%C3%ADa%20Civil/2025-1/Termodin%C3%A1mica/Tareas/T1/attachments/Pasted%20image%2020250402183628.png)
Sabiendo la entalpía, se puede calcular la nueva calidad del sistema.:
$$
\begin{align}
x_{4} & =\frac{\overline{h}_{4}-\overline{h}_{L}}{\overline{h}_{V}-\overline{h}_{L}} \\
 & =\frac{1058.88 \, \pu{ \frac{kJ}{kg}}\, \pu{ kJ} - 640.23\, \pu{ \frac{kJ}{kg}}}{2748.7\, \pu{ \frac{kJ}{kg}}-640.23\, \pu{ \frac{kJ}{kg}}} \\
x_{4} & \approx 0.20 \end{align}
$$
Con este valor se pueden despejar las demás funciones de estado. De la regla de la palanca se tiene que:
$$
\begin{align}
\bar{U}_{4} & =\bar{U}_{L}+x_{4}(\bar{U}_{V}-\bar{U}_{L}) \\
 &= 639.68 \, \pu{ \frac{kJ}{kg}}+0.2(2561.2\pu{ \frac{kJ}{kg}}-639.68\pu{ \frac{kJ}{kg}}) \\
 & =1023.98\pu{ \frac{kJ}{kg}}
\end{align}
$$
$$
\begin{align}
\bar{V}_{4} & =\bar{V}_{L}+x_{4}(\bar{V}_{V}-\bar{V}_{L}) \\
 &= 1.09 · 10^{-3} \, \pu{ \frac{m^3}{kg}}+0.2(0.37\pu{ \frac{m^3}{kg}}-1.09 · 10^{-3}\pu{ \frac{m^3}{kg}}) \\
 & = 0.075 \pu{ \frac{m^3}{kg}}
\end{align}
$$
Finalmente:
- $T_{4}=151.9\, \pu{ ºC}$
- $\bar{V}_{2}=0.075\, \pu{ \frac{m^{3}}{kg}}$
- $\implies V_{2}=0.075\, \pu{ \frac{m^{3}}{kg}}·0.9\, \pu{ kg}=0.0675\, \pu{ m^{3}}$
- Fase: Mezcla liquido vapor
- $\bar{U}_{2}=1472.23 \, \pu{ \frac{kJ}{kg}}$
- $\implies U_{2}=1472.23\, \pu{ \frac{kJ}{kg}}·0.9\, \pu{ kg}=1325.01 \, \pu{ kJ}$
- $\bar{h}_{2}=1549.05 \, \pu{ \frac{kJ}{kg}}$
- $\implies h_{2}=1549.05 \, \pu{ \frac{kJ}{kg}}·0.9\, \pu{ kg}=1394.15\, \pu{ kJ}$

## Proceso 4-1; estado 1
"Calentamiento a volumen constante hasta volver al estado 1"
Esto dice que el estado 1 tiene un volumen:
- $\bar{V}_{1}=\bar{V}_{4}=0.075 \, \pu{ \frac{m^{3}}{kg}}$
Del proceso 1-2:
- $P_{1}=P_{2}=10\, \pu{ bar}$
Con estas dos variables ya se puede caracterizar todo el sistema usando la tabla para $10\, \pu{ bar}$.
![Pasted image 20250402231500.png|600](/img/user/Cursos/Ingenier%C3%ADa%20Civil/2025-1/Termodin%C3%A1mica/Tareas/T1/attachments/Pasted%20image%2020250402231500.png)
Calculando la calidad:
$$
\begin{align}
x_{1} & =\frac{\bar{V}_{1}-\bar{V}_{L}}{\bar{V}_{V}-\bar{V}_{L}} \\
 & =\frac{0.075 \, \pu{ \frac{m^{3}}{kg}}-1.13·10^{-3}}{0.19\, \pu{ \frac{m^{3}}{kg}}-1.13·10^{-3}} \\x_{1}
 & =0.39
\end{align}
$$
Ahora, para la energía interna:
$$
\begin{align}
\bar{U}_{1} & = \bar{U}_{L}+x_{1}(\bar{U}_{V}-\bar{U}_{L}) \\
 & =761.68 \, \pu{ \frac{kJ}{kg}}+0.39(2583.6\, \pu{ \frac{kJ}{kg}}-761.68\, \pu{ \frac{kJ}{kg}}) \\
 & =1472.23\, \pu{ \frac{kJ}{kg}}
\end{align}
$$
Para la entalpía
$$
\begin{align}
\bar{h}_{1} & = \bar{h}_{L}+x_{1}(\bar{h}_{V}-\bar{h}_{L}) \\
 & =762.81 \, \pu{ \frac{kJ}{kg}}+0.39(2778.1\, \pu{ \frac{kJ}{kg}}-762.81\, \pu{ \frac{kJ}{kg}}) \\
 & =1549.05\, \pu{ \frac{kJ}{kg}}
\end{align}
$$

Finalmente:
- $T_{2}=179.9\, \pu{ ºC}$
- $\bar{V}_{2}=0.075\, \pu{ \frac{m^{3}}{kg}}$
- $\implies V_{2}=0.075\, \pu{ \frac{m^{3}}{kg}}·0.9\, \pu{ kg}=0.0675\, \pu{ m^{3}}$
- Fase: Mezcla líquido vapor
- $\bar{U}_{2}=1472.23 \, \pu{ \frac{kJ}{kg}}$
- $\implies U_{2}=1472.23\, \pu{ \frac{kJ}{kg}}·0.9\, \pu{ kg}=1325.01 \, \pu{ kJ}$
- $\bar{h}_{2}=1549.05 \, \pu{ \frac{kJ}{kg}}$
- $\implies h_{2}=1549.05 \, \pu{ \frac{kJ}{kg}}·0.9\, \pu{ kg}=1394.15\, \pu{ kJ}$
## Gráficos
![Pasted image 20250402234056.png](/img/user/Cursos/Ingenier%C3%ADa%20Civil/2025-1/Termodin%C3%A1mica/Tareas/T1/attachments/Pasted%20image%2020250402234056.png)
![Pasted image 20250402234312.png](/img/user/Cursos/Ingenier%C3%ADa%20Civil/2025-1/Termodin%C3%A1mica/Tareas/T1/attachments/Pasted%20image%2020250402234312.png)