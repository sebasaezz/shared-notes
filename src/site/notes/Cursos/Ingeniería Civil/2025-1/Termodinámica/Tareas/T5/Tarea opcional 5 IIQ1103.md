---
{"dg-publish":true,"permalink":"/cursos/ingenieria-civil/2025-1/termodinamica/tareas/t5/tarea-opcional-5-iiq-1103/"}
---

# Pregunta 1

> [!quote]
> Como parte de un programa nacional de salud en zonas rurales de difícil acceso, un equipo médico se desplaza a distintas comunidades utilizando vehículos equipados con tubos de óxido nitroso ($N_{2}O$), un gas ampliamente utilizado como anestésico en procedimientos menores.
> 
> Estos tubos, de $150\, \pu{ L}$ de volumen interno, permiten llevar atención de urgencia a pacientes en localidades donde no existen centros hospitalarios. Durante el verano, se notaron altas temperaturas en las zonas de ayuda y se midió que la máxima presión interna que alcanzaban los cilindros era de $50 \, \pu{ bar}$. Para garantizar la seguridad durante el traslado se estableció que la temperatura del gas no debe superar el límite técnico de $45\, \pu{ ºC}$.
> 
> Determine la masa de óxido nitroso, en kilogramos, que puede contener cada tubo cuando se alcanza esta temperatura máxima segura durante el transporte. Realice los cálculos utilizando los siguientes métodos:

Primero que nada se anotan los datos, esto se hacen considerando un estado de condiciones límite que plantea el enunciado.
- $V=150\, \pu{ L}=0.15\, \pu{ m3}$
- $P_{\text{max}}=P=50\, \pu{ bar}=5·10^{6}\, \pu{ Pa}$
- $T_{\text{max}}=T=45\, \pu{ ºC}= 318.15 \, \pu{ K}$
Además se puede calcular que:
- $PM_{\, \pu{ N_{2}O}}=2·14 \, \pu{ \frac{g}{mol}}+16 \, \pu{ \frac{g}{mol}}=44\, \pu{ \frac{g}{mol}}$
Del apéndice A del libro _Matsoukas Thermodynamics_ disponible en canvas, se obtienen los siguientes valores del $\, \pu{ N_{2}O}$:
- $T_{\text{c}}=309.6\, \pu{ K}$
- $P_{\text{c}}=72.55\, \pu{ bar}$
- $V_{\text{c}}=97\, \pu{ \frac{cm^{3}}{mol}}$
- $\omega=0.162$ ^[Valor obtenido de anuncio en canvas] 

Se tienen los siguientes valores reducidos:

$$
\begin{align}
T_{\text{r}} & =\frac{T}{T_{\text{c}}} & P_{\text{r}} & =\frac{P}{P_{\text{c}}} \\
 & =\frac{318.15\, \pu{ \cancel{ K }}}{309.6\, \pu{ \cancel{ K }}} &  & =\frac{50\, \pu{ \cancel{ bar }}}{72.55\, \pu{ \cancel{ bar }}} \\
T_{\text{r}} & = 1.028 & P_{\text{r}} & = 0.689
\end{align}
$$
## Inciso a)

> [!quote]
> La ecuación de gas ideal.

Para un gas ideal:
$$
PV=nRT
$$

De aquí:
$$
\begin{align}
n & =\frac{PV}{RT} \\
 & =\frac{5·10^{6} \, \pu{ \frac{\cancel{ J }}{\cancel{ m^{3} }}}·0.15\, \pu{ \cancel{ m^{3} }}}{8.314 \, \pu{ \frac{\cancel{ J }}{mol·\cancel{ K }}}·318.15\, \pu{ \cancel{ K }}} \\
n & = 283.54\, \pu{ mol}
\end{align}
$$
Aplicando el peso molecular
$$
\begin{align}
m & =  44\, \pu{ \frac{\cancel{ g }}{\cancel{ mol }}}· 283.54\, \pu{ \cancel{ mol }}· \frac{1\, \pu{ kg}}{1000\, \pu{ \cancel{ g }}} \\
m & =12.476\, \pu{ kg}
\end{align}
$$
## Inciso b)

> [!quote]
> El método de Lee Kesler.

El método de Lee Kesler (Método de Pitzer con valores de Kee & Kesler) necesita un valor de $Z^{(0)}$ y $Z^{(1)}$ obtenidos de las gráficas.

