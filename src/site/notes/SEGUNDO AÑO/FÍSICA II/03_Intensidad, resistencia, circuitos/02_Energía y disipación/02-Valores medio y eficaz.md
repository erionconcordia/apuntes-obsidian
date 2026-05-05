---
{"dg-publish":true,"permalink":"/segundo-ano/fisica-ii/03-intensidad-resistencia-circuitos/02-energia-y-disipacion/02-valores-medio-y-eficaz/","dgPassFrontmatter":true,"dg-note-properties":{}}
---

Tags: #electrodinámica #corriente-alterna #valor-eficaz #valor-medio

>[!abstract] Resumen y conexión
>Cuando la intensidad de una corriente eléctrica no es constante, sino que varía con el tiempo (como en la corriente alterna de nuestros hogares), es muy difícil hacer cálculos directos de energía. Para resolver esto, los físicos definieron dos "valores equivalentes" de corriente continua que nos simplifican la vida: el valor medio (basado en la carga total transportada) y el valore eficaz (basado en el calor total disipado).
>
>Es muy similar a lo desarrollado en la cátedra de *ELECTROTECNIA I*: [[SEGUNDO AÑO/ELECTROTECNIA I/03_Circuitos de CA/03_Conceptos/14-Valor eficaz o RMS\|14-Valor eficaz o RMS]]. En esencia son lo mismo.

---
## 1. Valor medio (transporte de carga)
Sabemos que la carga transportada por una corriente constante es simplemente $q=i\cdot t$. Pero si la corriente $i$ varía con el tiempo, la carga total debe calcularse integrando:
$$q=\int_0^ti\cdot dt$$
El valor medio ($I_m$) de una corriente variable se define como la intensidad de una corriente constante imaginaria que transportaría exactamente la misma carga neta en el mismo intervalo de tiempo que la corriente variable real.
$$I_m=\frac{1}{t}\int_0^ti\cdot dt$$
**Utilidad:** El valor medio es una medida directa del efecto electrolítico de la corriente, ya que la masa de sustancia depositada en un electrodo depende exclusivamente de la cantidad total de carga que circuló.

---
## 2. Valor eficaz (RMS)
El transporte de carga no es lo único que nos importa; la disipación de calor (Ley de Joule) es vital. Como el calor depende del cuadrado de la corriente, los picos de intensidad generan muchísimo más calor proporcionalmente.

El valor eficaz ($I_{ef}$) de una corriente variable se define como la intensidad constante imaginaria que desarrollaría exactamente la misma cantidad de calor en la misma resistencia y en el mismo tiempo.

Igualando el calor de una corriente constante ($I_{ef}^2\cdot R\cdot t$) con el calor integrado de la variable ($\int i^2\cdot R\cdot dt$), obtenemos:
$$I_{ef}=\sqrt{\frac{1}{t}\int_0^ti^2\cdot dt}$$

---
## 3. La corriente alterna sinusoidal
El tipo más común de corriente variable es la que sale de los enchufes de pared, la cual oscila siguiendo una función seno:
$$i=I_0\sin(2\pi ft)$$
Donde $I_0$ es el pico máximo de corriente y $f$ es la frecuencia en Hertz ($Hz$).
![Pasted image 20260502194555.png](/img/user/IM%C3%81GENES/Pasted%20image%2020260502194555.png)

Si aplicamos la integral del "valor eficaz" a esta onda matemática y resolvemos, llegamos a un resultado súper simple:
$$I_{ef}=\frac{I_0}{\sqrt{2}}\approx0.707\cdot I_0$$
>[!important] ¿Qué significa esto en la realidad?
>El efecto calorífico de una corriente alterna es exactamente el mismo que produciría una corriente continua que valga el 70.7% de su pico máximo.
>
>*Detalle clave: En la práctica, cuando nos dicen "tenemos un enchufe de 220 V" o "circulan 10 A de alterna", siempre están dando valores eficaces, nunca los picos máximos, a menos que se aclare.*

