---
{"dg-publish":true,"permalink":"/segundo-ano/probabilidad-y-estadistica/02-probabilidad/03-enfoques-y-axiomas/02-enfoque-frecuencial/","dgPassFrontmatter":true,"dg-note-properties":{}}
---

Tags: #probabilidad #enfoque_frecuencial #frecuencia_relativa #probabilidad_objetiva

>[!observacion]
>El **enfoque clásico** que vimos anteriormente colapsa cuando los resultados no son equiprobables (ej. un dado cargado, o una máquina que produce más piezas buenas que malas). Para resolver estos problemas reales de ingeniería, dependemos de la experimentación empírica a través del enfoque frecuencial.

---
# 1. Fundamento matemático y teórico
El enfoque frecuencial frecuencial no se basa únicamente en la intuición, sino que está sustentado por teoremas de convergencia en estadística, específicamente la Ley de los Grandes Números.

Para que este enfoque sea válido, un experimento debe cumplir con dos condiciones inquebrantables:
1. Debe poder repetirse $n$ veces bajo condiciones idénticas.
2. Cada repetición debe ser estrictamente independiente de las demás (el resultado de un ensayo no afecta al siguiente).

Si definimos la frecuencia relativa $f_{ra}$ de un evento $A$ como el cociente entre l número de veces que ocurrió el evento $n_A$ y el número total de ensayos $n$:
$$f_{ra}=\frac{n_A}{n}$$
La **Ley de los Grandes Números (LGN)** demuestra que, aunque para valores pequeños de $n$ la frecuencia relativa $f_{ra}$ fluctúa de manera impredecible debido al azar, a medida que $n$ crece y tiende al infinito, la frecuencia relativa deja de fluctuar y converge hacia una constante fija.

---
# 2. La fórmula frecuencial
La interpretación objetiva de la probabilidad identifica una constante de estabilización matemática directamente con la probabilidad del evento A.

La definición matemática formal que sustenta este enfoque es el cálculo del límite cuando los ensayos tienden al infinito:
$$\lim_{n\to\infty}f_{ra}=\lim_{n\to\infty}\frac{n_A}{n}=Constante=P(A)$$
Donde:
- $n_A$ = Número de veces que ocurre el evento $A$ (casos favorables empíricos).
- $n$ = Número total de veces que se repitió el experimento.
- $P(A)$ = La verdadera probabilidad objetiva del evento.

>[!abstract] Resumen del concepto
>Bajo condiciones de **independencia**, la aleatoriedad individual de cada ensayo se "cancela" a largo plazo. El teorema de convergencia nos garantiza que la frecuencia relativa $f_{ra}$ no vagará para siempre, sino que encontrará un punto de equilibrio (una constante). Esa constante es lo que llamamos Probabilidad.

---
# Ejemplos de aplicación
### 1. El fenómeno de estabilización
Supongamos que queremos conocer la probabilidad objetiva $P(A)$ de que un votante en Argentina elija al "Candidato X". Si comenzamos a encuestar personas una por una (cada encuesta es un ensayo independiente), observaremos lo siguiente en la frecuencia relativa ($f_{ra}=n_A/n$):
- $n=10:$ Si 7 dicen que sí, $f_{ra}=0.7$
- $n=100:$ Si 45 dicen que sí, la frecuencia cae drásticamente a $f_{ra}=0.45$
- $n=2000:$ Si 1060 dicen que sí, $f_{ra}=0.53$

La evidencia empírica demuestra que a medida que $n$ crece, la frecuencia relativa deja de dar "saltos" y se estabiliza. En la práctica, no necesitamos llegar al "infinito" teórico; al acercarnos a $n=2000$, la frecuencia ya casi no fluctúa sin importar a cuántos encuestemos después. Matemáticamente, hemos alcanzado la "constante" y podemos asumir que la probabilidad real ronda el 53%.