En el gráfico:
<style> .container {font-family: sans-serif; text-align: center;} .button-wrapper button {z-index: 1;height: 40px; width: 100px; margin: 10px;padding: 5px;} .excalidraw .App-menu_top .buttonList { display: flex;} .excalidraw-wrapper { height: 800px; margin: 50px; position: relative;} :root[dir="ltr"] .excalidraw .layer-ui__wrapper .zen-mode-transition.App-menu_bottom--transition-left {transform: none;} </style><script src="https://cdn.jsdelivr.net/npm/react@17/umd/react.production.min.js"></script><script src="https://cdn.jsdelivr.net/npm/react-dom@17/umd/react-dom.production.min.js"></script><script type="text/javascript" src="https://cdn.jsdelivr.net/npm/@excalidraw/excalidraw@0/dist/excalidraw.production.min.js"></script><div id="Tarea_opcional_5_IIQ1103_2025-06-02_1519.23.excalidraw.md1"></div><script>(function(){const InitialData={"type":"excalidraw","version":2,"source":"https://github.com/zsviczian/obsidian-excalidraw-plugin/releases/tag/1.9.12","elements":[{"id":"fkoN4w-j69_PO4atwvQ6n","type":"image","x":-68.75634743493652,"y":-267.0840148925781,"width":364.7328918322296,"height":304,"angle":0,"strokeColor":"transparent","backgroundColor":"transparent","fillStyle":"hachure","strokeWidth":1,"strokeStyle":"solid","roughness":1,"opacity":100,"groupIds":[],"frameId":null,"roundness":null,"seed":1490158671,"version":4,"versionNonce":494551041,"isDeleted":false,"boundElements":null,"updated":1748891970202,"link":null,"locked":false,"status":"pending","fileId":"f5bceb8e3d29dbed9a10b53a19fffb68a6677854","scale":[1,1]},{"id":"vj8MlHYoumz-ON6voSUvj","type":"line","x":77.62675265351268,"y":8.224313005275803,"width":0,"height":226.82780857501646,"angle":0,"strokeColor":"#e03131","backgroundColor":"transparent","fillStyle":"hachure","strokeWidth":1,"strokeStyle":"solid","roughness":0,"opacity":100,"groupIds":[],"frameId":null,"roundness":{"type":2},"seed":1045068943,"version":227,"versionNonce":1386915617,"isDeleted":false,"boundElements":null,"updated":1748892126278,"link":null,"locked":false,"points":[[0,0],[0,-226.82780857501646]],"lastCommittedPoint":null,"startBinding":null,"endBinding":null,"startArrowhead":null,"endArrowhead":null},{"id":"hDiejB5-QaSt_rNGJz2EW","type":"line","x":79.59928776687806,"y":-156.4696810363276,"width":116.61510256312664,"height":0.22865742919137233,"angle":0,"strokeColor":"#e03131","backgroundColor":"transparent","fillStyle":"hachure","strokeWidth":1,"strokeStyle":"solid","roughness":0,"opacity":100,"groupIds":[],"frameId":null,"roundness":{"type":2},"seed":459993551,"version":166,"versionNonce":1758877281,"isDeleted":false,"boundElements":null,"updated":1748892215421,"link":null,"locked":false,"points":[[0,0],[-116.61510256312664,-0.22865742919137233]],"lastCommittedPoint":null,"startBinding":null,"endBinding":null,"startArrowhead":null,"endArrowhead":null}],"appState":{"theme":"light","viewBackgroundColor":"#ffffff","currentItemStrokeColor":"#e03131","currentItemBackgroundColor":"transparent","currentItemFillStyle":"hachure","currentItemStrokeWidth":1,"currentItemStrokeStyle":"solid","currentItemRoughness":0,"currentItemOpacity":100,"currentItemFontFamily":1,"currentItemFontSize":20,"currentItemTextAlign":"left","currentItemStartArrowhead":null,"currentItemEndArrowhead":"arrow","scrollX":71.0385983162195,"scrollY":180.61461086222403,"zoom":{"value":7.527249919003},"currentItemRoundness":"round","gridSize":null,"currentStrokeOptions":null,"previousGridSize":null,"frameRendering":{"enabled":true,"clip":true,"name":true,"outline":true}},"files":{}};InitialData.scrollToContent=true;App=()=>{const e=React.useRef(null),t=React.useRef(null),[n,i]=React.useState({width:void 0,height:void 0});return React.useEffect(()=>{i({width:t.current.getBoundingClientRect().width,height:t.current.getBoundingClientRect().height});const e=()=>{i({width:t.current.getBoundingClientRect().width,height:t.current.getBoundingClientRect().height})};return window.addEventListener("resize",e),()=>window.removeEventListener("resize",e)},[t]),React.createElement(React.Fragment,null,React.createElement("div",{className:"excalidraw-wrapper",ref:t},React.createElement(ExcalidrawLib.Excalidraw,{ref:e,width:n.width,height:n.height,initialData:InitialData,viewModeEnabled:!0,zenModeEnabled:!0,gridModeEnabled:!1})))},excalidrawWrapper=document.getElementById("Tarea_opcional_5_IIQ1103_2025-06-02_1519.23.excalidraw.md1");ReactDOM.render(React.createElement(App),excalidrawWrapper);})();</script>
Se va a tomar $Z^{(0)}=0.735$.

