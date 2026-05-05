---
{"dg-publish":true,"permalink":"/segundo-ano/probabilidad-y-estadistica/01-estadistica-descriptiva/05-medidas-de-forma/01-asimetria-skewness/","dgPassFrontmatter":true,"dg-note-properties":{}}
---

La asimetría evalúa si los datos se distribuyen de manera equilibrada a ambos lados del centro. Se dice que una distribución es simétrica si se puede doblar a lo largo de un eje vertical de manera que la mitad izquierda sea una imagen de espejo (coincida perfectamente) con la mitad derecha.

![Pasted image 20260423112401.png](/img/user/IM%C3%81GENES/Pasted%20image%2020260423112401.png)

Cuando una distribución carece de esta simetría, se dice que está **sesgada**. Existen dos tipos de sesgo que debemos identificar en el análisis:
- Sesgo a la derecha.
- Sesgo a la izquierda.

## Asimetría positiva (sesgo a la derecha)
Ocurre cuando la cola derecha (superior) del histograma o curva se alarga mucho más en comparación con la cola izquierda (inferior).

![Pasted image 20260423112351.png](/img/user/IM%C3%81GENES/Pasted%20image%2020260423112351.png)

Los valores extremos muy grandes (que forman la cola larga) "jalan" a la media aritmética $\bar{x}$ a la derecha, pero no afectan a la mediana $\tilde{x}$. Por lo tanto, en una distribución con asimetría positiva:
$$\text{Media }\bar{x}>\text{Mediana }\tilde{x}$$
**Ejemplo:** Los tiempos hasta la falla de un componente electrónico o los tiempos de reparación. Un componente no puede fallar en un tiempo menor a cero (límite izquierdo), pero ocasionalmente algunos componentes durarán muchísimo tiempo antes de fallar (cola derecha larga).

## Asimetría negativa (sesgo a la izquierda)
Ocurre cuando el alargamiento de la curva se da hacia la izquierda (valores menores).

![Pasted image 20260423112634.png](/img/user/IM%C3%81GENES/Pasted%20image%2020260423112634.png)

Los pocos valores extremadamente pequeños "jalan" el promedio hacia abajo, por lo tanto:
$$\text{Media }\bar{x}<\text{Mediana }\tilde{x}$$
**Ejemplo:** La calificación de un examen sumamente fácil. La mayoría de los estudiantes sacará notas altas (amontonamiento a la derecha), pero unos pocos sacarán notas muy bajas, creando una cola larga hacia la izquierda.

>[!dato] Relación con el Boxplot
>Como vimos en la sección de **Medidas de posición**, el diagrama de caja es excelente para detectar esto: si la caja o el bigote derecho son mucho más grandes que los de la izquierda, hay asimetría positiva.

