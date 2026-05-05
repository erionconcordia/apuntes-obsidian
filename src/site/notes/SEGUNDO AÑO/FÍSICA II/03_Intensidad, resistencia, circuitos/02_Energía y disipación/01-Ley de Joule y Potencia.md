---
{"dg-publish":true,"permalink":"/segundo-ano/fisica-ii/03-intensidad-resistencia-circuitos/02-energia-y-disipacion/01-ley-de-joule-y-potencia/","dgPassFrontmatter":true,"dg-note-properties":{}}
---

Tags: #electrodinámica #potencia #joule #calor

## 1. El origen microscópico del calor
Aunque solemos imaginar que los electrones libres viajan por un cable a una velocidad media constante, su viaje real es muy caótico. El campo eléctrico los acelera, pero enseguida chocan contra las partículas fijas de la red cristalina del conductor, frenándose en seco.

En cada uno de estos choques, los electrones ceden a las partículas fijas la energía cinética que acaban de ganar. Esta energía adquirida por las partículas fijas aumenta su amplitud de vibración térmica, lo que a nivel macroscópico nosotros experimentamos sencillamente como un aumento de temperatura (calor).

---
## 2. Potencia eléctrica ($P$)
(*Conexión con [[SEGUNDO AÑO/ELECTROTECNIA I/01_Introducción/01_Conceptos/07-Potencia y energía\|07-Potencia y energía]] de Electrotecnia I*) Para deducir la cantidad de energía que consume o suministra cualquier dispositivo, analizamos el trabajo que realiza la carga. Si una cantidad de carga $dq$ entra por un borne $a$ a un potencial $V_a$ y sale por el borne $b$ a un potencial $V_b$, entonces ha transportado energía. La energía cedida por esa carga ($dW$) es:
$$dW=dq\cdot(V_a-V_b)=dq\cdot V_{ab}$$
La rapidez con la que se transforma esa energía (energía por unidad de tiempo) se llama Potencia ($P$). Dividiendo la ecuación por el tiempo $dt$, y recordando que la intensidad es $i=dq/dt$, obtenemos la fórmula general de la potencia eléctrica:
$$P=\frac{dW}{dt}=i\cdot V_{ab}$$
>[!important] Unidades: El Watt
>Si la corriente $i$ se mide en Amperes ($Coulomb/segundo$) y el voltaje $V_{ab}$ se mide en Volts ($Joule/Coulomb$), la Potencia resulta medida en Joule por segundo, lo que se denomina Watt ($W$). Esta ecuación:
>$$P=i\cdot V$$
>es universal y se aplica a cualquier elemento (resistencias, motores, baterías, etc.).

---
## 3. Ley de Joule
![Pasted image 20260502193421.png](/img/user/IM%C3%81GENES/Pasted%20image%2020260502193421.png)
*¿Qué pasa cuando la "caja" anterior es una resistencia pura?* En ese caso, toda la energía eléctrica suministrada se convierte irreversiblemente en calor. Si el material cumple con la Ley de Ohm, podemos sustituir el voltaje en nuestra fórmula de potencia:
$$P=i\cdot(i\cdot R)$$
$$P=i^2\cdot R$$
Esta ecuación expresa que la cantidad de calor producida por unidad de tiempo es igual al producto del cuadrado de la corriente por la resistencia. Esto es la Ley de Joule.

>[!dato] Detalle teórico
>Al igual que la Ley de Ohm, la Ley de Joule no es una ley general de la materia, sino una cualidad especial de ciertas sustancias conductoras (como los metales). Si el material cumple a Ohm, cumple necesariamente a Joule.

