---
{"dg-publish":true,"permalink":"/primer-ano/fisica-i/04-trabajo-y-energia/04-conceptos/06-energia-potencial/","dgPassFrontmatter":true,"dg-note-properties":{}}
---

La energía potencial se define como la capacidad que tiene un cuerpo o sistema de realizar trabajo debido a su posición dentro de un campo de fuerzas. Su principal característica es que no depende del movimiento del cuerpo, sino que de su posición, y solo tiene sentido en presencia de fuerzas conservativas, aquellas cuyo trabajo no depende del camino seguido, solo del punto inicial y final.

Existen dos tipos de energía potencial:
1. Energía potencial gravitatoria $(U_g)$.
2. Energía potencial elástica $(U_e)$.

### 1. ENERGÍA POTENCIAL GRAVITATORIA
Es una forma de energía que depende de la posición de un cuerpo con respecto a un sistema de referencia. Es decir, es aquel tipo de energía que posee un cuerpo debido a la altura a la que se encuentra, con respecto al plano de referencia horizontal, considerado como arbitrario.
$$
U_g=mgh
$$
Para obtener esta expresión, definimos el trabajo sobre el cuerpo:
$$W_{grav}=\vec{F}\cdot s \ \ \ (1)$$
Recordamos la [[PRIMER AÑO/FÍSICA I/03_Dinámica/03_Leyes_y_condiciones/01-2da Ley de Newton\|01-2da Ley de Newton]] para armar la segunda expresión:
$$\vec{F}=m\cdot\vec{a}=m\cdot\vec{g} \ \ \ (2)$$
Por lo tanto, reemplazando la expresión $(2)$ en la $(1)$ y, teniendo en cuenta que la posición $s=h$ varía con respecto a la altura, obtenemos:
$$W_{grav}=m\cdot\vec{g}\cdot(y_2-y_1)$$
$$W_{grav}=m\cdot\vec{g}\cdot y_2 - m\cdot\vec{g}\cdot y_1$$
Por lo tanto, definimos la energía potencial gravitatoria como:
$$U_g=m\cdot\vec{g}\cdot h$$
### 2. ENERGÍA POTENCIAL ELÁSTICA
Es la energía almacenada en un cuerpo elástico cuando se lo deforma (ya sea estirándolo o comprimiéndolo) dentro de su límite elástico.
$$U_e=\frac{1}{2}kx^2$$
>[!importante]
>Un concepto importante es el de **fuerza variable**.
>Una fuerza variable es una fuerza cuya magnitud y/o dirección cambia con el tiempo o con la posición del cuerpo sobre el que actúa.

Si la fuerza sobre un cuerpo es **variable** en vez de **constante**, como lo es en el ejemplo de un resorte:
$$F=k\cdot x$$
Entonces, podemos deducir la fórmula de la energía potencial elástica de la siguiente forma:

Tenemos en cuenta que para estirar un resorte se realiza trabajo, por lo que:
$$W=\int_0^xF \ dx$$
$$W=\int_0^xk\cdot x \ dx$$
$$W=\frac{1}{2}kx^2 \ \ \ \to \ \ \ U_e=\frac{1}{2}kx^2$$
