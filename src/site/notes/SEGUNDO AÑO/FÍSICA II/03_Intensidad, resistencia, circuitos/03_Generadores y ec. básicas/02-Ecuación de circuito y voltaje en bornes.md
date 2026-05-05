---
{"dg-publish":true,"permalink":"/segundo-ano/fisica-ii/03-intensidad-resistencia-circuitos/03-generadores-y-ec-basicas/02-ecuacion-de-circuito-y-voltaje-en-bornes/","dgPassFrontmatter":true,"dg-note-properties":{}}
---

Tags; #electrodinámica #circuitos #voltaje #baterías 

## 1. La ecuación del circuito
Consideramos un circuito cerrado que contiene un generador (ej. una batería con fem $\epsilon$ y resistencia interna $r$), un receptor que consume energía (ej. un motor con fuerza contraelectromotriz $\epsilon'$ y resistencia interna $r'$), y una resistencia exterior $R$ (que pueden ser los cables).

Si aplicamos el principio de conservación de la energía para un segundo de tiempo, sabemos que todo el trabajo que hace la batería debe ser igual al trabajo mecánico que hace el motor más todo el calor disipado por el efecto Joule en todas las resistencias (internas y externas):
$$P_{suministrada}=P_{util}+P_{perdida-calor}$$
$$\epsilon\cdot i=\epsilon'\cdot i+R\cdot i^2+r\cdot i^2+r'\cdot i^2$$
Si dividimos toda la ecuación por la intensidad de corriente $(i)$, obtenemos la ecuación del circuito en serie:
$$i=\frac{\epsilon-\epsilon'}{R+r+r'}$$
>[!important] Regla General
>La intensidad de la corriente en un circuito en serie es igual a la suma algebraica de las FEM del circuito, dividida por la suma de todas las resistencias del mismo.
>$$i=\frac{\sum\epsilon}{\sum R}$$

---
## 2. Diferencia de potencial entre dos puntos
*(Relacionado con [[SEGUNDO AÑO/FÍSICA II/02_Potencial eléctrico/01_Conceptos/02-Potencial y dif. de potencial\|02-Potencial y dif. de potencial]])* Si no queremos analizar todo el circuito, sino solo un tramo desde un punto $a$ hasta un punto $b$, podemos calcular la diferencia de potencial o caída de voltaje entre esos dos puntos. La fórmula general se deduce del balance de potencias y es:
$$V_{ab}=\sum(i\cdot R)-\sum\epsilon$$
>[!danger] Cuidado: Convenio de signos
>Si decidimos caminar o analizar el tramo desde $a$ hasta $b$:
>1. **Corriente ($i$):** Es positiva si fluye en nuestra misma dirección (de $a$ hacia $b$), y negativa si viene de frente.
>2. **FEM ($\epsilon$):** Es positiva si "empuja" en nuestra misma dirección, y negativa si "empuja" en contra.
>3. **Resistencias ($R$):** Siempre son positivas.

Aquí está la gran trampa teórica. Si compramos una pila que dice "1.5 V", *¿siempre entrega 1.5 V al circuito?* **NO**. El voltaje real que medimos en los bornes metálicos exteriores de la pila ($V_{ab}$) depende de lo que esté haciendo la pila.
- **Caso A: La batería está entregando corriente (descargándose)**
  La corriente $i$ sale del borne positivo. Dentro de la batería, la resistencia interna $r$ "frena" un poco esa energía. El voltaje real que llega al circuito es la FEM teórica menos lo que se perdió adentro:
  $$V_{ab}=\epsilon-i\cdot r$$
- **Caso B: La batería recibiendo corriente (cargándose)**
  Obligamos a la corriente a entrar por el borne positivo (como hace un alternador para recargarla). Ahora, para meter la energía, debemos vencer la FEM de la batería y además superar la fricción de su resistencia interna:
  $$V_{ab}=\epsilon+i\cdot r$$
- **Caso C: Circuito abierto**
  Si la batería está desconectada, la corriente es nula ($i=0$). Solo en este caso exacto, el voltaje en los bornes es exactamente igual a la FEM ($V_{ab}=\epsilon$).
