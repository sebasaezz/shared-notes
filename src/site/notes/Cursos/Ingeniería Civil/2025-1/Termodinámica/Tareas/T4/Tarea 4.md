---
{"dg-publish":true,"permalink":"/cursos/ingenieria-civil/2025-1/termodinamica/tareas/t4/tarea-4/","tags":["I2IIQ1003"]}
---

# Pregunta 1

> [!quote] Enunciado
> Se tiene una combinación de ciclos de Carnot como se muestran en la siguiente figura:
> ![Pasted image 20250514211440.png|350](/img/user/Cursos/Ingenier%C3%ADa%20Civil/2025-1/Termodin%C3%A1mica/Tareas/T4/attachments/Pasted%20image%2020250514211440.png)
> Del diagrama anterior se conocen los datos mostrados en la tabla de a continuación:
> 
> | Nº                                                          |       1 |       2 | 3      | 4      |       5 |
> | :-----------------------------------------------------------: | ------: | ------: | -----: | -----: | ------: |
> | $T_{\text{c}}\, \pu{ [K]}$        |         |   263.3 | 499.2  |        |   297.3 |
> | $T_{\text{h}} \, \pu{ [K]}$       |   477.0 |         | 519.8  | 455.3  |   501.8 |
> | $\dot{Q}_{\text{c}}\,  \left[\pu{ \frac{kJ}{s}} \right]$    |  -1427.9 |   -728.7 |        | -1553.6 |         |
> | $\dot{Q}_{\text{h}}\,  \left[\pu{ \frac{kJ}{s}} \right]$    |         |  1463.0 | 1222.2 | 1612.7 |  -2889.1 |
> | $\dot{W}_{\text{in}}\, \left[ \pu{ \frac{kJ}{s}} \right]$   | ------- | ------- | 1106.5 | 146.9  |         |
> | $\dot{W}_{\text{out}}\, \left[  \pu{ \frac{kJ}{s}} \right]$ |         |         |        |        | ------- |
> 
> Encuentre los datos que faltan y los valores de $\alpha$ y $\beta$.

Hay que obtener ecuaciones para cada uno de los ciclos, para así resolver el sistema completo. La variable más crucial a analizar es $\dot{W}_{\text{neto}}$, ya que establece conexiones entre los sistemas.

Las ecuaciones más útiles en este contexto son:

$$
W_{\text{neto}}=-Q_{\text{h}}-Q_{\text{c}}=-Q_{\text{h}}\left( 1- \frac{T_{\text{c}}}{T_{\text{h}}} \right) =-Q_{\text{c}}\left( \frac{T_{\text{c}}}{T_{\text{h}}}-1 \right)\tag{1}
$$

Además, como en los sistemas a veces entra un trabajo externo $W_{\text{in}}$, se va a tener que:

$$
W_{\text{neto}}=W_{\text{out}}+W_{\text{in}}\tag{2}
$$

En esta ecuación se debe considerar los signos del trabajo, 

Así como también es importante que:

$$
\Delta S=-\frac{Q_{\text{h}}}{T_{\text{h}}}-\frac{Q_{\text{c}}}{T_{\text{c}}}=0 \tag{3}
$$
## Ciclo 2

Para el ciclo 2, se tienen las suficientes variables para despejar $\dot{W}_{\text{out},2}$.

$$
\begin{align}
\dot{W}_{\text{neto},2}=\dot{W}_{\text{out},2} & =-\dot{Q}_{\text{c}}-\dot{Q}_{\text{h}} \\
 & =728.7 \, \pu{ \frac{kJ}{s}}-1463.0 \, \pu{ \frac{kJ}{s}} \\
 \dot{W}_{\text{out},2}& =-734.3 \, \pu{ \frac{kJ}{s}}
\end{align}
$$

Ahora para la temperatura del foco caliente se despeja la ecuación 3:

$$
\begin{align}
-\frac{\dot{Q}_{\text{h},2}}{T_{\text{h},2}}-\frac{\dot{Q}_{\text{c},2}}{T_{\text{c},2}} & =0 \\
-\frac{\dot{Q}_{\text{h},2}}{T_{\text{h},2}} & =\frac{\dot{Q}_{\text{c},2}}{T_{\text{c},2}} \\
T_{\text{h},2} & =-\frac{\dot{Q}_{\text{h},2}·T_{\text{c},2}}{\dot{Q}_{\text{c},2}} \\
 & =-\frac{ 1463\, \cancel{ \pu{ \frac{kJ}{s}} }·263.3\, \pu{ K}}{-728.8\, \cancel{ \pu{ \frac{kJ}{s}}} } \\
T_{\text{h},2} & =528.62\, \pu{ K}
\end{align}
$$
## Ciclo 4

Pero la imagen muestra que $\dot{W}_{\text{in},4}=-(1-\alpha)\dot{W}_{\text{out},2}$ . Se toma negativo ya que estos valores son de los otros sistemas donde representan variables de salida (negativas).

$$
\begin{align}
\dot{W}_{\text{out},4}-(1-\alpha)\dot{W}_{\text{out},2} & =-\dot{Q}_{\text{c},4}-\dot{Q}_{\text{h},4} \\
\dot{W}_{\text{out},4} & =1553.6\, \pu{ \frac{kJ}{s}} -1612.7\, \pu{ \frac{kJ}{s}}+(1-\alpha)\left( -734.3\, \pu{ \frac{kJ}{s}} \right) \\
\dot{W}_{\text{out},4} & =-793.4\, \pu{ \frac{kJ}{s}}+\alpha 734.3\, \pu{ \frac{kJ}{s}}
\end{align}
$$

Pero ahora se nota que según el enunciado, $\dot{W}_{\text{in},4}=146.9 \, \pu{ \frac{kJ}{s}}$. Entonces:

$$
\begin{align}
\dot{W}_{\text{in},4} & =-(1-\alpha)\dot{W}_{\text{out},2} \\
\dot{W}_{\text{in},4}+\dot{W}_{\text{out},2} & =\alpha \dot{W}_{\text{out},2} \\
\alpha & =\frac{\dot{W}_{\text{in},4}+\dot{W}_{\text{out},2}}{\dot{W}_{\text{out},2}} \\
 & =\frac{146.9\, \cancel{ \pu{ \frac{kJ}{s}} }+\left( -734.3\, \cancel{ \pu{ \frac{kJ}{s}} } \right)}{-734.3\, \cancel{ \pu{ \frac{kJ}{s}} }} \\
 \alpha& =0.8
\end{align}
$$
Reemplazando para despejar $\dot{W}_{\text{out},4}$:
$$
\begin{align}
\dot{W}_{\text{out},4} & =-793.4 \, \pu{ \frac{kJ}{s}}+0.8·734.3 \, \pu{ \frac{kJ}{s}}\\
 & =-205.96 \, \pu{ \frac{kJ}{s}}
\end{align}
$$

