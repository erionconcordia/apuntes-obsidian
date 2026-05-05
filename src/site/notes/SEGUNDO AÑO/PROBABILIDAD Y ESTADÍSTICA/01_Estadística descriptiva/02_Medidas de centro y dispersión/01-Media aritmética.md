---
{"dg-publish":true,"permalink":"/segundo-ano/probabilidad-y-estadistica/01-estadistica-descriptiva/02-medidas-de-centro-y-dispersion/01-media-aritmetica/","dgPassFrontmatter":true,"dg-note-properties":{}}
---

Tags: #centralización #estadística_descriptiva #medidas_resumen #fórmulas 

# Media aritmética
## 1. Media poblacional ($\mu$)
Promedio de todos los valores en una población de tamaño $N$.
$$\mu=\frac{\sum_{i=1}^{N}x_i}{N}$$
## 2. Media muestral ($\bar{x}$)
Promedio aritmético de una muestra. Es el centroide o punto de equilibrio físico de los datos.
$$\bar{x}=\frac{\sum_{i=1}^{n}x_i}{n} \ \ \ \ \text{(datos no agrupados)}$$
$$\bar{x}=\sum_{i=1}^{mca}(mca_i\cdot\ f_{r}) \ \ \ \ \text{(datos agrupados)}$$
>[!cuidado]
>El principal defecto de la media aritmética es que su valor se ve drásticamente afectado por la presencia de un solo valor atípico (outlier) extremo.

## 3. Interpretación
Para entender qué significa el resultado de estas fórmulas, imaginemos que estamos analizando los tiempos de vuelta de Lewis Hamilton en una sesión de clasificación libre de 20 vueltas.

La **media** es el rendimiento general esperado. Si su tiempo medio es de 1:20.500, ese es su ritmo promedio. Un valor más alto significa un ritmo más lento en general, y un valor más bajo significa un ritmo más rápido en general.
El **problema de la media** es que es muy sensible. Si en una vuelta Lewis se despista, entra a boxes y marca un tiempo de 3:00.000, ese único dato "tira" del promedio hacia arriba, haciéndonos creer que su ritmo en general fue más lento de lo que realmente fue.

## 4. Propiedades de la media aritmética

>[!important] Propiedad 1
>**Equivalencia de la sumatoria total**
>La suma de todos los valores individuales de un conjunto de datos es igual a multiplicar la media $\bar{x}$ del conjunto por la cantidad total de datos $n$.
>$$\sum_{i=1}^{n}x_i=n\cdot\bar{x}$$

>[!important] Propiedad 2
>**Transformación lineal**
>Dada una variable $x$, si aplicamos $y=a\cdot x+b$, la nueva media será directamente:
>$$\bar{y}=a\cdot\bar{x}+b$$

>[!important] Propiedad 3
>**Suma de desviaciones nula**
>La suma de las desviaciones de cada dato respecto a su media siempre es cero:
>$$\sum_{i=1}^n(x_i-\bar{x})=0$$

>[!important] Propiedad 4
>**Mínimos caudrados**
>La suma de los cuadrados de las desviaciones de $n$ datos con respecto a una constante $c$, es decir:
>$$\sum_{i=1}^n(x_i-c)^2$$
>es mínima cuando esa constante es exactamente la media ($c=\bar{x}$).

>[!observacion]
>En estadística, cuando hablamos de una **desviación**, nos referimos pura y exclusivamente a la distancia o diferencia que hay entre un dato específico y el promedio. Matemáticamente, la desviación de un dato es simplemente esta resta: $x_i-\bar{x}$.

## 4. Demostración de propiedades

