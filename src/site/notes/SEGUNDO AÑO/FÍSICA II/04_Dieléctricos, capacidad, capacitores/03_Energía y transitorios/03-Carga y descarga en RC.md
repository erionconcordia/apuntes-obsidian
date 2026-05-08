---
{"dg-publish":true,"permalink":"/segundo-ano/fisica-ii/04-dielectricos-capacidad-capacitores/03-energia-y-transitorios/03-carga-y-descarga-en-rc/","dgPassFrontmatter":true,"dg-note-properties":{}}
---

Tags: #transitorios #circuito-RC #carga #descarga

## 1. Proceso de carga: desarrollo matemático
Consideremos un circuito con una fuente de voltaje ($V_{ab}$), una resistencia ($R$), un condensador ($C$) inicialmente descargado y un interruptor ($S$).

![Pasted image 20260504123111.png](/img/user/IM%C3%81GENES/Pasted%20image%2020260504123111.png)

En el instante en que cerramos el interruptor ($t=0$), la suma de las caídas de potencial en el circuito debe ser igual al voltaje de la fuente:
$$V_{ab}=v_R+v_C$$
Usando la Ley de Ohm ($v_R=i\cdot R$) y la definición de capacidad ($v_C=q/C$):
$$V_{ab}=i\cdot R+\frac{q}{C}$$
Como la intensidad es la rapidez con la que llega la carga ($i=dq/dt$), sustituimos y reordenamos para obtener la **ecuación diferencial del proceso**:
$$\frac{dq}{dt}+\frac{q}{RC}-\frac{V_{ab}}{R}=0$$
Resolviendo mediante el uso de un factor integrante e integrando entre los límites de tiempo 0 y $t$, y carga 0 y $q$, llegamos a la **función de carga**:
$$q(t)=C\cdot V_{ab}\cdot\left(1-e^{-t/RC}\right)$$
- Donde $Q_f=C\cdot V_{ab}$ es la carga final máxima que alcanzará el condensador después de un tiempo "infinito".

Derivando la expresión de la carga respecto al tiempo, obtenemos cómo varía la **corriente**:
$$i(t)=\frac{V_{ab}}{R}\cdot e^{-t/RC}$$
---
## 2. Constante de tiempo ($\tau$)
El producto $R\cdot C$ tiene unidades de tiempo y es el parámetro más importante del circuito. Se denomina constante de tiempo ($\tau$).

>[!definicion] Definición física: Constante de tiempo ($\tau$)
>Es el tiempo necesario para que la carga del condensador aumente hasta que la diferencia entre la carga final y la actual sea una fracción $1/e\ (\approx36.9\%)$ de su valor final. Matemáticamente:
>$$\tau=R\cdot C$$

En la práctica, tras un intervalo de tiempo igual a $5\tau$, se considera que el condensador está totalmente cargado (alcanza el 99.3% de su valor final).

**A)** **"$t$" es el reloj, $\tau$ es el ADN del circuito**
El valor $t$ es una variable independiente (un segundo, dos segundos, etc.). Pero $\tau=R\cdot C$ es una propiedad intrínseca de un circuito específico.
- Si tenemos un capacitor gigante ($C$ grande) o cables muy finos con mucha resistencia ($R$ grande), el producto $R\cdot C$ será un número alto. Esto nos dice que el circuito es lento.
- Si ambos son chicos, el circuito es veloz.

**B) La necesidad matemática**
En física, no podemos elevar un número a la "5 segundos" ($e^{5s}$), eso no tiene sentido matemático. Los exponentes deben ser números puros (sin unidades). Al usar la fracción $t\cdot\tau$, dividimos "segundos" por "segundos" ($R\cdot C$ da segundos), y obtenemos un número puro que la función exponencial puede procesar.

**C) El valor de referencia universal**
$\tau$ sirve como una "regla de medir" universal para cualquier circuito RC:
- En $1\tau$, la corriente siempre habrá caído al 36.9% de su valor inicial.
- En $1\tau$, al capacitor siempre le faltará exactamente un 36.9% para terminar de cargarse.
- Se considera que un capacitor está totalmente cargado (o descargado) cuando han pasado $5\tau$. En ese punto, el proceso ha llegado al 99.3%, lo cual es suficiente para cualquier ingeniero.

**D) ¿Por qué no usar simplemente un valor "t" de tiempo?**
Porque el valor "$t$" es solo una medida externa. En cambio, $\tau$ nos habla de la calidad y el diseño del circuito: nos dice si el sistema fue construido para liberar su energía de forma explosiva ($\tau$ pequeña, poca resistencia) o de forma lenta y controlada ($\tau$ grande, mucha resistencia).

>[!example] Ejemplo con fórmula 1
>Imaginemos que el sistema ERS de un piloto es un capacitor:
>- $t$ es el tiempo que el piloto pasa frenando la curva.
>- $\tau$ es la eficiencia del sistema: si los cables son malos ($R$ alto), $\tau$ es grande.
>- Si el ingeniero le dice al piloto: "cargamos en 2 segundos", eso no le sirve a otro auto. Pero si dice: "este sistema se carga en 5$\tau$", es una ley universal para ese diseño. No importa si le ponemos una batería de 12V o de 1000V, el tiempo que tarda en llenarse (su "ritmo") siempre estará dictado por su $\tau$ ($R\cdot C$).