<div id="Tarea_opcional_5_IIQ1103_2025-06-02_1510.57.excalidraw.md2"></div><script>(function(){const InitialData={"type":"excalidraw","version":2,"source":"https://github.com/zsviczian/obsidian-excalidraw-plugin/releases/tag/1.9.12","elements":[{"id":"DECcOo0li9NUizQ73MnPc","type":"image","x":-163.36225174923646,"y":-111.08401489257812,"width":371.9447004608295,"height":304,"angle":0,"strokeColor":"transparent","backgroundColor":"transparent","fillStyle":"hachure","strokeWidth":1,"strokeStyle":"solid","roughness":1,"opacity":100,"groupIds":[],"frameId":null,"roundness":null,"seed":755752806,"version":4,"versionNonce":1266442938,"isDeleted":false,"boundElements":null,"updated":1748891468283,"link":null,"locked":false,"status":"pending","fileId":"8f4e3a4ab34cef3db7c7e311e86289972adf28b0","scale":[1,1]},{"id":"1fFgDBZ2Nb2sgmbZ-N9wK","type":"line","x":-5.4866168689551955,"y":160.03114017997243,"width":0.2378014552802199,"height":175.73500714736986,"angle":0,"strokeColor":"#e03131","backgroundColor":"transparent","fillStyle":"hachure","strokeWidth":1,"strokeStyle":"solid","roughness":0,"opacity":100,"groupIds":[],"frameId":null,"roundness":{"type":2},"seed":50052582,"version":335,"versionNonce":466289830,"isDeleted":false,"boundElements":null,"updated":1748891504205,"link":null,"locked":false,"points":[[0,0],[-0.2378014552802199,-175.73500714736986]],"lastCommittedPoint":[-0.2378014552802199,-175.73500714736986],"startBinding":null,"endBinding":null,"startArrowhead":null,"endArrowhead":null},{"id":"Kx0Okokz8M8iATO5AygFN","type":"line","x":-2.98970684594633,"y":38.20687266772914,"width":128.4125950568566,"height":0.7134043658407023,"angle":0,"strokeColor":"#e03131","backgroundColor":"transparent","fillStyle":"hachure","strokeWidth":1,"strokeStyle":"solid","roughness":0,"opacity":100,"groupIds":[],"frameId":null,"roundness":{"type":2},"seed":42958822,"version":141,"versionNonce":1373219686,"isDeleted":false,"boundElements":null,"updated":1748891681683,"link":null,"locked":false,"points":[[0,0],[-128.4125950568566,-0.7134043658407023]],"lastCommittedPoint":[-128.4125950568566,-0.7134043658407023],"startBinding":null,"endBinding":null,"startArrowhead":null,"endArrowhead":null}],"appState":{"theme":"light","viewBackgroundColor":"#ffffff","currentItemStrokeColor":"#e03131","currentItemBackgroundColor":"transparent","currentItemFillStyle":"hachure","currentItemStrokeWidth":1,"currentItemStrokeStyle":"solid","currentItemRoughness":0,"currentItemOpacity":100,"currentItemFontFamily":1,"currentItemFontSize":20,"currentItemTextAlign":"left","currentItemStartArrowhead":null,"currentItemEndArrowhead":"arrow","scrollX":280.11343346340226,"scrollY":53.71488365842968,"zoom":{"value":2.559200246489588},"currentItemRoundness":"round","gridSize":null,"currentStrokeOptions":null,"previousGridSize":null,"frameRendering":{"enabled":true,"clip":true,"name":true,"outline":true}},"files":{}};InitialData.scrollToContent=true;App=()=>{const e=React.useRef(null),t=React.useRef(null),[n,i]=React.useState({width:void 0,height:void 0});return React.useEffect(()=>{i({width:t.current.getBoundingClientRect().width,height:t.current.getBoundingClientRect().height});const e=()=>{i({width:t.current.getBoundingClientRect().width,height:t.current.getBoundingClientRect().height})};return window.addEventListener("resize",e),()=>window.removeEventListener("resize",e)},[t]),React.createElement(React.Fragment,null,React.createElement("div",{className:"excalidraw-wrapper",ref:t},React.createElement(ExcalidrawLib.Excalidraw,{ref:e,width:n.width,height:n.height,initialData:InitialData,viewModeEnabled:!0,zenModeEnabled:!0,gridModeEnabled:!1})))},excalidrawWrapper=document.getElementById("Tarea_opcional_5_IIQ1103_2025-06-02_1510.57.excalidraw.md2");ReactDOM.render(React.createElement(App),excalidrawWrapper);})();</script>
Se va a tomar $Z^{(1)}=-0.02$.
Ahora, usando la relación de Lee & Kesler:
$$
\begin{align}
Z &= Z^{(0)}+\omega Z^{(1)} \\
 & \approx0.735-0.162·0.02 \\
 Z& \approx0.731