Para calcular $T_{\text{c},4}$, se va a usar la ecuación 1:
$$
\begin{align}
\dot{W}_{\text{neto},4}  =\dot{W}_{\text{in},4}+\dot{W}_{\text{out,4}} &=-\dot{Q}_{\text{h},4}\left( 1-\frac{T_{\text{c},4}}{T_{\text{h},4}} \right) \\
 T_{\text{c},4} & =\left( \frac{\dot{W}_{\text{in},4}+\dot{W}_{\text{out},4}}{\dot{Q}_{\text{h},4}}+1 \right)T_{\text{h},4}  \\
 & =\left( \frac{146.9\, \cancel{ \pu{ \frac{kJ}{s}} }-205.96\, \cancel{ \pu{ \frac{kJ}{s}} }}{1612.7\, \cancel{ \pu{ \frac{kJ}{s}}} } +1\right)·455.3\, \pu{ K} \\
T_{\text{c},4} & \approx 438.63\, \pu{ K}
\end{align}
$$
## Ciclo 3

Para el ciclo 3, se tienen las suficientes variables para obtener todas las incógnitas. Se debe considerar al trabajo neto de la siguiente forma:

$$
\begin{align}
\dot{W}_{\text{neto},3} & =\dot{W}_{\text{out},3}+\dot{W}_{\text{in},3}
\end{align}
$$

Pero $\dot{W}_{\text{in},3}=-(\dot{W}_{\text{out},1}+\alpha \dot{W}_{\text{out},2})$ según el enunciado..

$$
\begin{align}
W_{\text{out},3}-\dot{W}_{\text{out},1}-\alpha\dot{W}_{\text{out},2}& = -\dot{Q}_{\text{h},3}\left( 1-\frac{T_{\text{c},3}}{T_{\text{h},3}} \right) \\
 \dot{W}_{\text{out},3}& = 
- 1222.2\, \pu{ \frac{kJ}{s}} \left( 1-\frac{499.2\, \pu{ K}}{519.8\, \pu{ K}} \right)
+\alpha \dot{W}_{\text{out},2} +\dot{W}_{\text{out},1}
 \\
 \dot{W}_{\text{out},3}& =-48.4366\, \pu{ \frac{kJ}{s}}+0.8·\left( - 734.3\, \pu{ \frac{kJ}{s}} \right) +\dot{W}_{\text{out},1} \\
 & =-635.8766\, \pu{ \frac{kJ}{s}}+\dot{W}_{\text{out},1}
\end{align}
$$

Además, según el enunciado, se sabe que $\dot{W}_{\text{in},3}=1106.5\, \pu{ \frac{kJ}{s}}$. Entonces se puede despejar $\dot{W}_{\text{out},1}$:
$$
\begin{align}
\dot{W}_{\text{in},3} & =1106.5\, \pu{ \frac{kJ}{s}} \\
-(\dot{W}_{\text{out},1}+\alpha \dot{W}_{\text{out},2}) & =1106.5\, \pu{ \frac{kJ}{s}}  \\
\dot{W}_{\text{out},1} & =-1106.5\, \pu{ \frac{kJ}{s}}-\alpha \dot{W}_{\text{out},2} \\
 & =-1106.5\, \pu{ \frac{kJ}{s}}-0.8·\left( -734.3\, \pu{ \frac{kJ}{s}} \right) \\
\dot{W}_{\text{out},1} & =-519.06 \, \pu{ \frac{kJ}{s}}
\end{align}
$$

Reemplazando en lo obtenido para $\dot{W}_{\text{out},3}$:
$$
\begin{align}
\dot{W}_{\text{out},3} & = -635.8766\, \pu{ \frac{kJ}{s}} +(-519.06\, \pu{ \frac{kJ}{s}} ) \\
 \dot{W}_{\text{out},3}&= -  1154.9366 \, \pu{ \frac{kJ}{s}}   
\end{align}
$$
Para calcular $\dot{Q}_{\text{c},3}$, se va a usar la ecuación 3:
$$
\begin{align}
0 & =-\frac{Q_{\text{h},3}}{T_{\text{h},3}}-\frac{Q_{\text{c},3}}{T_{\text{c},3}}  \\
Q_{\text{c},3} & =-\frac{Q_{\text{h},3}}{T_{\text{h},3}}T_{\text{c},3} \\ 
 & =- \frac{1222.2 \, \pu{ \frac{kJ}{s}}}{519.8\,\cancel{  \pu{ K} }}·499.2\, \cancel{ \pu{ K} }
\\
 Q_{\text{c},3}& \approx -  1173.76 \, \pu{ \frac{kJ}{s}}
\end{align}
$$
## Ciclo 5

El ciclo 5 es diferente a los demás, ya que en la imagen se ve que tiene las flechas invertidas. Esto significa que rechaza calor al reservorio caliente como un refrigerador. Por esto se cambio el signo en la tabla.
Se aplica lo mismo, con $\dot{W}_{\text{in},5}=-(\dot{W}_{\text{out},3}+\beta \dot{W}_{\text{out},4})$. Además, como no sale una flecha del ciclo, y la celda está en negro, se asume que $\dot{W}_{\text{out},5}=0$.

$$
\begin{align}
\dot{W}_{\text{out},5}& =-Q_{\text{h}}\left( 1-\frac{T_{\text{c}}}{T_{\text{h}}} \right)+\dot{W}_{\text{out},3}+\beta \dot{W}_{\text{out},4}  \\
 0& =2889.1\, \pu{ \frac{kJ}{s}}\left( 1-\frac{297.3\, \pu{ K}}{501.8\, \pu{ K}} \right)+\dot{W}_{\text{out},3}+\beta \dot{W}_{\text{out},4} \\
 &  =1177.403\, \pu{ \frac{kJ}{s}}-  1154.9366 \, \pu{ \frac{kJ}{s}} +\beta \left(-205.96 \, \pu{ \frac{kJ}{s}}\right) \\
0 & = 22.4664 \, \pu{ \frac{kJ}{s}}-\beta·205.96\, \pu{ \frac{kJ}{s}} \\
\beta & =\frac{-22.6446 \, \pu{ \frac{kJ}{s} }}{-205.96 \, \pu{ \frac{kJ}{s}}}= 0.102 
\end{align}
$$
Ahora se calcula $\dot{W}_{\text{in},5}$ con lo que ya se dijo:
$$
\begin{align}
\dot{W}_{\text{in},5} & =-(\dot{W}_{\text{out},3}+\beta \dot{W}_{\text{out},4}) \\
 & -\left( -  1154.9366 \, \pu{ \frac{kJ}{s}}  -0.102·205.96 \, \pu{ \frac{kJ}{s}} \right) \\
 \dot{W}_{\text{in},5}& \approx 1175.94 \, \pu{ \frac{kJ}{s}}
