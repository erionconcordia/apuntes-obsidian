---
{"dg-publish":true,"permalink":"/segundo-ano/fisica-ii/03-intensidad-resistencia-circuitos/03-generadores-y-ec-basicas/01-fuerza-electromotriz-fem/","dgPassFrontmatter":true,"dg-note-properties":{}}
---

Tags: #electrodinámica #fem #generadores #baterías

## 1. Concepto de reversibilidad termodinámica
Cuando la corriente pasa por un conductor con resistencia, la energía se convierte en calor y se pierde hacia el ambiente (proceso irreversible, ya que el calor no puede transformarse de nuevo en energía eléctrica al 100%).

Po el contrario, dispositivos como una batería de acumuladores, un alternador o un motor realizan transformaciones energéticas reversibles en el sentido termodinámico.
- **Descarga:** En la batería de un automóvil al encender el motor de arranque, la energía interna (química) disminuye y se convierte en energía eléctrica (y luego mecánica).
- **Carga:** Una vez en marcha, el alternador envía una corriente en sentido contrario hacia la batería, transformando de nuevo la energía eléctrica en energía interna.
A cualquier dispositivo en el cual pueda producirse esta transformación reversible entre energía eléctrica y otra forma de energía, se lo denomina **generador de fuerza electromotriz**.

---
## 2. Definición y ecuación de la fem ($\epsilon$)
El valor de la fuerza electromotriz de un generador se define como la energía convertida de forma eléctrica a no eléctrica (o viceversa) por unidad de carga que pasa a través del mismo. En resumen, la fuerza electromotriz es el trabajo por unidad de carga.

Si una carga $dq$ atraviesa el generador en un tiempo $dt$, y $dW$ es la energía transformada en ese tiempo, la fem ($\epsilon$) se define como:
$$\epsilon=\frac{dW}{dq}$$
>[!important] La Unidad: El volt
>Puesto que la fuerza electromotriz es trabajo por unidad de carga, su unidad en el SI es el Joule por Coulomb, a la que llamamos Volt ($V$).
>
>*Aclaración:* Aunque la fem y la diferencia de potencial se miden en voltios, se refieren a conceptos físicamente distintos (la fem representa la conversión de energía de otra naturaleza a eléctrica, mientras que el potencial es simplemente una medida del nivel energético en un punto).

---
## 3. Potencia del generador
El trabajo realizado por el generador al mover esa carga es $dW=\epsilon\cdot dq$. Si queremos saber con qué rapidez suministra o consume esa energía (su potencia $P$), dividimos por el tiempo ($dt$):
$$P=\frac{dW}{dt}=\epsilon\cdot i$$
*Ejemplo práctico:* La fem de una batería de automóvil típica es de unos 12 V (12 J/C). Esto significa que, por cada Coulomb que pasa, 12 Joules de energía interna se convierten en electricidad. Si el circuito consume una corriente de 10 A (10 Coulombs por segundo), la energía transformada por unidad de tiempo será $P=12V\cdot 10A=120W$.

![Pasted image 20260502195902.png](/img/user/IM%C3%81GENES/Pasted%20image%2020260502195902.png)