\end{align}
$$
Ahora se aplica la definición de $Z$:
$$
\begin{align}
Z & =\frac{PV_{m}}{RT} \\
V_{m} & =\frac{ZRT}{P} \\
V_{m} & = \frac{0.731·8.314 \, \pu{ \frac{\cancel{ J }}{mol·\cancel{ K }}}·318.15\, \pu{ \cancel{ K }}}{5·10^{6} \, \pu{ \frac{\cancel{ J }}{m^{3}}}} \\
V_{m} & = 0.000387 \, \pu{ \frac{m^{3}}{mol}}
\end{align}
$$
Ponderando por $PM_{\, \pu{ N_{2}O}}$ y $V$:
$$
\begin{align}
m & =\frac{0.15\, \pu{ \cancel{ m^{3} }}}{0.000387 \, \pu{ \frac{\cancel{ m^{3} }}{\cancel{ mol }}}} ·44 \, \pu{ \frac{\cancel{ g }}{\cancel{ mol }}} · \frac{1 \, \pu{ kg}}{1000\, \pu{ \cancel{ g }}} \\
m & =17.0543\, \pu{ kg}
\end{align} 
$$
## Inciso c)

> [!quote]
> La ecuación virial truncada al segundo coeficiente.

En clases, se vio que:
$$
Z\approx1 + \frac{BP}{RT} \tag{c.1}
$$
Reemplazando la definición de $Z$ se llega a que:
$$
P·(V_{m}-B)\approx RT
$$
Para obtener el valor de $B$ se deben encontrar valores $B^{1}$ y $B^{0}$ tales que:
$$
\frac{BP_{\text{c}}}{RT_{\text{c}}}=B^{0}+\omega B^{1}
$$
Por lo visto en clases:
$$
\begin{align}
B^{0} & =0.083-\frac{0.422}{T_{\text{r}}^{1.6}} & B^{1} & =0.139-\frac{0.172}{T_{\text{r}}^{4.2}} \\
 & =0.083 - \frac{0.422}{1.028^{1.6}} &  & =0.139- \frac{0.172}{1.028^{4.2}} \\
 B^{0}& =-0.3201 &  B^{1}& = -  0.0142
\end{align}
$$
Ahora:
$$
\begin{align}
B & =\frac{B^{0}+\omega B^{1}}{P_{\text{c}}}RT_{\text{c}} \\
 & = \frac{-0.3201-0.162·0.0142}{7255000\, \pu{ \cancel{ J }/m^{3}}}8.314 \, \pu{ \frac{\cancel{ J }}{mol·\cancel{ K }}}·309.6 \, \pu{ \cancel{ K }} \\