\end{align}
$$
El calor transferido $\dot{Q}_{\text{c},5}$ se calcula con la ecuación 3:
$$
\begin{align}
0 & =-\frac{Q_{\text{h}}}{T_{\text{h}}}-\frac{Q_{\text{c}}}{T_{\text{c}}} \\
 \dot{Q}_{\text{c},5}& =-\frac{\dot{Q}_{\text{h},5}}{T_{\text{h},5}}T_{\text{c},5} \\
 & = -\frac{-2889.1 \, \pu{ \frac{kJ}{s}}}{501.8\, \pu{ K}} ·297.3\, \pu{ K} \\
\dot{Q}_{\text{c},5} & \approx 1711.7 \, \pu{ \frac{kJ}{s}}
\end{align}
$$
## Ciclo 1
Ahora se puede terminar con las variables del ciclo 1 ya que se conoce $\dot{W}_{\text{out,1}}=-519.06 \, \pu{ \frac{kJ}{s}}=\dot{W}_{\text{neto},1}$. Aplicando la ecuación 1:
$$
\begin{align}
\dot{W}_{\text{neto},1} & =-\dot{Q}_{\text{c},1}\left(  \frac{T_{\text{c},1}}{T_{\text{h},1}}-1 \right) \\
T_{\text{c},1} & =\left( -\frac{\dot{W}_{\text{neto},1}}{\dot{Q}_{\text{c},1}}+1 \right)T_{\text{h},1} \\
 & =\left( -\frac{-519.06 \, \pu{ \frac{kJ}{s}}}{-1427.9\, \pu{ \frac{kJ}{s}}} +1\right)·477.0\, \pu{ K} \\
 T_{\text{c},1}&\approx 303.60\, \pu{ K}
\end{align}
$$
Finalmente, se usa la ecuación 3 para obtener $\dot{Q}_{\text{h},1}$.
$$
\begin{align}
0 & =-\frac{Q_{\text{h},1}}{T_{\text{h},1}}-\frac{Q_{\text{c},1}}{T_{\text{c},1}} \\
Q_{\text{h},1} & =-\frac{Q_{\text{c},1}}{T_{\text{c},1}}T_{\text{h},1} \\
 & =-\frac{-1427.9 \, \pu{ \frac{kJ}{s}}}{303.60\, \pu{ K}}·477.0\, \pu{ K} \\
\dot{Q}_{\text{h},1} & \approx 2243.44\, \pu{ \frac{kJ}{s}}
\end{align}
$$
## Tabla final
Finalmente, se obtuvo un valor de $\alpha=0.8$ y $\beta=0.102$. Los valores de las demás variables son:

|                             Nº                              |       1 |       2 |        3 |       4 |       5 |
| :---------------------------------------------------------: | ------: | ------: | -------: | ------: | ------: |
|                 $T_{\text{c}}\, \pu{ [K]}$                  |  303.60 |   263.3 |    499.2 |  438.63 |   297.3 |
|                 $T_{\text{h}} \, \pu{ [K]}$                 |   477.0 |  528.62 |    519.8 |   455.3 |   501.8 |
|  $\dot{Q}_{\text{c}}\,  \left[\pu{ \frac{kJ}{s}} \right]$   | -1427.9 |  -728.7 | -1173.76 | -1553.6 |  1711.7 |
|  $\dot{Q}_{\text{h}}\,  \left[\pu{ \frac{kJ}{s}} \right]$   | 2243.44 |  1463.0 |   1222.2 |  1612.7 | -2889.1 |
|  $\dot{W}_{\text{in}}\, \left[ \pu{ \frac{kJ}{s}} \right]$  | ------- | ------- |   1106.5 |   146.9 | 1175.94 |
| $\dot{W}_{\text{out}}\, \left[  \pu{ \frac{kJ}{s}} \right]$ | -519.06 |  -734.3 | -1154.94 | -205.96 | ------- |

# Problema 2

> [!quote]
> Considere el proceso de la Figura 1. En este, $1000 \, \pu{\frac{kg}{h}}$ de agua como líquido saturado a $0.1 \, \pu{ bar}$ entra a una bomba con $85 \%$ de eficiencia, que sube la presión hasta $150 \, \pu{ bar}$. Luego pasa a una caldera donde se calienta hasta $480\, \pu{ ºC}$. Posteriormente el flujo se expande hasta $1 \, \pu{ bar}$ en una turbina con $75 \%$ de eficiencia. Luego el flujo entra a un primer separador flash. La corriente 7 que sale por el fondo pasa a una válvula para luego ingresar a un segundo separador flash que opera a $0.06 \, \pu{ bar}$. El flujo 10, que sale por el tope, entra a un intercambiador de calor donde se calienta hasta $90\, \pu{ ºC}$. Por otro lado, el flujo 5 entra al mismo intercambiador de calor para salir como la corriente 6. Finalmente, se mezcla el flujo 11 con una corriente de $15 \, \pu{ \frac{kg}{h}}$ con $20 \%$ de calidad. En base a esto determine:
![Pasted image 20250523193934.png|400](/img/user/Cursos/Ingenier%C3%ADa%20Civil/2025-1/Termodin%C3%A1mica/Tareas/T4/attachments/Pasted%20image%2020250523193934.png)

## Inciso a)

> [!quote]
> Determine las presiones, entalpías específicas y flujo másico en kg/h de todas las corrientes.

Se va a armar una tabla con los datos del enunciado y conversiones para facilitar:

| Flujo | $P \, \pu{ [bar]}$ | $h\,  \left[\pu{ \frac{kJ}{kg}}\right]$ | $\dot{m}\, \left[ \pu{ \frac{kg}{h}} \right]$ | $\dot{m}\, \left[  \pu{\frac{kg}{s}} \right]$ | $x$ | Est. | $T\, \pu{ ºC}$ |
| ----- | -----------------: | --------------------------------------: | --------------------------------------------: | --------------------------------------------: | --: | ---: | -------------: |
| 1     |                0.1 |                                         |                                          1000 |                                         60000 |   0 |  LST |                |
| 2     |                150 |                                         |                                               |                                               |     |      |                |
| 3     |                    |                                         |                                               |                                               |     |      |            480 |
| 4     |                  1 |                                         |                                               |                                               |     |      |                |
| 5     |                    |                                         |                                               |                                               |   1 |  VST |                |
| 6     |                    |                                         |                                               |                                               |     |      |                |
| 7     |                    |                                         |                                               |                                               |   0 |  LST |                |
| 8     |               0.06 |                                         |                                               |                                               |     |      |                |
| 9     |                    |                                         |                                               |                                               |   0 |  LST |                |
| 10    |                    |                                         |                                               |                                               |   1 |  VST |                |
| 11    |                    |                                         |                                               |                                               |     |      |             90 |
| 12    |                    |                                         |                                            15 |                                               |  20 |  L-V |                |
| 13    |                    |                                         |                                               |                                               |     |      |                |
### Análisis de presiones
Se analizan los procesos que no inducen cambio de presión o es negligible, estos son el intercambiador de calor, caldera y los separadores flash. De esto se concluye que $P_{3}=150\, \pu{ bar}$. Las corrientes que siguen de 4 están a $1\, \pu{ bar}$ y no cambian de no ser por las que vienen después de la válvula que quedan en $0.06\, \pu{ bar}$.
- $P_{4}=P_{5}=P_{6}=P_{7}=1\, \pu{ bar}$
- $P_{8}=P_{9}=P_{10}=P_{11}=0.06\, \pu{ bar}$
el mezclador adiabático también funciona isobáricamente en todas sus direcciones, entonces $P_{12}=P_{13}=0.06\, \pu{ bar}$.
### Flujo 1
De la tabla A-3, se revisa la fila de $0.1\, \pu{ bar}$ para concluir que:
- $T_{1}=45.81\, \pu{ ºC}$
- $s_{1}=0.6493\, \pu{ \frac{kJ}{kg·K}}$
- $h_{1}=191.83\, \pu{ \frac{kJ}{kg}}$
### Flujo 2
Del balance de masa:
$$
\dot{m}_{1}=-\dot{m}_{2}
$$
_Nota:_ esto es interpretando como flujo negativo a salir de la máquina
Primero se analiza la situación donde $\eta=100\%$ o que $\dot{S}_{\text{gen}}=0$.
Para encontrar $h_{2}$ se debe buscar en tablas un valor a $150\, \pu{ bar}$ que tenga la misma entropía.
![Pasted image 20250524202250.png|400](/img/user/Cursos/Ingenier%C3%ADa%20Civil/2025-1/Termodin%C3%A1mica/Tareas/T4/attachments/Pasted%20image%2020250524202250.png)
![Pasted image 20250524202302.png|400](/img/user/Cursos/Ingenier%C3%ADa%20Civil/2025-1/Termodin%C3%A1mica/Tareas/T4/attachments/Pasted%20image%2020250524202302.png)
Hay que interpolar con respecto a la entropía:

| $s\,\left[ \pu{\frac{kJ}{kg·K}}  \right]$ | $h\,  \left[\pu{ \frac{kJ}{kg}}\right]$ |
| ----------------------------------------: | --------------------------------------: |
|                                    0.5666 |                                  180.78 |
|                                    0.6493 |                               $h_{2}^*$ |
|                                    1.0656 |                                  346.81 |
Interpolando:
$$
\begin{align}
h_{2}^* & \approx \frac{0.6493\, \pu{ \frac{kJ}{kg·K}}-1.0656\, \pu{ \frac{kJ}{kg·K}}}{0.5666\, \pu{ \frac{kJ}{kg·K}}-1.0656\, \pu{ \frac{kJ}{kg·K}}}\left( 180.78\, \pu{ \frac{kJ}{kg}}-346.81\pu{ \frac{kJ}{kg}} \right)+346.81\pu{ \frac{kJ}{kg}}
 \\ & \approx 208.30\pu{ \frac{kJ}{kg}}
\end{align}
$$
Haciendo el balance de energía, se llega a que:
$$
\begin{align}
\cancelto{ 0 }{ \frac{ \mathrm{d}U }{ \mathrm{d}t }  } & =\sum_{k=1}^{2}\dot{m}_{k}h_{k}+\cancelto{ 0 }{ \dot{W} }+ \dot{W}_{\text{s}} +\cancelto{ 0 }{ \dot{Q} }
 \\
0 & =\dot{m}_{1}h_{1}+\dot{m}_{2}h_{2}+\dot{W}_{\text{s}} \\
 \dot{W}_{\text{s}}& =\dot{m}_{1}(h_{2}-h_{1})
\end{align}
$$
Esto es tanto para el caso ideal como con eficiencia, y se sabe que para una bomba:
$$
\begin{align}
\eta_{12} & =\frac{\dot{W}^*_{\text{s}}}{\dot{W}_{\text{s}}} \\
 \eta_{12}& =\frac{\cancel{ \dot{m} }(h_{2}^*-h_{1})}{\cancel{ \dot{m} }(h_{2}-h_{1})} \\
h_{2} & =\frac{h_{2}^*-h_{1}}{\eta_{12}}+h_{1} \\
  & =\frac{208.30\, \pu{ \frac{kJ}{kg}}-191.83\, \pu{ \frac{kJ}{kg}}}{85\%}+191.83\, \pu{ \frac{kJ}{kg}} \\
h_{2} & = 211.21 \, \pu{ \frac{kJ}{kg}}
\end{align}
$$
Para calcular la entropía, se interpola en la misma tabla:

| $h\, \left[ \pu{ \frac{kJ}{kg}} \right]$ | $s \, \left[ \pu{ \frac{kJ}{kg·K}} \right]$ |
| ---------------------------------------- | ------------------------------------------- |
| 180.78                                   | 0.5666                                      |
| 211.21                                   | $s_{2}$                                     |
| 346.81                                   | 1.0656                                      |
$$
\begin{align}
s_{2} & \approx \frac{211.21 \, \pu{ \frac{kJ}{kg}}-346.81\, \pu{ \frac{kJ}{kg}}}{180.78\, \pu{ \frac{kJ}{kg}}-346.81\, \pu{ \frac{kJ}{kg}}}\left( 0.5666 -1.0656 \right)\, \pu{ \frac{kJ}{kg·K}}+1.0656\, \pu{ \frac{kJ}{kg·K}} \\
s_{2} & \approx 0.6581\, \pu{ \frac{kJ}{kg·K}} 
\end{align}
$$
Se hace lo mismo con la temperatura:

| $h\, \left[ \pu{ \frac{kJ}{kg}} \right]$ | $T\, [\pu{ ºC}]$ |
| ---------------------------------------- | ---------------- |
| 180.78                                   | 40               |
| 211.21                                   | $T_{2}$          |
| 346.81                                   | 80               |
$$
\begin{align}
T_{2} & \approx \frac{211.21 \, \pu{ \frac{kJ}{kg}}-346.81\, \pu{ \frac{kJ}{kg}}}{180.78\, \pu{ \frac{kJ}{kg}}-346.81\, \pu{ \frac{kJ}{kg}}}(40-80)\, \pu{ ºC}+80\, \pu{ ºC} \\
T_{2} & \approx 47.33 \, \pu{ ºC}
\end{align}
$$
### Flujo 3
Se tiene una caldera que sube la temperatura a $480\, \pu{ ºC}$. El balance de masa es:
$$
\dot{m}_{2}=-\dot{m}_{3}
$$
Se puede obtener $h_{3}$ buscando en la tabla A-4 a $150\, \pu{ bar}$ los $480\, \pu{ ºC}$. Se tiene una interpolación:

| $P \, [\pu{ Pa}]$ | $h\,  \left[\pu{ \frac{kJ}{kg}}\right]$ |
| ----------------: | --------------------------------------: |
|               140 |                                  3264.5 |
|               150 |                                 $h_{3}$ |
|               160 |                                  3234.4 |
$$
\begin{align}
h_{3} & \approx \frac{150\, \pu{ ºC}-160\, \pu{ ºC}}{140\, \pu{ ºC}-160\, \pu{ ºC}}\left( 3264.5\, \pu{ \frac{kJ}{kg}}-3234.4\, \pu{ \frac{kJ}{kg}} \right)+3234.4\, \pu{ \frac{kJ}{kg}} \\
h_{3} & \approx  3249.45 \, \pu{ \frac{kJ}{kg}}
\end{align}
$$
La entropía será útil, y se calcula de la misma forma:

| $P \, [\pu{ Pa}]$ | $s\,  \left[\pu{ \frac{kJ}{kg·K}}\right]$ |
| ----------------: | ----------------------------------------: |
|               140 |                                    6.3143 |
|               150 |                                   $s_{3}$ |
|               160 |                                    6.2215 |

$$
\begin{align}
s_{3} & \approx \frac{150\, \pu{ ºC}-160\, \pu{ ºC}}{140\, \pu{ ºC}-160\, \pu{ ºC}}\left( 6.3143\, \pu{ \frac{kJ}{kg·K}}-6.2215\, \pu{ \frac{kJ}{kg·K}} \right)+6.2215\, \pu{ \frac{kJ}{kg·K}} \\
s_{3} & \approx  6.2679 \, \pu{ \frac{kJ}{kg·K}}
\end{align}
$$
### Flujo 4 
Al igual que el 2, se calcula para isoentrópico, con $\eta_{34}=100\%$. Se busca en la tabla A-3 la entropía $s_{3}$ a $1\, \pu{ bar}$ y se concluye que está en L-V. Se calcula la calidad:
$$
\begin{align}
x_{4^*} & =\frac{s_{4}^*-s_{\text{l}}^{1\, \pu{ bar}}}{s_{\text{g}}^{1\, \pu{ bar}}-s_{\text{l}}^{1\, \pu{ bar}}} \\
 & =\frac{6.2679 \, \pu{ \frac{kJ}{kg·K}}-1.3026\, \pu{ \frac{kJ}{kg·K}}}{7.3594\, \pu{ \frac{kJ}{kg·K}}-1.3026\, \pu{ \frac{kJ}{kg·K}}} \\
x_{4^*} & = 81.98\% 
\end{align}
$$
Ahora se usa la regla de la palanca:
$$
\begin{align}
x_{4^{*}} & =\frac{h_{4}^*-h_{\text{l}}^{1\, \pu{ bar}}}{h_{\text{g}}^{1\, \pu{ bar}}-h_{\text{l}}^{1\, \pu{ bar}}} \\
 h_{4}^*& =x_{4^*}(h_{\text{g}}^{1\, \pu{ bar}}-h_{\text{l}}^{1\, \pu{ bar}})+h_{\text{l}}^{1\, \pu{ bar}} \\
 & =81.98\%·\left( 2675.5\, \pu{ \frac{kJ}{kg}}-417.46\, \pu{ \frac{kJ}{kg}} \right)+417.46\, \pu{ \frac{kJ}{kg}} \\
h_{4}^* & =  2268.60\, \pu{ \frac{kJ}{kg}}  
\end{align}
$$
Para una turbina, se tiene el siguiente balance de masa y energía:
$$
m_{3}=-m_{4}
$$
$$
\begin{align}
\cancelto{ 0 }{ \frac{ \mathrm{d}U }{ \mathrm{d}t }  } & =\sum_{k=3}^{4}\dot{m}_{k}h_{k}+\cancelto{ 0 }{ \dot{W}+\dot{Q} }+\dot{W}_{\text{s}} \\
0 & =\dot{m}_{3}h_{3}+\dot{m}_{4}h_{4} +\dot{W}_{\text{s}}\\
\dot{W}_{\text{s}} & =\dot{m}_{3}(h_{4}-h_{3})
\end{align}
$$
Nuevamente este balance no depende de la entropía, entonces, como:
$$
\begin{align}
\eta_{34} & =\frac{\dot{W}}{\dot{W}_{\text{s}}^*} \\
  \eta_{34} & =\frac{\cancel{ \dot{m}_{3} }(h_{4}-h_{3})}{\cancel{ \dot{m}_{3} }(h_{4}^*-h_{3})} \\
h_{4} & =\eta_{34}(h_{4}^*-h_{3})+h_{3} \\
  h_{4} & =75\%\left( 2268.60\, \pu{ \frac{kJ}{kg}}  -3249.45 \, \pu{ \frac{kJ}{kg}} \right)+3249.45 \, \pu{ \frac{kJ}{kg}} \\
h_{4} & = 2513.81\, \pu{ \frac{kJ}{kg}} 
\end{align}
$$
Calculando nuevamente la calidad:
$$
\begin{align}
x_{4} & =\frac{h_{4}-h_{\text{l}}^{1\, \pu{ bar}}}{h_{\text{g}}^{1\, \pu{ bar}}-h_{\text{l}}^{1\, \pu{ bar}}}  \\
 & =\frac{2513.81\, \pu{ \frac{kJ}{kg}}-417.46\, \pu{ \frac{kJ}{kg}} }{2675.5\, \pu{ \frac{kJ}{kg}}-417.46\, \pu{ \frac{kJ}{kg}}} \\
x_{4} & =92.84\%
\end{align}
$$
Ahora se usa la calidad para calcular la entropía:
$$
\begin{align}
x_{4} & =\frac{s_{4}-s_{\text{l}}^{1\, \pu{ bar}}}{s_{\text{g}}^{1\, \pu{ bar}}-s_{\text{l}}^{1\, \pu{ bar}}} \\
s_{4} & =x_{4}(s_{\text{g}}^{1\, \pu{ bar}}-s_{\text{l}}^{1\, \pu{ bar}})+s_{\text{l}}^{1\, \pu{ bar}} \\
 & =92.84\%(7.3594-1.3026)\, \pu{ \frac{kJ}{kg·K}}+1.3026\, \pu{ \frac{kJ}{kg·K}} \\
s_{4} & = 6.9257 \, \pu{ \frac{kJ}{kg·K}}
\end{align}
$$
Finalmente, la temperatura está en la tabla.
$$
T_{4}=99.63\, \pu{ ºC}
$$
### Flujo 5
Este flujo es el vapor separado del líquido en un separador flash. Se puede calcular el flujo de vapor saturado simplemente ponderando el flujo másico por la calidad (cantidad de vapor):
$$
\begin{align}
\dot{m}_{5} & =x_{4}·\dot{m}_{4} \\
 &= 92.84\%·1000\, \pu{ \frac{kg}{h}} \\
 \dot{m}_{5}&=928.4\, \pu{ \frac{kg}{h}} 
\end{align}
$$
Las propiedades como presión y temperatura se mantienen, mientas que loas otras propiedades son las del vapor saturado a $1\, \pu{ bar}$.
$$
\begin{align}
h_{5} & =2675.5\, \pu{ \frac{kJ}{kg}}, & s_{5} & =7.3594\, \pu{ \frac{kJ}{kg·K}}
\end{align}
$$
### Flujo 7
Lo mismo del flujo 5, pero con líquido saturado.
$$
\begin{align}
\dot{m}_{7} & =(1-x_{4})·\dot{m}_{4} \\
 & =(1-92.84\%)·1000\, \pu{ \frac{kg}{h}} \\
 \dot{m}_{7}& =71.6\, \pu{ \frac{kg}{h}} 
