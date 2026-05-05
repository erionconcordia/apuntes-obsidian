---
{"dg-publish":true,"permalink":"/segundo-ano/probabilidad-y-estadistica/01-estadistica-descriptiva/03-descripcion-de-un-conjunto-de-datos/05-histogramas/","dgPassFrontmatter":true,"dg-note-properties":{}}
---

Tags: #estadística_descriptiva #representaciones_gráficas #histograma 

## 1. ¿Qué es y para qué sirve?
Un histograma es la representación gráfica por excelencia para resumir y visualizar datos numéricos (cuantitativos), especialmente cuando la variable es continua (como mediciones físicas: resistencia, peso, tiempo, etc.) o cuando hay muchos datos discretos agrupados.

**¿Para qué sirve en la práctica?**
Permite ver de un vistazo cómo se distribuyen los datos en la realidad (su forma, su centro y su grado de dispersión).

A medida que el tamaño de la muestra aumenta, los intervalos se hacen más estrechos, el contorno del histograma se aproxima a la curva suave de la verdadera distribución de probabilidad de la población.

En ingeniería, sirve para ver rápidamente qué porcentaje de la producción cae dentro o fuera de los límites de especificación aceptables.

---
## 2. Anatomía del histograma
A diferencia de un gráfico de barras (que separa categorías cualitativas), en un histograma los rectángulos están pegados unos a otros, reflejando la naturaleza continua de la línea de números.
![Pasted image 20260422110849.png\|336](/img/user/IM%C3%81GENES/Pasted%20image%2020260422110849.png)

El histograma se compone de las siguientes partes:

**1. Eje horizontal ($X$):** Representa la escala de medición de la variable. Se divide en intervalos de clase (o "bins") que abarcan todo el rango de los datos sin traslaparse.

**2. Eje vertical ($Y$):** Dependiendo de cómo se construya, puede representar:
- Frecuencia absoluta ($f_i$): *El conteo exacto de cuántas observaciones cayeron en ese intervalo.*
- Frecuencia relativa ($f_r$): La proporción o porcentaje de datos en el intervalo ($f_i/n$).
- Densidad: *Se usa cuando los intervalos no tienen el mismo ancho.*

**3. El área de los rectángulos:** En estadística, el área de cada rectángulo es directamente proporcional a la frecuencia relativa de las observaciones en ese intervalo.

---
## 3. ¿Cómo construirlo?
Para agrupar los datos continuos, se debe decidir cuántas clases usar. No hay reglas inquebrantables, pero en general, se recomienda usar entre 5 y 20 clases.
- **Regla empírica para el número de clases:** Una buena estimación inicial es usar la raíz cuadrada del número total de observaciones ($n$).
$$\text{Número de clases}\approx\sqrt{n}$$
![Pasted image 20260422111423.png](/img/user/IM%C3%81GENES/Pasted%20image%2020260422111423.png)

**Manejo de los anchos de clase**
1. **Anchos iguales:** Es el caso más común. Se divide el rango de los datos en partes iguales y la altura del rectángulo es simplemente la frecuencia absoluta o frecuencia relativa.
2. **Anchos desiguales (escala de densidad):** Si los datos tienen una "cola" muy larga (valores extremos muy separados), usar anchos iguales dejará muchas clases vacías. Es mejor agrupar los extremos en clases más anchas. Pero **¡cuidado!**, si hacemos esto, la altura ya no puede ser la frecuencia porque el gráfico se distorsionará. Debemos usar la **densidad**:
$$\text{Altura del rectángulo (Densidad)}=\frac{\text{Frecuencia relativa de la clase}}{\text{Ancho de clase}}$$
---
## 4. Interpretación de formas comunes
El valor real del histograma está en diagnosticar el comportamiento del fenómeno que estás estudiando al observar su silueta:
- **Simétrico (forma de campana):** La mitad izquierda es una imagen espejo de la derecha. Sugiere fuertemente una distribución normal, indicando que el proceso está bajo control y variando naturalmente alrededor de un valor central.
- **Sesgado positivamente (asimetría hacia la derecha):** La "cola" de los datos se alarga hacia los valores altos. Muy común en ingeniería en variables como tiempos de falla o tiempos de reparación, donde el tiempo no puede ser menor a 0 pero puede alargarse indefinidamente.
- **Sesgado negativamente (asimetría hacia al izquierda):** La "cola" se alarga hacia los valores bajos.
- **Bimodal (dos crestas distintas):** ¡Alerta de ingeniería! Un histograma bimodal casi siempre indica que tus datos mezclan dos poblaciones diferentes. Por ejemplo: componentes que vienen de dos proveedores distintos, mediciones hechas por dos operadores diferentes, o dos rutas de viaje distintas.