B & =-0.0001144 \, \pu{ \frac{m^{3}}{mol}}
\end{align}
$$
Reemplazando en (c.1):
$$
\begin{align}
Z & \approx 1- \frac{0.0001144 \, \pu{ \frac{\cancel{ m^{3} }}{\cancel{ mol }}}·5·10^{6}\, \pu{ \cancel{ J }/\cancel{ m^{3} }}}{8.314 \, \pu{ \frac{\cancel{ J }}{\cancel{ mol }·\cancel{ K }}}318.15\, \pu{ \cancel{ K }}} \\
Z & \approx 0.784
\end{align}
$$
Reemplazando en la definición de $Z$:
$$
\begin{align}
Z & =\frac{PV_{m}}{RT} \\
V_{m} & =\frac{ZRT}{P} \\
V_{m} & = \frac{0.784·8.314 \, \pu{ \frac{\cancel{ J }}{mol·\cancel{ K }}}·318.15\, \pu{ \cancel{ K }}}{5·10^{6} \, \pu{ \frac{\cancel{ J }}{m^{3}}}} \\
V_{m} & =  0.0004147 \, \pu{ \frac{m^{3}}{mol}}
\end{align}
$$
Ahora pasando a $\pu{ kg}$:
$$
\begin{align}
m & =\frac{0.15\, \pu{ \cancel{ m^{3} }}}{ 0.0004147 \, \pu{ \frac{\cancel{ m^{3} }}{\cancel{ mol }}}} ·44 \, \pu{ \frac{\cancel{ g }}{\cancel{ mol }}} · \frac{1 \, \pu{ kg}}{1000\, \pu{ \cancel{ g }}} \\
m & =15.915\, \pu{ kg}
\end{align} 
$$
## Inciso d)

> [!quote]
> La ecuación de Van der Waals.

Se necesitan calcular las constante $a$ y $b$ para el $\pu{ N_{2}O}$.

Para esto se usan las ecuaciones vistas en clases:
$$
\begin{align}
a & =\frac{27}{64} \frac{(RT_{\text{c}})^{2}}{P_{\text{c}}} & b & =\frac{RT_{\text{c}}}{8P_{\text{c}}} \\
 & =\frac{27}{64} \frac{\left( 8.314 \, \pu{ \frac{J}{mol·\cancel{ K }}}309.6\, \pu{ \cancel{ K }} \right)^{2}}{72.55 ·10^{5} \, \pu{ J/m^{3}}} &  & =\frac{8.314 \, \pu{ \frac{\cancel{ J }}{mol·\cancel{ K }}}·309.6\, \pu{ \cancel{ K }}}{8·72.55 ·10^{5}\, \pu{ \cancel{ J }/m^{3}}} \\
 a & = 0.3853 \, \pu{ \frac{J·m^{3}}{mol^{2}}} =0.3853\, \pu{ \frac{Pa·m^{6}}{mol^{2}}}& b & =44.3 ·10^{-6} \, \pu{ \frac{m^{3}}{mol}} \\

\end{align}
$$
Ahora, según lo visto en clases, se tiene la siguiente ecuación cúbica:
$$
V_{m}^{3}-\left( b+\frac{RT}{P} \right)V^{2}_{m}+\frac{a}{P}V_{m}-\frac{ab}{P}=0
$$
Tras reemplazar esto en el programa Wolfram Mathematica, se obtuvieron dos valores complejos conjugados y uno real. Se va a tomar el real, que también es el mayor (valor para vapor saturado):
$$
V_{m}=0.0004032 \, \pu{ \frac{m^{3}}{mol}}
$$
Despejando $m$:
$$
\begin{align}
m & =\frac{0.15\, \pu{ \cancel{ m^{3} }}}{ 0.0004032 \, \pu{ \frac{\cancel{ m^{3} }}{\cancel{ mol }}}} ·44 \, \pu{ \frac{\cancel{ g }}{\cancel{ mol }}} · \frac{1 \, \pu{ kg}}{1000\, \pu{ \cancel{ g }}} \\
m & =16.369\, \pu{ kg}
\end{align} 
$$
## Inciso e)

> [!quote]
> La ecuación de Soave-Redlich-Kwong.

Nuevamente se debe despejar el valor de $a$ y $b$, pero estos dependen de un valor $\Omega$ o $k_{RK}$ dado por:
$$
\begin{align}
\Omega & =0.480+1.574\omega -0.176\omega^{2} \\
 & = 0.480  +  1.574 · 0.162  -  0.176  · 0.162  ^ { 2 } \\