\end{align}
$$
Los valores de líquido saturado a $1\, \pu{ bar}$ son:
$$
\begin{align}
h_{7} & =417.46\, \pu{ \frac{kJ}{kg}}, & s_{7} & =1.3026\, \pu{ \frac{kJ}{kg·K}}
\end{align}
$$
### Flujo 8
Se tiene una válvula que baja la presión a $0.06\, \pu{ bar}$. Se sabe que las válvulas son isoentálpicas, por lo que:
$$
h_{8}=h_{7}=417.46\, \pu{ \frac{kJ}{kg}}
$$
Ahora se puede calcular la nueva calidad usando valores de vapor y liquido saturado de la tabla A-3 a $0.06\, \pu{ bar}$:
$$
\begin{align}
x_{8} & =\frac{h_{8}-h_{\text{l}}^{0.06\, \pu{ bar}}}{h_{\text{g}}^{0.06\, \pu{ bar}}-h_{\text{l}}^{0.06\, \pu{ bar}}} \\
 & =\frac{417.46\, \pu{ \frac{kJ}{kg}}-151.53\, \pu{ \frac{kJ}{kg}}}{2567.4\, \pu{ \frac{kJ}{kg}}-151.53\, \pu{ \frac{kJ}{kg}}} \\
x_{8} & =11.01\%
\end{align}
$$
Con esto se puede calcular la entropía:
$$
\begin{align}
x_{8} & =\frac{s_{8}-s_{\text{l}}^{0.06\, \pu{ bar}}}{s_{\text{g}}^{0.06\, \pu{ bar}}-s_{\text{l}}^{0.06\, \pu{ bar}}} \\
 s_{8}& =x_{8}(s_{\text{g}}^{0.06\, \pu{ bar}}-s_{\text{l}}^{0.06\, \pu{ bar}})+s_{\text{l}}^{0.06\, \pu{ bar}}  \\
 & =11.01\%\left( 8.3304\, \pu{ \frac{kJ}{kg·K}}-0.5210\, \pu{ \frac{kJ}{kg·K}} \right)+0.5210 \, \pu{ \frac{kJ}{kg·K}} \\
s_{8} & = 1.3808\, \pu{ \frac{kJ}{kg·K}} 
\end{align}
$$
La temperatura de la tabla es:
$$
T_{8}=36.16\, \pu{ ºC}
$$
Además, el flujo es el mismo, $\dot{m}_{8}=\dot{m}_{7}=71.6 \, \pu{ \frac{kg}{h}}$
### Flujo 9
Nuevamente un separador flash, entonces se pondera por la calidad:
$$
\begin{align}
\dot{m}_{9} & =(1-x_{8})·\dot{m}_{8} \\
 & =(1-11.01\%)·71.6 \, \pu{ \frac{kg}{h}} \\
\dot{m}_{9} & = 63.7168\, \pu{ \frac{kg}{h}} 
\end{align}
$$
La temperatura y la presión se deben mantener constantes, entonces se usa la misma fila de la tabla para el liquido saturado.
$$
\begin{align}
h_{9} & =151.53\, \pu{ \frac{kJ}{kg}}, & s_{9} & =0.5210\, \pu{ \frac{kJ}{kg·K}}
\end{align}
$$
### Flujo 10
Esta es la parte del vapor del mismo separador flash. Se hace lo mismo:
$$
\begin{align}
\dot{m}_{10} & =x_{8}·\dot{m}_{8} \\
 & =11.01\%·71.6 \, \pu{ \frac{kg}{h}} \\
\dot{m}_{10} & =  7.8832 \, \pu{ \frac{kg}{h}} 
\end{align}
$$
Mirando la tabla para los valores de VST:
$$
\begin{align}
h_{10} & =2567.4\, \pu{ \frac{kJ}{kg}}, & s_{10} & =8.3304\, \pu{ \frac{kJ}{kg·K}}
\end{align}
$$
### Flujo 11
En este flujo, la presión se mantiene constante o con cambio negligible y la temperatura sube a $90\, \pu{ ºC}$. Se tenía VST, entonces ahora se va a tener vapor sobrecalentado (VSC).
Se va a tener que interpolar

| $T\, [\pu{ ºC}]$ | $h\, \left[ \pu{ \frac{kJ}{kg}} \right]$ |
| ---------------: | ---------------------------------------: |
|               80 |                                   2650.1 |
|               90 |                                 $h_{11}$ |
|              120 |                                   2726.0 |
$$
\begin{align}
h_{11} & \approx \frac{90\, \pu{ ºC}-120\, \pu{ ºC}}{80\, \pu{ ºC}-120\, \pu{ ºC}}\left( 2650.1\, \pu{ \frac{kJ}{kg}}-2726.0\, \pu{ \frac{kJ}{kg}} \right)+2726.0\, \pu{ \frac{kJ}{kg}} \\
h_{11} & \approx 2669.1\, \pu{ \frac{kJ}{kg}} 
\end{align}
$$
Ahora se calcula la entropía de la misma forma:

| $T\, [\pu{ ºC}]$ | $s\, \left[ \pu{ \frac{kJ}{kg}} \right]$ |
| ---------------: | ---------------------------------------: |
|               80 |                                   8.5804 |
|               90 |                                 $s_{11}$ |
|              120 |                                   8.7840 |
$$
\begin{align}
s_{11} & \approx \frac{90\, \pu{ ºC}-120\, \pu{ ºC}}{80\, \pu{ ºC}-120\, \pu{ ºC}}\left( 8.5804\, \pu{ \frac{kJ}{kg·K}}-8.7840\, \pu{ \frac{kJ}{kg·K}} \right)+8.7840\, \pu{ \frac{kJ}{kg·K}} \\
s_{11} & \approx 8.6313 \, \pu{ \frac{kJ}{kg·K}} 
\end{align}
$$
### Flujo 6
Ahora que se tiene el flujo 11, se puede calcular el 6 en el intercambiador.
Considerando el siguiente balance de masa:
$$
\begin{align}
\dot{m}_{5} & =-\dot{m}_{6}, & \dot{m}_{10}=-\dot{m}_{11}
\end{align}
$$
Se hace el balance de energía:
$$
\begin{align}
\cancelto{ 0 }{ \frac{ \mathrm{d}U }{ \mathrm{d}t }  } & =\sum_{k=5}^{6}\dot{m}_{k}h_{k}+\sum_{k=10}^{11}\dot{m}_{k}h_{k}+\cancelto{ 0 }{ \dot{W}+\dot{W}_{\text{s}}+\dot{Q} } \\
0 & =\dot{m}_{5}h_{5}+\dot{m}_{6}h_{6}+\dot{m}_{10}h_{10}+\dot{m}_{11}h_{11} \\
\dot{m}_{5}(h_{6}-h_{5}) & =\dot{m}_{10}(h_{10}-h_{11}) \\
h_{6} & =\frac{\dot{m}_{10}}{\dot{m}_{5}}(h_{10}-h_{11})+h_{5}
\end{align}
$$
Reemplazando con los valores conocidos:
$$
\begin{align}
h_{6} & =\frac{7.8832 \, \cancel{ \pu{ \frac{kg}{h}} }}{928.4\, \cancel{ \pu{ \frac{kg}{h}}} }\left( 2567.4\, \pu{ \frac{kJ}{kg}}-2669.1 \, \pu{ \frac{kJ}{kg}}\right)+2675.50\, \pu{ \frac{kJ}{kg}} \\
h_{6} & =  2674.64 \, \pu{ \frac{kJ}{kg}}
\end{align}
$$
Ahora se calcula la calidad de este flujo usando los valores de la tabla a $1\, \pu{ bar}$.
$$
\begin{align}
x_{6} & =\frac{h_{6}-h_{\text{l}}^{1\, \pu{ bar}}}{h_{\text{g}}^{1\, \pu{ bar}}-h_{\text{l}}^{1\, \pu{ bar}}}  \\
 & =\frac{2674.64 \, \pu{ \frac{kJ}{kg}}-417.46\, \pu{ \frac{kJ}{kg}}}{2675.5\, \pu{ \frac{kJ}{kg}}-417.46\, \pu{ \frac{kJ}{kg}}} \\