---
## 3. Análisis de gráficos durante la carga
Los gráficos de carga y corriente son opuestos y se aproximan a sus valores finales de forma asintótica.
#### 3.1. Gráfico de carga ($q$)
![Pasted image 20260504124123.png](/img/user/IM%C3%81GENES/Pasted%20image%2020260504124123.png)

Este gráfico representa cómo el capacitor se va cargando de electrones.

En el instante exacto en el que cerramos el interruptor $S$ del circuito ($t=0$), la carga es cero ($q=0$). Físicamente, el condensador se comporta como un cable pelado (un cortocircuito) porque no hay cargas adentro que se opongan a la que quieren entrar.

La curva (con crecimiento exponencial) sube muy rápido al principio y luego se va "achatando".
- **¿Por qué?** Porque a medida que entran cargas al capacitor, este empieza a generar su voltaje ($v_C=q/C$). Este voltaje interno tiene el sentido opuesto al de la fem.
- Imaginemos que la batería empuja cargas hacia adentro, pero las cargas que ya entraron empujan hacia afuera. Cuantas más cargas hay adentro, más difícil es meter la siguiente.
La curva nunca toca la línea de carga máxima ($Q=C\cdot V_{ab}$), tiene una asíntota cuanto $t\to\infty$. En la teoría, tardaría un tiempo infinito en llenarse al 100%, aunque en la práctica, después de un *ratito*, la diferencia es tan minúscula que lo consideramos lleno.

#### 3.2. Gráfico de intensidad ($i$)
![Pasted image 20260504124700.png](/img/user/IM%C3%81GENES/Pasted%20image%2020260504124700.png)
Este gráfico es el "espejo" del anterior y representa la velocidad del flujo.

En $t=0$, la corriente arranca en su valor más alto: $I_0=V_{ab}/R$. Es el pico máximo porque, como el capacitor está vacío, no ofrece ninguna resistencia al paso de la corriente; solo los cables ($R$) limitan el flujo.

La corriente baja rápidamente hacia el cero tras cierto período de tiempo (decaimiento exponencial).
- **¿Por qué?** Por la misma razón que la carga se frena: el capacitor se está llenando y su "contra-voltaje" es cada vez más fuerte. La fuerza neta que empuja a los electrones ($V_{ab}-v_C$) es cada vez más chica, por lo tanto, circulan cada vez más "lento".

Cuando el voltaje del capacitor "iguala" exactamente al de la batería, la corriente cesa por completo y el circuito queda "abierto" por el propio capacitor.

---
## 4. Proceso de descarga
Si desconectamos la batería y cerramos el circuito uniendo las placas a través de la resistencia, el condensador actúa como fuente. El desarrollo es similar pero con $V_{ab}=0$:

**Carga en descarga:** La carga disminuye exponencialmente.
$$q(t)=Q_0\cdot e^{-t/RC}$$
**Corriente en descarga:** La corriente fluye en sentido opuesto y también decae.
$$i(t)=I_0\cdot e^{-t/RC}$$

---
## 5. Análisis de gráficos durante la descarga
#### 5.1. Gráfica de carga en descarga ($q$)
Este gráfico representa cómo se va vaciando el "tanque" de electrones a medida que circulan por la resistencia.
![Pasted image 20260504132031.png](/img/user/IM%C3%81GENES/Pasted%20image%2020260504132031.png)

En el instante exacto en el que se cierra el interruptor para iniciar la descarga ($t=0$), el condensador posee una carga máxima inicial ($Q_0$). En este momento, la diferencia de potencial durante sus armaduras es máxima ($V_0=Q_0/C$) y está listo para liberar toda su energía.

La curva de $q$ baja muy rápido al principio (decaimiento exponencial) y luego se va suavizando gradualmente hasta acercarse al eje cero.
- **¿Por qué sucede esto?** El condensador actúa como una batería cuya "fuerza" (voltaje) depende directamente de cuánta carga le queda ($v_C=q/C$). Al principio, al estar lleno, empuja los electrones con mucha intensidad. A medida que pierde carga, su voltaje disminuye y, por lo tanto, tiene cada vez menos fuerza para empujar el remanente de carga a través de la resistencia.

Teóricamente, el condensador tarda un tiempo infinito en vaciarse por completo (tiene comportamiento asintótico cuando $t\to\infty$), ya que la tasa de descarga se vuelve infinitesimalmente pequeña a medida que la carga se agota. Sin embargo, a fines prácticos, se considera descargado en un tiempo muy breve.

#### 5.2. Gráfica de intensidad en descarga ($i$)
![Pasted image 20260504132542.png](/img/user/IM%C3%81GENES/Pasted%20image%2020260504132542.png)

En el instante inicial ($t=0$), la corriente salta instantáneamente a su valor más alto: $I_0=V_{capacitor}/R$.
- Nota de sentido: *Es importante notar que, si definimos el sentido de la corriente de carga como positivo, la corriente de descarga fluye en sentido opuesto (sale de la placa positiva), por lo que en muchos textos este gráfico se dibuja en la parte negativa del eje de ordenadas*.

Al igual que la carga, la intensidad de la corriente disminuye exponencialmente siguiendo el ritmo de voltaje del condensador.
- **¿Por qué decae?** Como el "tanque" tiene cada vez menos presión (voltaje), la velocidad a la que los electrones pueden atravesar la resistencia disminuye hasta que se detienen por completo cuando la diferencia de potencial llega a cero.