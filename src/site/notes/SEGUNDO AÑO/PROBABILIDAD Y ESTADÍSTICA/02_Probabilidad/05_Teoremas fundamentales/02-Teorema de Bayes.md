---
{"dg-publish":true,"permalink":"/segundo-ano/probabilidad-y-estadistica/02-probabilidad/05-teoremas-fundamentales/02-teorema-de-bayes/","dgPassFrontmatter":true,"dg-note-properties":{}}
---

Tags: #probabilidad #teorema_de_bayes

>[!informacion] Vinculación
>Este teorema es la culminación de la [[SEGUNDO AÑO/PROBABILIDAD Y ESTADÍSTICA/02_Probabilidad/04_Prob. condicional e independencia/01-Probabilidad condicional\|01-Probabilidad condicional]]. Nos permite resolver problemas complejos dividiéndolos en partes más pequeñas y manejables.

---
## El requisito previo: Participación de un espacio muestral
Para poder aplicar la **Ley de la Probabilidad Total** (o el **Teorema de Bayes** más adelante), primero debemos entender cómo dividir nuestro espacio muestral $\ohm$ de forma correcta.

Se dice que un conjunto de eventos $\{B_1,B_2,...,B_n\}$ constituye una partición del espacio muestral si cumplen dos reglas estrictas:
1. **Son mutuamente excluyentes:** No pueden ocurrir al mismo tiempo.
2. **Son exhaustivos:** Entre todos cubren la totalidad de los resultados posibles del experimento (su unión es igual a $\ohm$).

---
# Teorema de Bayes
Mientras que la probabilidad total averigua la posibilidad de un "efecto" final (ej. pieza defectuosa), el **Teorema de Bayes** hace el camino inverso: si ya sabemos que el "efecto" ocurrió, calcula la probabilidad de que haya sido provocado por una "causa" o escenario específico.

En estadística bayesiana, la probabilidad el escenario $B_j$ antes de hacer el experimento se llama probabilidad previa, y la probabilidad recalculada tras conocer la nueva evidencia $A$ se llama probabilidad posterior.

>[!definicion] Teorema de Bayes
>Sea $\{B_1,B_2,...,B_n\}$ una partición de $\ohm$. Si $A$ es un evento cualquiera que ya ocurrió, la probabilidad de que provenga de la partición $B_j$ es:
>$$
>P(B_j/A)=\frac{P(B_j)\cdot P(A/B_j)}{\sum_{i=1}^nP(B_i)\cdot P(A/B_i)}=\frac{P(B_j)\cdot P(A/B_j)}{P(A)}
>$$

>[!observacion] Nota
>El denominador es, ni más ni menos, que la fórmula de la Probabilidad Total.

**Ejemplo:** Una planta de ensamble recibe productos provenientes de tres fabricantes A, B y C. El 50% del total se compra a A, mientras que a B y C se le compran el resto en partes iguales. El porcentaje de productos defectuosos para A, B y C, es de 5, 10 y 12% respectivamente. Determine la probabilidad de que una unidad ensamblada tenga un componente malo. Si se toma al azar un componente y se encuentra que es defectuoso:

1. ¿Cuál es la probabilidad de que haya sido vendido por el proveedor B?
- Numerador (Intersección $B\cap D$): $P(B)\cdot P(D/B)=0.25\cdot 0.10=0.025$
- Denominador (Probabilidad total D): $0.08$.
$$
P(B/D)=\frac{0.025}{0.08}=0.3125
$$
1. ¿Y que no haya sido comprado por A?
$$P(A^c/D)=1-P(A/D)$$
$$
P(A/D)=\frac{P(A)\cdot P(D/A)}{P(D)}=\frac{0.50\cdot 0.05}{0.08}=\frac{0.025}{0.08}=0.3125
$$
$$
P(A^c/D)=1-0.3125=0.6875
$$

>[!important] Estrategia (Causa vs. Efecto)
>Al leer un ejercicio, la clave para saber qué teorema usar es identificar qué información nos dan como "hecho" o "condición":
>- Si nos piden la probabilidad del evento final (ej. "¿Cuál es la probabilidad de que una pieza seleccionada esté rota?) $\to$ **Probabilidad Total**
>- Si nos dicen que el evento final ya se comprobó y nos preguntan de dónde provino (ej. "Se extrae una pieza, se constata que está rota... ¿Qué probabilidad hay de que sea de la máquina 2?") $\to$ **Teorema de Bayes**.



