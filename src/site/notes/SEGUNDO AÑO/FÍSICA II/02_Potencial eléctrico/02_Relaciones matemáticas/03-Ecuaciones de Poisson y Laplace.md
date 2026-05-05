---
{"dg-publish":true,"permalink":"/segundo-ano/fisica-ii/02-potencial-electrico/02-relaciones-matematicas/03-ecuaciones-de-poisson-y-laplace/","dgPassFrontmatter":true,"dg-note-properties":{}}
---

Tags: #potencial #poisson #laplace #matemática 

>[!abstract] Resumen
>Las ecuaciones de Poisson y Laplace son las herramientas matemáticas definitivas para resolver problemas de electroestática en el espacio tridimensional. Nos permiten relacionar directamente cómo cambia la "pendiente" del potencial eléctrico (su derivada segunda) en un punto del espacio con la cantidad de carga volumétrica que existe exactamente en ese punto.

## 1. El problema de la carga espacial
Imaginemos dos placas paralelas conductoras ($A$ y $B$) con un campo eléctrico dirigido de $A$ hacia $B$. Normalmente, entre las placas no hay nada. Pero, *¿qué pasa si el espacio entre ellas está lleno de una "nube" de cargas distribuidas uniformemente?* A esto se le llama carga espacial, y se representa con la densidad volumétrica de carga $\rho$ (carga por unidad de volumen).

![Pasted image 20260502170613.png\|430](/img/user/IM%C3%81GENES/Pasted%20image%2020260502170613.png)

Si analizamos un pequeño "espesor" $\Delta x$ de esta nube de área $A$, el campo eléctrico en la cara izquierda será $E$, pero en la cara derecha el campo será un poco más fuerte ($E+\Delta E$) porque la propia nube de carga aporta nuevas líneas de fuerza.

Aplicando el [[SEGUNDO AÑO/FÍSICA II/01_Ley de Coulomb y campo eléctrico/03_Leyes y teoremas/02-Teorema de Gauss\|02-Teorema de Gauss]] a este volumen elemental:
- Flujo neto saliente: *La diferencia entre el campo que sale y el que entra multiplicada por el área: $\Delta E\cdot A$.*
- Carga encerrada: *La densidad por el volumen: $\rho\cdot A\cdot\Delta x$.*

Igualando ambas partes (y dividiendo por $\epsilon_0$):
$$\Delta E\cdot A=\frac{\rho\cdot A\cdot\Delta x}{\epsilon_0}$$
Simplificando el área $A$ y pasando $\Delta x$ dividiendo, obtenemos la variación del campo respecto a la distancia:
$$\frac{dE}{dx}=\frac{\rho}{\epsilon_0}$$
---
## 2. Ecuación de Poisson
Aquí es donde conectamos con [[SEGUNDO AÑO/FÍSICA II/02_Potencial eléctrico/02_Relaciones matemáticas/02-Gradiente de potencial\|02-Gradiente de potencial]]. Sabemos que el campo eléctrico es el gradiente de potencial cambiado de signo: $E=-\frac{dV}{dx}$. Si derivamos esta expresión nuevamente respecto a $x$, tenemos que la derivada del campo es igual a la derivada segunda del potencial:
$$\frac{dE}{dx}=-\frac{d^2V}{dx^2}$$
Sustituyendo esto en la ecuación que obtuvimos con Gauss, llegamos a la Ecuación de Poisson *en una dimensión*:
$$\frac{d^2V}{dx^2}=-\frac{\rho}{\epsilon_0}$$

>[!important] Generalización a 3D
>Como el espacio real tiene tres dimensiones, el potencial $V$ depende de las coordenadas ($x,y,z$). La ecuación completa de Poisson se escribe sumando las derivadas parciales segundas en los tres ejes:
>$$\frac{\partial^2V}{\partial x^2}+\frac{\partial^2V}{\partial y^2}+\frac{\partial^2V}{\partial z^2}=-\frac{\rho}{\epsilon_0}$$

---
## 3. Ecuación de Laplace
Existe un caso particular muchísimo más común en los problemas de ingeniería: *¿Qué pasa si en la región del espacio que estábamos analizando no hay carga espacial ($\rho=0$)?* Si la densidad de carga es nula, el término de la derecha desaparece, y la ecuación de Poisson se reduce instantáneamente a la Ecuación de Laplace:
$$\frac{\partial^2V}{\partial x^2}+\frac{\partial^2V}{\partial y^2}+\frac{\partial^2V}{\partial z^2}=0$$

>[!informacion] Utilidad práctica
>Un campo eléctrico queda completamente determinado si conocemos su potencial en todos los puntos. Si resolvemos esta ecuación diferencial (sabiendo los voltajes de los bordes o condiciones de contorno), podemos mapear todo el potencial del espacio, y luego derivarlo para encontrar el campo $E$ con el gradiente.

