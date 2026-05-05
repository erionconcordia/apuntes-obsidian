---
{"dg-publish":true,"permalink":"/segundo-ano/fisica-ii/03-intensidad-resistencia-circuitos/04-analisis-de-redes/02-redes-complejas-y-reglas-de-kirchhoff/","dgPassFrontmatter":true,"dg-note-properties":{}}
---

Tags: #electrodinámica #circuitos #kirchoff #redes 

## 1. Nodos y mallas
(*Conexión directa con [[SEGUNDO AÑO/ELECTROTECNIA I/01_Introducción/01_Conceptos/10-Nodos, ramas y lazos\|10-Nodos, ramas y lazos]] de ELECTROTECNIA I*). Antes de aplicar las reglas, necesitamos definir exactamente cómo está construido nuestro circuito:
- **Nodo:** Es un punto de la red eléctrica en el cual se unen tres (o más conductores). Es decir, es una bifurcación real donde la corriente tiene la opción de dividirse.
- **Malla:** Es cualquier recorrido conductor que sea completamente cerrado. Un circuito complejo puede imaginarse como un rompecabezas formado por varias mallas pequeñas que comparten cables.

---
## 2. Regla de los nodos
Esta regla se aplica a las bifurcaciones y establece que: la suma algebraica de las intensidades de las corrientes que se dirigen a cualquier nodo de la red es estrictamente cero.
$$\sum i=0$$
**Sentido físico**
Esta regla expresa simplemente que la carga eléctrica no se acumula ni se "amontona" mágicamente en ninguna intersección de la red. Toda la carga que entra, tiene que salir.

**Convenio de signos**
Para armar la ecuación matemática, se considera positiva ($+$) la intensidad de una corriente si se dirige hacia el nodo, y negativa ($-$) si se aleja del mismo.

---
## 3. Regla de las mallas
Esta regla se aplica a los recorridos cerrados y establece que: la suma algebraica de las fuerzas electromotrices en una malla cualquiera es exactamente igual a la suma algebraica de las caídas de potencial en esa misma malla.
$$\sum \epsilon=\sum(i\cdot R)$$**Sentido físico**
Si das una vuelta completa a una malla y vuelves exactamente al mismo punto de partida, la diferencia de potencial neta que subiste (baterías) y bajaste (resistencias) tiene que ser cero.

**Convenio de signos**
Se elige arbitrariamente un sentido de giro para analizar la malla (como las agujas del reloj). Las corrientes y FEM que "empujen" en ese sentido elegido serán positivas, y las que vayan en contra, negativas.
