---
{"dg-publish":true,"permalink":"/segundo-ano/fisica-ii/02-potencial-electrico/02-relaciones-matematicas/01-potencial-y-distr-de-cargas/","dgPassFrontmatter":true,"dg-note-properties":{}}
---

Tags: #potencial #cálculo #matemática 

## 1. Potencial de una carga puntual
Si tenemos una sola carga puntual $q$, y queremos saber el potencial en un punto situado a una distancia $r$ de ella, partimos de la definición de diferencia de potencial e integramos el campo eléctrico $E=\frac{1}{4\pi\epsilon_0}\frac{q}{r^2}$ desde el infinito hasta ese punto.

El resultado de esa integral nos da la fórmula directa para el potencial de una carga puntual:
$$V=\frac{1}{4\pi\epsilon_0}\frac{q}{r}$$
>[!important] El signo importa
>A diferencia del campo eléctrico, donde a veces analizamos solo el módulo, aquí la distancia $r$ siempre es positiva, por lo que el potencial $V$ tendrá siempre el mismo signo algebraico que la carga $q$. Si $q$ es negativa, genera un potencial negativo a su alrededor. El potencial se mide en $V$ si la carga está en Coulomb y la distancia en metros.

---
## 2. Sistema de múltiples cargas (superposición)
*¿Qué sucede si el campo es creado por varias cargas puntuales ($q_1,q_2,...$)?* El potencial en un punto dado será simplemente la suma de los potenciales individuales generados por cada carga.
$$V=\frac{1}{4\pi\epsilon_0}\sum\frac{q_i}{r_i}$$
$$V=\frac{1}{4\pi\epsilon_0}\left(\frac{q_1}{r_1}+\frac{q_2}{r_2}+...+\frac{q_n}{r_n}\right)$$
---
## 3. Distribuciones continuas de carga
Si en lugar de cargas puntuales separadas tenemos un cuerpo macizo, un hilo o una placa cargada, la suma algebraica se transforma en una integral. Imaginamos el cuerpo dividido en infinitas cargas elementales $dq$, y el potencial será:
$$V=\frac{1}{4\pi\epsilon_0}\int\frac{dq}{r}$$
*Nota:* Esta misma ecuación se aplica para calcular el potencial en puntos exteriores a una esfera conductora uniformemente cargada, ya que su campo exterior se comporta igual que si toda su carga estuviera concentrada en el centro.

---
## 4. Independencia de la trayectoria
De las ecuaciones anteriores se deduce algo mecánicamente brillante: el potencial en un punto de un campo electroestático solo depende de los valores de las cargas que lo crean y de sus distancias al punto elegido ($r$). Esto reafirma teóricamente que el potencial es totalmente independiente de la trayectoria que hayamos utilizado para calcular la integral desde el infinito hasta el punto. Si la trayectoria importara, el potencial no tendría un valor único y este concepto no tendría sentido físico.

---

>[!example] Ejemplos: La ventaja escalar vs vectorial:
>**Calcular el campo eléctrico (vectores)**
>Es como analizar un choque múltiple en la primera curva. Tenemos que calcular con qué fuerza (módulo) golpeó el auto de Hamilton, desde qué ángulo exacto (dirección) y hacia dónde (sentido). Sumar todo eso requiere trigonometría, componentes $X4 e $Y$, y es un dolor de cabeza.
>
>**Calcular el potencial (escalar)**
>Es como sumar el tiempo de penalización de Franco Colapinto. Si los comisarios le dan $+5$ segundos por exceder los limites de pista, $+10$ segundos por causar una colisión y le restan $-3$ segundos por una apelación exitosa... simplemente tenemos $5+10-3=12$ segundos. No importa la dirección ni el ángulo, la suma de potenciales es así de directa; solo tomamos la magnitud de la carga, la dividimos por la distancia y suma algebraicamente.