#### - Propiedad 1
Partimos de la definición matemática fundamental de la media muestral:
$$\bar{x}=\frac{\sum_{i=1}^nx_i}{n}$$
Multiplicamos a ambos lados de la ecuación por $n$:
$$n\cdot\bar{x}=\frac{\sum_{i=1}^nx_i}{n}\cdot n$$
Entonces, llegamos a la propiedad:
$$\sum_{i=1}^nx_i=n\cdot\bar{x}$$
#### - Propiedad 2
Definimos nuestra nueva variable y aplicamos la fórmula de la media:
$$\bar{y}=\frac{\sum_{i=1}^ny_1}{n}$$
Sustituimos $y_i$ por su transformación lineal $a\cdot x_i+b$:
$$\bar{y}=\frac{\sum_{i=1}^n(a\cdot x_i+b)}{n}$$
Distribuimos la sumatoria:
$$\bar{y}=\frac{\sum_{i=1}^n(a\cdot x_i)+\sum_{i=1}^nb}{n}$$
Sacamos la constante $a$ fuera de al sumatoria y resolvemos la sumatoria de la constante $b$ (que es $n\cdot b$). Luego separamos la fracción en dos términos.
$$
\bar{y}=\frac{a\sum_{i=1}^nx_i+n\cdot b}{n}
\ \ \ \ \ \ \to \ \ \ \ \ \
\bar{y}=a\left(\frac{\sum_{i=1}^nx_i}{n}\right)+\frac{n\cdot b}{n}
$$
El paréntesis es la definición de $\bar{x}$, y las $n$ del segundo término se cancelan, entonces demostramos:
$$\bar{y}=a\cdot\bar{x}+b$$
#### - Propiedad 3
Queremos demostrar que $\sum_{i=1}^n(x_i-\bar{x})=0$. Entonces, distribuimos la sumatoria $\Sigma$:
$$\sum_{i=1}^n(x_i-\bar{x})=\sum_{i=1}^nx_i-\sum_{i=1}^n\bar{x}$$
Como $\bar{x}$ es una constante, sumar una constante $n$ veces es igual a $n\cdot\bar{x}$:
$$\sum_{i=1}^n(x_i-\bar{x})=\sum_{i=1}^nx_i-n\cdot\bar{x}$$
Por la propiedad 1, sabemos que $\sum_{i=1}^nx_i=n\cdot\bar{x}$. Entonces, sustituimos esto en nuestra ecuación y demostramos:
$$\sum_{i=1}^n(x_i-\bar{x})=n\cdot\bar{x}-n\cdot\bar{x}=0$$
#### - Propiedad 4
Sea $c$ cualquier valor constante. Queremos evaluar la expresión:
$$\sum_{i=1}^n(x_i-c)^2$$
Entonces, sumamos y restamos la media $\bar{x}$ dentro del paréntesis (esto no altera el valor):
$$\sum_{i=1}^n(x_i-\bar{x}+\bar{x}-c)^2$$
Agrupamos los términos convenientes para formar un binomio al cuadrado:
$$\sum_{i=1}^n\big[(x_i-\bar{x})+(\bar{x}-c)\big]^2
\ \ \ \ \to \ \ \ \
\sum_{i=1}^n\big[(x_i-\bar{x})^2+2(x_i-\bar{x})(\bar{x}-c)+(\bar{x}-c)^2\big]
$$
Habiendo desarrollado el binomio al cuadrado, distribuimos la sumatoria en los tres términos resultantes. Notamos que en el segundo término, $2(\bar{x}-c)$ es una constante, por lo que sale de la sumatoria.
$$
\sum_{i=1}^n(x_i-\bar{x})^2+2(\bar{x}-c)\sum_{i=1}^n(x_i-\bar{x})+\sum_{i=1}^n(\bar{x}-c)^2
$$
Por la segunda propiedad, sabemos que $\sum_{i=1}^n(x_i-\bar{x})=0$. Por lo tanto, todo el término del medio se hace cero y desaparece:
$$\sum_{i=1}^n(x_i-\bar{x})^2+0+\sum_{i=1}^n(\bar{x}-c)^2$$
El término $(\bar{x}-c)^2$ es una constante sumada $n$ veces, entonces:
$$\sum_{i=1}^n(x_i-c)^2=\sum_{i=1}^n(x_i-\bar{x})^2+n(\bar{x}-c)^2$$
Entonces, como todo número elevado al cuadrado es positivo (o cero), la cantidad $n(\bar{x}-c)^2$ siempre será $\geq0$. Por lo tanto, demostramos que la sumatoria total será lo más chica posible (mínima) únicamente cuando el término $n(\bar{x}-c)^2=0$, y eso solo ocurre cuando $c=\bar{x}$.

