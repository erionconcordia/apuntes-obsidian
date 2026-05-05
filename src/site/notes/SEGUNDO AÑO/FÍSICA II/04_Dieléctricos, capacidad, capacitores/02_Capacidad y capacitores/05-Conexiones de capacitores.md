---
{"dg-publish":true,"permalink":"/segundo-ano/fisica-ii/04-dielectricos-capacidad-capacitores/02-capacidad-y-capacitores/05-conexiones-de-capacitores/","dgPassFrontmatter":true,"dg-note-properties":{}}
---

Tags: #redes #capacitores #capacidad-equivalente

## 1. Conexión en serie
Se dice que dos o más condensadores están en serie cuando se conectan uno a continuación del otro, ofreciendo una trayectoria única para la carga.

- La carga ($Q$): en una conexión en serie, la carga en todas las armaduras de todos los condensadores es exactamente la misma ($Q_1=Q_2=Q$). Esto ocurre porque el proceso de carga consiste en desplazar electrones de una placa a la siguiente a través del circuito.

- El voltaje ($V$): La diferencia de potencial total aplicada es la suma de las caídas de potencial en cada condensador ($V_{ab}=V_1+V_2+...$)

**Capacidad equivalente**
Aplicando la definición:
$$V=\frac{q}{C}$$
Se deduce que la inversa de la capacidad equivalente es igual a la suma de las inversas de las capacidades individuales:
$$\frac{1}{C_{eq}}=\frac{1}{C_1}+\frac{1}{C_2}+\frac{1}{C_3}+...$$
>[!warning] Efecto en el diseño
>Al conectar capacitores en serie, la capacidad total del conjunto es siempre menor que la del capacitor más pequeño del grupo. Se usa principalmente para repartir un alto voltaje entre varios componentes y evitar que uno solo llegue a su punto de ruptura dieléctrica.

---
## 2. Conexión en paralelo
En esta conexión, todas las armaduras positivas se unen a un punto y todas las negativas a otro, de modo que todos los condensadores están sometidas a la misma diferencia de potencial.

- El voltaje ($V$): La diferencia de potencial entre las armaduras de cada condensador es la misma ($V_{ab}$).
  
- La carga ($Q$): La carga total desplazada por la batería es la suma de las cargas almacenadas en cada capacitor ($Q=Q_1+Q_2+...$).

**Capacidad equivalente**
Se obtiene simplemente sumando los valores de cada capacidad:
$$C_{eq}=C_1+C_2+C_3+...$$
>[!success] Efecto en el diseño
>La conexión en paralelo se utiliza para aumentar la capacidad total de almacenamiento de energía de un sistema, manteniendo el mismo nivel de voltaje.

