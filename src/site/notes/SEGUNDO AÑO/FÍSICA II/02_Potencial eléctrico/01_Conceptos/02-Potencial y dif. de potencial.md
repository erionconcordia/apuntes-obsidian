---
{"dg-publish":true,"permalink":"/segundo-ano/fisica-ii/02-potencial-electrico/01-conceptos/02-potencial-y-dif-de-potencial/","dgPassFrontmatter":true,"dg-note-properties":{}}
---

Tags: #potencial #voltaje #volt

>[!abstract] Resumen de relaciones
>Así como la intensidad de un campo eléctrico es la "fuerza por unidad de carga", el potencial eléctrico es la "energía potencial por unidad de carga". Esta magnitud escalar nos permite describir un campo eléctrico no por los empujones que da, sino por el nivel de energía que tiene cada punto del espacio, dándonos origen al famoso Volt.

---
## 1. Definición de Potencial
Recordemos que la intensidad de un campo eléctrico ($E$) en un punto es la razón entre la fuerza ejercida sobre una carga de prueba y el valor de dicha carga ($E=F/q'$).
Análogamente, el potencial ($V$) en un punto de un campo eléctrico se define así:

>[!definicion] Definición: Potencial eléctrico
>El potencial, denotado como $V$, en un punto de un campo eléctrico se define como la razón de la energía potencial de un cuerpo de prueba al valor de su carga.
>$$V_a=\frac{EP_a}{q'}$$

En otras palabras, el potencial es la energía potencial por unidad de carga.

>[!important] La unidad: El Volt
>Como la energía se mide en Joule ($J$) y la carga en Coulomb ($C$), el potencial se expresa en Joule por Coulomb ($J/C$). A esta unidad se la bautizó Volt ($V$) en honor a Alessandro Volta, el inventor de la pila.

---
## 2. Diferencia de potencial (Voltaje)
En la práctica, casi nunca nos importa traer cargas desde el infinito. Lo que realmente medimos en los circuitos es la diferencia de potencial entre dos puntos reales, $a$ y $b$.

Si dividimos el trabajo necesario para ir de $a$ hacia $b$ por la carga, obtenemos la diferencia de potencial ($V_{ab}$), también conocida coloquialmente como voltaje:
$$V_{ab}=V_a-V_b=-\int_b^aE\cdot\cos(\theta)\cdot ds$$
La diferencia de potencial entre $b$ y $a$ es el trabajo realizado por unidad de carga contra las fuerzas eléctricas para mover una carga desde $b$ hasta $a$.

>[!warning] Aclaración importante sobre ($V_{ab}$)
>Es muy común encontrar dos formas distintas de escribir esta diferencia de potencial:
>**1. Potencial relativo**
>La diferencia de potencial entre dos puntos $a$ y $b$, expresada abreviadamente por $V_{ab}$, se define estrictamente como el potencial del primer punto menos el del segundo:
>$$V_{ab}=V_a-V_b$$
>Esta forma mide qué tan por encima (o por debajo) está el nivel de energía de $a$ respecto al de $b$.
>
>**2. Variación de potencial $\Delta V$**
>A veces, en la práctica, cuando analizamos una carga que se mueve físicamente desde el punto $a$ hacia el punto $b$, nos interesa calcular el incremento o salto total ("final menos inicial"):
>$$\Delta V_{a\to b}=V_{ab}=V_{final}-V_{inicial}=V_b-V_a$$
>Si el resultado es negativo, significa que la carga perdió potencial en el trayecto.

![Pasted image 20260502161553.png\|219](/img/user/IM%C3%81GENES/Pasted%20image%2020260502161553.png)

**¿Qué significa esto en la vida real?** Si la diferencia de potencial entre los bornes de una batería de auto es de 12 V, significa que para transportar una carga positiva desde el borne negativo al borne positivo, hay que realizar un trabajo contra el campo de *12 Joules por cada Coulomb* de carga que crucemos. El borne positivo se encuentra a un potencial superior al negativo.

---
## 3. La integran en una trayectoria cerrada
Hay una propiedad matemática fundamental que hace que el concepto de "potencial" tenga sentido lógico. Vimos que la diferencia de potencial es la integral curvilínea (cambiada de signo) del campo eléctrico a lo largo de una trayectoria.

**¿Qué pasa si la trayectoria se cierra sobre sí misma, de modo que salimos del punto $a$, damos una vuelta por el campo y volvemos exactamente al punto $a$?** La diferencia de potencial entre un punto y sí mismo es evidentemente cero. Por lo tanto:
$$\oint E\cdot\cos(\theta)\cdot ds=0$$
Esta ecuación demuestra que el trabajo realizado para mover una carga depende únicamente de los puntos de salida y llegada, y es totalmente independiente del camino que elijas. Si no fuera así, el potencial no tendría un valor único y toda esta teoría no tendría sentido físico.