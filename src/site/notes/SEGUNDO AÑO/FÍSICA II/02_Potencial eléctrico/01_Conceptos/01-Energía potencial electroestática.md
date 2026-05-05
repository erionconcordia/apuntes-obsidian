---
{"dg-publish":true,"permalink":"/segundo-ano/fisica-ii/02-potencial-electrico/01-conceptos/01-energia-potencial-electroestatica/","dgPassFrontmatter":true,"dg-note-properties":{}}
---

Tags: #potencial #energía #trabajo

## 1. El trabajo en un campo eléctrico
Imaginemos un campo eléctrico y una línea que representa una trayectoria de forma arbitraria entre dos puntos, $A$ y $B$. Si colocamos una carga positiva de prueba $q'$ en ese campo, experimentará una fuerza eléctrica dada por el vector $F=q'\cdot E$.

![Pasted image 20260502155001.png\|346](/img/user/IM%C3%81GENES/Pasted%20image%2020260502155001.png)

Para mover esa carga desde $A$ hasta $B$, habrá que realizar un esfuerzo. Si descomponemos la fuerza eléctrica en una componente tangencial y otra normal a la trayectoria, es el componente tangencial la que realiza trabajo (o contra la cual nosotros realizamos trabajo) a lo largo del desplazamiento $ds$.

---
## 2. Acerca de la demostración matemática
Aplicando la [[PRIMER AÑO/FÍSICA I/03_Dinámica/03_Leyes_y_condiciones/01-2da Ley de Newton\|01-2da Ley de Newton]] y analizando el aumento de energía cinética, la teoría nos demuestra que el trabajo realizado contra la fuerza eléctrica del campo para mover la carga se expresa mediante una integral curvilínea.

>[!warning] Significado del signo negativo
>La expresión matemática del incremento de energía potencial es:
>$$EP_b-EP_a=-\int_a^bq'\cdot E\cdot\cos(\theta)\cdot ds$$
>El signo negativo es crucial: *significa que se ha realizado trabajo contra las fuerzas eléctricas. Es análogo a empujar algo "cuesta arriba"*.

Si la única fuerza que actúa sobre la carga es la del propio campo eléctrico (no hay fuerzas exteriores empujando), la suma de las energías cinética y potencial de la carga se mantiene constante en todos los puntos de la trayectoria ($EC_a+EP_a=EC_b+EP_b$).

---
## 3. El infinito como punto de referencia
Para poder hablar de la energía potencial en un punto específico (y no solo de "diferencias" entre dos puntos), necesitamos establecer un punto de referencia arbitrario donde la energía potencial sea cero, tal como hacemos con el nivel del piso para la gravedad.

Para que las matemáticas sean más sencillas, se elige convencionalmente el infinito como punto de referencia. Suponemos que la energía potencial es nula cuando la carga está infinitamente alejada de las otras cargas que crean el campo.

Por lo tanto, la energía potencial ($EP$) de una carga en un punto cualquiera se define como el trabajo realizado contra el campo para traer dicha carga desde el infinito hasta ese punto.
$$EP=-\int_\infty^bq'\cdot E\cdot\cos(\theta)\cdot ds$$
