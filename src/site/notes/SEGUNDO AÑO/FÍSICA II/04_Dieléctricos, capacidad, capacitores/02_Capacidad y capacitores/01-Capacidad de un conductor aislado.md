---
{"dg-publish":true,"permalink":"/segundo-ano/fisica-ii/04-dielectricos-capacidad-capacitores/02-capacidad-y-capacitores/01-capacidad-de-un-conductor-aislado/","dgPassFrontmatter":true,"dg-note-properties":{}}
---

Tags: #capacidad #conductores #faradio

## 1. Definición matemática y unidades
Para cualquier conductor cargado, la carga ($q$) es proporcional a su potencial ($V$). Esta relación se define mediante una constante de proporcionalidad llamada capacidad:
$$q=C\cdot V \ \ \ \ \ \ \to \ \ \ \ \ \ C=\frac{q}{V}$$
Esta capacidad representa la razón entre la carga y el potencial. Se expresa en Coulomb por Volt ($C/V$), a esta unidad se la denomina *Faradio* ($F$), en honor al Michael Faraday.

Como el Faradio es una unidad gigantesca para la práctica común, solemos usar microfaradios ($\mu F$), nanofaradios ($nF$) o picofaradios ($pF$).

>[!tip] Concepto clave
>Es fundamental entender que la capacidad NO depende de la carga ($q$) ni del voltaje ($V$). Si duplicamos la carga de un conductor, su voltaje se duplicará automáticamente, pero su capacidad $C$ permanecerá constante. La capacidad es una propiedad intrínseca del diseño: depende de cuántos metros mide (geometría) y de qué material está rodeado.

---
## 2. Caso de la esfera conductora
Si tomamos una esfera metálica de radio $a$ en el vacío, sabemos que su potencial es:
$$V=\frac{1}{4\pi\epsilon_0}\frac{q}{a}$$
Al aplicar la definición de capacidad ($C=q/V$), obtenemos:
$$C=4\pi\epsilon_0a$$
>[!important] Conclusión geométrica
>La capacidad de una esfera aislada es directamente proporcional a su radio. Esto confirma que la capacidad es una propiedad puramente geométrica: cuanto más grande es el objetivo, más "espacio" tiene para que las cargas se distribuyan sin subir tanto el voltaje.

---
## 3. Rigidez dieléctrica
A diferencia de un recipiente de agua que tiene un volumen máximo fijo, un conductor podría (en teoría) recibir carga indefinidamente elevando su potencial. Sin embargo, el límite real lo impone el medio que lo rodea (generalmente el aire):
- Si seguimos agregando carga, el campo eléctrico en la superficie aumentará hasta superar la rigidez dieléctrica del aire ($3\cdot10^6V/m$)
- En ese punto, el aire se ioniza, se vuelve conductor y la carga se escapa en forma de chispa o corona.