x_{6} & =99.96\%
\end{align}
$$
Ahora se calcula la entropía con la calidad:
$$
\begin{align}
x_{6} & =\frac{s_{6}-s_{\text{l}}^{1\, \pu{ bar}}}{s_{\text{g}}^{1\, \pu{ bar}}-s_{\text{l}}^{1\, \pu{ bar}}} \\
s_{6} & =x_{6}(s_{\text{g}}^{1\, \pu{ bar}}-s_{\text{l}}^{1\, \pu{ bar}})+s_{\text{l}}^{1\, \pu{ bar}}  \\
 & =99.96\%(7.3594-1.3026)\, \pu{ \frac{kJ}{kg·K}}+1.3026\, \pu{ \frac{kJ}{kg·K}} \\
s_{6} & =7.3570\, \pu{ \frac{kJ}{kg·K}}
\end{align}
$$
### Flujo 12
Se tiene un flujo con $x_{12}=20\%$ a $0.06\, \pu{ bar}$. Los valores se calculan simplemente usando la regla de la palanca:
$$
\begin{align}
x_{12} & =\frac{h_{12}-h_{\text{l}}^{0.06\, \pu{ bar}}}{h_{\text{g}}^{0.06\, \pu{ bar}}-h_{\text{l}}^{0.06\, \pu{ bar}}}  \\
h_{12} & =x_{12}(h_{\text{g}}^{0.06\, \pu{ bar}}-h_{\text{l}}^{0.06\, \pu{ bar}})+h_{\text{l}}^{0.06\, \pu{ bar}} \\
 & =20\%\left( 2567.4\, \pu{ \frac{kJ}{kg}}-151.53\, \pu{ \frac{kJ}{kg}} \right)+151.53\, \pu{ \frac{kJ}{kg}}  \\
h_{12} & = 634.70\, \pu{ \frac{kJ}{kg}}
\end{align}
$$
Ahora se usa lo mismo para calcular la entropía:
$$
\begin{align}
x_{12} & =\frac{s_{12}-s_{\text{l}}^{0.06\, \pu{ bar}}}{s_{\text{g}}^{0.06\, \pu{ bar}}-s_{\text{l}}^{0.06\, \pu{ bar}}}  \\
s_{12} & =x_{12}(s_{\text{g}}^{0.06\, \pu{ bar}}-s_{\text{l}}^{0.06\, \pu{ bar}})+s_{\text{l}}^{0.06\, \pu{ bar}}  \\
 & =20\%(8.3304-0.5210)\, \pu{ \frac{kJ}{kg·K}}+0.5210\, \pu{ \frac{kJ}{kg·K}} \\
s_{12} & = 2.0829\, \pu{ \frac{kJ}{kg·K}} 
\end{align}
$$
La temperatura se ve en la tabla, $T_{12}=36.16\, \pu{ ºC}$
### Flujo 13
Se tiene el siguiente balance de masas:
$$
\begin{align}
\dot{m}_{11}+\dot{m}_{12}+\dot{m}_{13} & =0 \\
\dot{m}_{13} & =-(\dot{m}_{11}+\dot{m}_{12}) \\
\dot{m}_{13} &  =-\left( 7.8832\, \pu{ \frac{kg}{h}}+15\, \pu{ \frac{kg}{h}} \right) \\
\dot{m}_{13} & = -22.8832 \, \pu{ \frac{kg}{h}} 
\end{align}
$$
_Nota:_ nuevamente el signo es solo para el balance con respecto a la máquina

Se hace el balance de energía:
$$
\begin{align}
\cancelto{ 0 }{ \frac{ \mathrm{d}U }{ \mathrm{d}t }  } & =\sum_{k=11}^{13}\dot{m}_{k}h_{k}+\cancelto{ 0 }{ \dot{W}+\dot{W}_{\text{s}}+\dot{Q} } \\
0 & =\dot{m}_{11}h_{11}+\dot{m}_{12}h_{12}+\dot{m}_{13}h_{13} \\
h_{13} & =\frac{\dot{m}_{11}h_{11}+\dot{m}_{12}h_{12}}{-\dot{m}_{13}} \\
 h_{13}& =\frac{7.8832\, \cancel{ \pu{ \frac{kg}{h}} }·2669.1\, \pu{ \frac{kJ}{kg}}+15\, \cancel{ \pu{ \frac{kg}{h}} }·634.70\, \pu{ \frac{kJ}{kg}}}{22.8832\, \cancel{ \pu{ \frac{kg}{h}}} } \\
h_{13} & = 1335.55\, \pu{ \frac{kJ}{kg}}
\end{align}
$$
Se nota que este valor se encuentra en mezcla líquido vapor, entonces se calcula la calidad:
$$
\begin{align}
x_{13} & =\frac{h_{13}-h_{\text{l}}^{0.06\, \pu{ bar}}}{h_{\text{g}}^{0.06\, \pu{ bar}}-h_{\text{l}}^{0.06\, \pu{ bar}}}  \\
 & =\frac{1335.55 \, \pu{ \frac{kJ}{kg}}-151.53\, \pu{ \frac{kJ}{kg}}}{2567.4\, \pu{ \frac{kJ}{kg}}-151.53\, \pu{ \frac{kJ}{kg}}} \\
