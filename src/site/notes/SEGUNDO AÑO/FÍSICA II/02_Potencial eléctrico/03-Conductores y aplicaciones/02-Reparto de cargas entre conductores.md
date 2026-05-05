---
{"dg-publish":true,"permalink":"/segundo-ano/fisica-ii/02-potencial-electrico/03-conductores-y-aplicaciones/02-reparto-de-cargas-entre-conductores/","dgPassFrontmatter":true,"dg-note-properties":{}}
---

Tags: #potencial #conductores #magia-electroestática

## 1. Contacto externo (dos esferas unidas por un cable)
Imaginemos dos esferas conductora, una pequeña $A$ (ej. 1 cm de radio) y una grande $B$ (ej. 10 cm de radio), separados por una distancia enorme en comparación con sus radios y conectadas por un hilo metálico muy fino. Si le damos una carga al sistema, la misma se repartirá de forma que ambas esferas igualan su potencial ($V_A=V_B$).

Para este caso se deducen dos conclusiones vitales:
**1. La carga prefiere el tamaño:**
Al igualar potenciales, la esfera más grande ($B$) se queda con la inmensa mayoría de la carga total del sistema ($q_B>q_A$).

**2. La densidad prefiere las puntas:**
Aunque la esfera pequeña ($A$) tiene poca carga total, el espacio para distribuirla es tan diminuto que su densidad superficial de carga ($\sigma$) es muchísimo mayor que en la esfera grande.

---
## 2. Contacto interno (La base del Van de Graff)
Imaginemos que la esfera grande $B$ es hueca y tiene un pequeño orificio. Introducimos la esfera pequeña $A$ por ese orificio y la situamos exactamente en el centro del espacio hueco de $B$.

Calculemos analíticamente la diferencia de potencial ($V_{AB}$) entre la esfera interior $A$ y la exterior hueca $B$. Como el campo eléctrico aportado por la esfera exterior $B$ es nulo en su propio interior, la diferencia topográfica de potencial depende únicamente de la carga de la esfera central $A$. La ecuación resulta:
$$V_{AB}=\frac{1}{4\pi\epsilon_0}\cdot q_A\cdot\left(\frac{1}{radio_A}-\frac{1}{radio_B}\right)$$
Como el radio de $A$ es menor que el de $B$, la fracción del paréntesis es siempre positiva. Por lo tanto, siempre que $A$ tenga una carga positiva, se encontrará a un potencial estrictamente superior al de la esfera envolvente $B$.

>[!warning] El traspaso total
>Si ahora tomamos un cable y conectamos la esfera interna $A$ con la pared interna de la esfera hueca $B$ (o simplemente hacemos que se toquen), la carga fluirá de la zona de alto potencial hacia la de bajo potencial hasta que $V_{AB}=0$. Pero según nuestra ecuación, la única forma matemática de que $V_{AB}=0$ es que $q_A=0$.
>
>*Conclusión inesperada:* Toda la carga de la esfera interna se transmite por completo a la esfera exterior, independientemente de los valores iniciales de carga y potencial que ya tuviera la esfera grande.

