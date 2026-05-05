---
{"dg-publish":true,"permalink":"/segundo-ano/fisica-ii/03-intensidad-resistencia-circuitos/01-conceptos/01-intensidad-y-densidad-de-corriente/","dgPassFrontmatter":true,"dg-note-properties":{}}
---

Tags: #electrodinámica #corriente #intensidad #amper 

## 1. El movimiento de las cargas
Un conductor es un cuerpo que posee cargas libres en su interior (en los metales son electrones negativos, en los electrolitos son iones positivos y negativos). Si conectamos los extremos de un cable de cobre a los bornes de una batería de 12 V, establecemos un campo eléctrico dentro del hilo.

Bajo la influencia de este campo, los electrones libres sienten una fuerza en sentido opuesto al campo y aceleran. Sin embargo, no aceleran infinitamente: chocan continuamente contra las partículas fijas del metal, se frenan y vuelven a acelerar. Este proceso hace que, en conjunto adquieran una velocidad media constante avanzando por el cable.

>[!informacion] Tipos de corriente
>- **Continua:** Si el campo eléctrico tiene siempre el mismo sentido, la corriente fluye en una sola dirección.
>- **Alterna:** Si el campo se invierte periódicamente (como en los enchufes de casa), el flujo de carga cambia de sentido constantemente.

---
## 2. Intensidad de corriente ($i$)
Si cortamos imaginariamente l cable y nos ponemos a contar cuánta carga cruza esa sección transversal en un intervalo de tiempo $dt$, obtenemos la intensidad.

![Pasted image 20260502190037.png](/img/user/IM%C3%81GENES/Pasted%20image%2020260502190037.png)

La cantidad de carga que atraviesa una sección de hilo por unidad de tiempo ($dq/dt$) se denomina intensidad de corriente ($i$):
$$i=\frac{dq}{dt}$$
- **Deducción matemática:** Si en un volumen del cable hay $n$ electrones libres, cada uno con carga $e$, moviéndose a una velocidad media $v$ a través de un área transversal $A$, la intensidad exacta será $i=n\cdot e\cdot v\cdot A$.
- **Unidad en el SI:** Al dividir la carga por tiempo, obtenemos Coulomb por segundo. A esta unidad se la bautizó **Ampere (A)**.

---
## 3. Densidad de corriente ($J$)
A diferencia de la electroestática donde el exceso de carga se iba a la superficie del conductor, cuando hay una corriente eléctrica circulando, los electrones libres fluyen y se distribuyen por toda el área de la sección transversal del hilo.

Para saber qué tan "concentrado" está ese flujo, definimos la densidad de corriente ($J$) como la razón entre la intensidad de la corriente y la sección transversal ($A$):
$$J=\frac{i}{A}$$
---
## 4. El convenio de signos y el circuito cerrado

>[!warning] La trampa del sentido de la corriente
>En un metal, sabemos que los que realmente se mueven son los electrones (cargas negativas) viajando de menos a más potencial. Sin embargo, por una convención histórica universal, el sentido de la corriente se considera siempre como si las cargas que se movieran fueran exclusivamente positivas. Por lo tanto, en nuestros diagramas, la flecha de la intensidad de corriente $(i)$ siempre apunta en sentido opuesto al movimiento real de los electrones.

![Pasted image 20260502190730.png](/img/user/IM%C3%81GENES/Pasted%20image%2020260502190730.png)

Para que esta corriente exista de manera permanente, la trayectoria debe ser un circuito completo o cerrado. La intensidad de corriente tiene que ser exactamente la misma en todas las secciones del circuito (incluyendo por dentro de la batería); si el circuito se interrumpe (circuito abierto), la corriente cesa inmediatamente en todas partes.