x_{13} & =  49.01\% 
\end{align}
$$
Con esto se calcula la entropía:
$$
\begin{align}
x_{12} & =\frac{s_{12}-s_{\text{l}}^{0.06\, \pu{ bar}}}{s_{\text{g}}^{0.06\, \pu{ bar}}-s_{\text{l}}^{0.06\, \pu{ bar}}}  \\
s_{12} & =x_{12}(s_{\text{g}}^{0.06\, \pu{ bar}}-s_{\text{l}}^{0.06\, \pu{ bar}})+s_{\text{l}}^{0.06\, \pu{ bar}}  \\
 & =49.01\%(8.3304-0.5210)\, \pu{ \frac{kJ}{kg·K}}+0.5210\, \pu{ \frac{kJ}{kg·K}} \\
s_{12} & = 4.3484 \, \pu{ \frac{kJ}{kg·K}}
\end{align}
$$
Por último la temperatura es la misma ya que está dentro de la campana.
$$
T_{13}=36.16\, \pu{ ºC}
$$
### Tabla final
Se muestra la tabla final mostrando con un * los procesos idealizados como isoentrópicos.

| Flujo         | $P \, \pu{ [bar]}$ | $h\,  \left[\pu{ \frac{kJ}{kg}}\right]$ | $\dot{m}\, \left[ \pu{ \frac{kg}{h}} \right]$ | $s\,\left[ \pu{\frac{kJ}{kg·K}}  \right]$ |  $x\%$ | Est. | $T\, [\pu{ ºC}]$ |
| ------------- | -----------------: | --------------------------------------: | --------------------------------------------: | ----------------------------------------: | -----: | ---: | ---------------: |
| 1             |               0.10 |                                  191.83 |                                       1000.00 |                                    0.6493 |   0.00 |  LST |            45.81 |
| 2$^*_{100\%}$ |             150.00 |                                  208.30 |                                       1000.00 |                                    0.6493 |    --- |  LSE |              --- |
| 2$_{85\%}$    |             150.00 |                                  211.21 |                                       1000.00 |                                    0.6581 |    --- |  LSE |            47.33 |
| 3             |             150.00 |                                 3249.45 |                                       1000.00 |                                    6.2679 |    --- |  VSC |           480.00 |
| 4$^*_{100\%}$ |               1.00 |                                 2268.60 |                                       1000.00 |                                    6.2679 |  81.98 |  L-V |            99.63 |
| 4$_{75\%}$    |               1.00 |                                 2513.81 |                                       1000.00 |                                    6.9257 |  92.84 |  L-V |            99.63 |
| 5             |               1.00 |                                 2675.50 |                                        928.40 |                                    7.3594 | 100.00 |  VST |            99.63 |
| 6             |               1.00 |                                 2674.64 |                                        928.40 |                                    7.3570 |  99.96 |  L-V |            99.63 |
| 7             |               1.00 |                                  417.46 |                                         71.60 |                                    1.3026 |   0.00 |  LST |            99.63 |
| 8             |               0.06 |                                  417.46 |                                         71.60 |                                    1.3808 |  11.01 |  L-V |            36.16 |
| 9             |               0.06 |                                  151.53 |                                         63.72 |                                    0.5210 |   0.00 |  LST |            36.16 |
| 10            |               0.06 |                                  2567.4 |                                          7.88 |                                    8.3304 | 100.00 |  VST |            36.16 |
| 11            |               0.06 |                                  2669.1 |                                          7.88 |                                    8.6313 |    --- |  VSC |            90.00 |
| 12            |               0.06 |                                  634.70 |                                         15.00 |                                    2.0829 |  20.00 |  L-V |            36.16 |
| 13            |               0.06 |                                 1335.55 |                                         22.88 |                                    4.3484 |  49.01 |  L-V |            36.16 |
## Inciso b)

> [!quote]
> La potencia de la turbina, de la bomba, la potencia neta del proceso y el calor agregado en la caldera en kW.

### Turbina
Para calcular la potencia de la turbina, se toma el balance de energía ya hecho:
$$
\begin{align}
\dot{W}_{\text{s, t}} & =\dot{m}_{3}(h_{4}-h_{3}) \\
 & =1000 \, \pu{ \frac{\cancel{ kg }}{\cancel{ h }}}· \frac{1\, \cancel{ \pu{ h} }}{3600\, \pu{ s}}·(2513.81-3249.45)\, \pu{ \frac{kJ}{\cancel{ kg }}} \\
 \dot{W}_{\text{s, t}} & = -  204.3444 \, \pu{ kW}
\end{align}
$$
Este trabajo es negativo por que sale de la turbina.
### Bomba
Nuevamente, se usa el mismo balance de energía:
$$
\begin{align}
 \dot{W}_{\text{s, b}}& =\dot{m}_{1}(h_{2}-h_{1}) \\
 &= 1000 \, \pu{ \frac{\cancel{ kg }}{\cancel{ h }}} \frac{1\, \cancel{ \pu{ h} }}{3600\, \pu{ s}} · \left( 211.21 -191.83\right)\, \pu{ \frac{kJ}{\cancel{ kg }}} \\
\dot{W}_{\text{s, b}} & = 5.3833 \, \pu{ kW}
\end{align}
$$
### Potencia neta
La potencia neta sería entonces sumar los dos valores obtenidos:
$$
\begin{align}
\dot{W}_{\text{net}} & =\dot{W}_{\text{s, t}}+\dot{W}_{\text{s, b}} \\
 & =-  204.3444\, \pu{ kW} +5.3833\, \pu{ kW} \\
\dot{W}_{\text{net}} & =-198.9611\, \pu{ kW}
\end{align}
$$
### Calor agregado a la caldera
Para el calor de la caldera, se debe hacer un balance de energía:
$$
\begin{align}
\cancelto{ 0 }{ \frac{ \mathrm{d}U }{ \mathrm{d}t }  } & =\sum_{k=2}^{3}\dot{m}_{k}h_{k}+\dot{Q}+\cancelto{ 0 }{ \dot{W}+\dot{W}_{\text{s}} } \\
\dot{Q}_{\text{in}} & =\dot{m}_{2}(h_{3}-h_{2}) \\
 & =1000 \, \pu{ \frac{\cancel{ kg }}{\cancel{ h }}} \frac{1\, \cancel{ \pu{ h} }}{3600\, \pu{ s}} ·(3249.45-211.21)\, \pu{ \frac{kJ}{\cancel{ kg }}} \\
 \dot{Q}_{\text{in}} & =843.9556\, \pu{ kW}
\end{align}
$$
## Inciso c)

> [!quote]
> La eficiencia térmica de este proceso.

La eficiencia térmica de un proceso como este se calcula de la siguiente forma:
$$
\begin{align}
\eta  & = \frac{\lvert \dot{W}_{\text{neto}} \rvert }{\dot{Q}_{\text{in}}} \\
 & = \frac{198.9611\, \pu{ kW}}{843.9556\, \pu{ kW}} \\
 \eta& =23.57\%
\end{align}
$$
### Inciso d)

> [!quote]
> Realice un diagrama T-S del proceso

![grafico etiquetado.jpg](/img/user/Cursos/Ingenier%C3%ADa%20Civil/2025-1/Termodin%C3%A1mica/Tareas/T4/grafico%20etiquetado.jpg)