\Omega & = 0.7304
\end{align}
$$
El valor de $a$ se despeja de la siguiente forma por lo visto en clases:
$$
\begin{align}
a & =0.42748 \frac{R^{2}T_{\text{c}}^{2}}{P_{\text{c}}}[1+(1-\sqrt{ T_{\text{r}} })·\Omega]^{2} \\
 & =0.42748 \frac{\left( 8.314 \, \pu{ \frac{J}{mol·\cancel{ K }}} ·309.6\, \pu{ \cancel{ K }}\right)^{2}}{72.55·10^{5}\, \pu{ J/m^{3}}}[1+(1-\sqrt{ 1.028 })·0.7304]^{2} \\
a & =0.3825\, \pu{ \frac{J·m^{3}}{mol^{2}}}=0.3825\, \pu{ \frac{Pa·m^{6}}{mol^{2}}}
\end{align}
$$
La ecuación para SRK de $b$ es:
$$
\begin{align}
b & =0.0866404 \frac{R T_{\text{c}}}{P_{\text{c}}} \\
 & =0.0866404 \frac{8.314 \, \pu{ \frac{J}{mol·K}} · 309.6\, \pu{ K}}{72.55·10^{5}\, \pu{ J/m^{3}}} \\
b & =30.7·10^{-6} \, \pu{ \frac{m^{3}}{mol}}
\end{align}
$$
Ahora se va a tener la siguiente ecuación cúbica:
$$
P= \frac{RT}{V_{m}-b}- \frac{a}{V_{m}(V_{m}+b)}
$$
Resolviendo con la calculadora Wolfram Mathematica para $V_{m}$. Nuevamente, se obtuvieron dos valores complejos conjugados y uno real (el mayor, respectivo al vapor saturado).
$$
V_{m}=0.000393422 \, \pu{ \frac{m^{3}}{mol}}
$$
Despejando $m$:
$$
\begin{align}
m & =\frac{0.15\, \pu{ \cancel{ m^{3} }}}{ 0.000393422 \, \pu{ \frac{\cancel{ m^{3} }}{\cancel{ mol }}}} ·44 \, \pu{ \frac{\cancel{ g }}{\cancel{ mol }}} · \frac{1 \, \pu{ kg}}{1000\, \pu{ \cancel{ g }}} \\
m & = 16.7759\, \pu{ kg}
\end{align} 
$$

## Inciso f)

> [!quote]
> La ecuación de Peng Robinson

Los valores de $a$ y $b$ se definen de la siguiente forma:
$$
\begin{align}
a & =0.45724 \frac{R^{2}T_{\text{c}}^{2}}{P_{\text{c}}} \left[ 1+(1-\sqrt{ T_{\text{r}} })·\Omega \right]^{2}  \\
& =0.45724 \frac{\left( 8.314 \, \pu{ \frac{J}{mol·\cancel{ K }}} ·309.6\, \pu{ \cancel{ K }}\right)^{2}}{72.55·10^{5}\, \pu{ J/m^{3}}}[1+(1-\sqrt{ 1.028 })·0.7304]^{2} \\
a & = 0.4091\, \pu{ \frac{J·m^{3}}{mol^{2}}}=0.4091\, \pu{ \frac{Pa·m^{6}}{mol^{2}}}
\end{align}
$$
El valor de $b$ se obtiene con la siguiente ecuación:
$$
\begin{align}
b & =0.07780 \frac{R T_{\text{c}}}{P_{\text{c}}} \\
 & =0.07780 \frac{8.314 \, \pu{ \frac{J}{mol·K}} · 309.6\, \pu{ K}}{72.55·10^{5}\, \pu{ J/m^{3}}} \\
b & =27.603·10^{-6} \, \pu{ \frac{m^{3}}{mol}}
\end{align}
$$
La ecuación de Peng-Robinson dice que:
$$
P= \frac{RT}{V_{m}-b}- \frac{a}{V_{m}^{2}+2bV_{m}-b^{2}}
$$
Resolviendo en _Mathematica_, y nuevamente tomando el valor real:
$$
V_{m}=0.0003823 \, \pu{ \frac{m^{2}}{mol}}
$$
Despejando $m$:
$$
\begin{align}
m & =\frac{0.15\, \pu{ \cancel{ m^{3} }}}{ 0.0003823 \, \pu{ \frac{\cancel{ m^{3} }}{\cancel{ mol }}}} ·44 \, \pu{ \frac{\cancel{ g }}{\cancel{ mol }}} · \frac{1 \, \pu{ kg}}{1000\, \pu{ \cancel{ g }}} \\
m & = 17.2639\, \pu{ kg}
\end{align} 
$$
