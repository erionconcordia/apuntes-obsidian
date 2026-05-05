---
{"dg-publish":true,"permalink":"/segundo-ano/probabilidad-y-estadistica/02-probabilidad/02-conceptos-basicos/02-espacio-muestral/","dgPassFrontmatter":true,"dg-note-properties":{}}
---

Tags: #probabilidad #espacio_muestral

## Espacio muestral ($\ohm$ o $S$)
Una vez que sabemos que un resultado es aleatorio, necesitamos "cercar" o definir cuáles son todos esos resultados posibles.

>[!definicion] Definición: Espacio muestral
>Es el conjunto formado por absolutamente todos los posibles resultados de un experimento aleatorio.

>[!warning] Diferencia de notación
>En clases, denotamos el espacio muestral con la letra griega $\ohm$. Sin embargo, en los libros como el Devore o el Walpole, se denota el espacio muestral con la letra $S$.

A cada resultado individual dentro del espacio muestral se le llama elemento o punto muestral. Existen diferentes formas de describir un espacio muestral dependiendo de su coplejidad:

**1. Por enumeración (Lista)**
Separando los elementos por comas entre llaves.
- Ej. Al lanzar un dado: $\ohm=$ {$1,2,3,4,5,6$}.

**2. Método de la regla**
Definiendo una propiedad matemática.
- Ej. El tiempo de vida $t$ de un componente: $\ohm=$ {$t|t\geq0$}

**3. Diagramas de árbol**
*(Desarrollado en [[SEGUNDO AÑO/PROBABILIDAD Y ESTADÍSTICA/02_Probabilidad/01_Fundamentos matemáticos/03-Técnicas de conteo\|03-Técnicas de conteo]])* Es una excelente herramienta visual de ramificación para listar de forma sistemática espacios muestrales en experimentos que ocurren en múltiples etapas.
- Ej. Lanzar una moneda 3 veces.

---
## Tipos de espacios muestrales
Reconocer el tipo de espacio muestral ayuda a la forma del cálculo de la probabilidad. Se dividen en tres grandes grupos:

**A. Discretos finitos**
Tienen un número limitado (finito) y contable de puntos muestrales.
- *Ejemplo:* Si inspeccionamos 3 artículos y los clasificamos como Normales (N) o Defectuosos (D), el espacio tiene exactamente 8 elementos: $\ohm=$ {$NNN,NND,NDN,DNN,NDD,DND,DDN,DDD$}.

**B. Discretos infinitos**
Tienen una cantidad de elementos que nunca termina, pero que aún se pueden contar o poner en una lista secuencial (hay un primero, un segundo, un tercero...)
- *Ejemplo:* Arrojar un dado repetidamente **hasta** obtener un cuatro. Podríamos obtenerlo en el 1° intento, en el 2°, en el 1000° o en el intento millón. La secuencia no tiene fin: $\ohm=$ {$E,FE,FFE,FFFE,...$} donde $E$ es el éxito y $F$ es falla.

**C. Continuos**
Contienen un número infinito de posibilidades que equivale al número de puntos en un segmento de recta, imposibles de enumerar individualmente. Ocurren siempre que el experimento implica medir magnitudes físicas en lugar de contar.
- *Ejemplo:* Registrar la vida útil de un objeto en horas, o la cantidad de precipitado y el volumen de un gas liberado en una reacción química. Sus probabilidades requerirán del uso del cálculo integral.
