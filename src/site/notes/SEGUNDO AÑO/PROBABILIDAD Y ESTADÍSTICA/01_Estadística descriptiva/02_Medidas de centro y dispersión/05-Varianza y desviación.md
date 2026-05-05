---
{"dg-publish":true,"permalink":"/segundo-ano/probabilidad-y-estadistica/01-estadistica-descriptiva/02-medidas-de-centro-y-dispersion/05-varianza-y-desviacion/","dgPassFrontmatter":true,"dg-note-properties":{}}
---

Tags: #dispersión #estadística_descriptiva #medidas_resumen #fórmulas 

## 1. Varianza poblacional ($\sigma^2$)
Evalúa la variabilidad poblacional promediando las desviaciones al cuadrado de cada dato respecto a la media poblacional:
$$\sigma^2=\frac{\sum_{i=1}^N(x_i-\mu)^2}{N}$$
## 2. Varianza muestral ($s^2$)
Evalúa la variabilidad de la muestra promediando las desviaciones al cuadrado de cada dato respecto a la media muestral:
$$s^2=\frac{\sum_{i=1}^n(x_i-\bar{x})^2}{n-1} \ \ \ \ \ \text{(datos no agrupados)}$$
$$s^2=\sum_{i=1}^{mca}f_{ri}(mca_i-\bar{x})^2 \ \ \ \ \ \text{(datos agrupado)}$$
>[!question]
>¿Por qué dividimos entre $n-1$ y no entre $n$ en la varianza muestral? Las observaciones de una muestra tienden a estar más cerca de su propia media muestral ($\bar{x}$) de lo que están de la verdadera media poblacional ($\mu$). Si dividiéramos entre $n$ estaríamos subestimando la verdadera variabilidad de la población (obtendríamos valores demasiado pequeños en promedio). Dividir entre $n-1$ (conocido como grados de libertad) corrige este sesgo, haciendo que $s^2$ sea un estimador "insesgado" de $\sigma^2$.

## 3. Desviación estándar muestral ($s$)
Es simplemente la raíz cuadrada positiva de la varianza muestral:
$$s=\sqrt{s^2}$$
Tiene la ventaja de estar en las mismas unidades lineales que los datos originales.

## 4. Interpretación de varianza y desviación muestral
Para entender qué significa el resultado de estas fórmulas, imaginemos que estamos analizando los tiempos de vuelta de Lewis Hamilton en una sesión de clasificación libre de 20 vueltas.

La **varianza** y la **desviación estándar** miden la consistencia o el error. En ingeniería suelen representar la tolerancia o el ruido.

Un **valor más bajo** (tendiendo a cero) significa precisión absoluta. Las 20 vueltas de Hamilton fueron clavadas en el mismo milisegundo, es un relojito. En ingeniería eléctrica, un $s$ bajo en una partida de resistores de 100 $\ohm$ significa excelente control de calidad (todos miden 99.9, 100.1, 100.0).

Un **valor más alto** significa inconsistencia, caos o mucha dispersión. Hamilton hizo algunas vueltas rapidísimas y otras lentísimas. En los resistores, un $s$ alto significa que te pueden tocar resistencias de 90 $\ohm$ o de 110 $\ohm$; es un lote poco confiable.

**¿Por qué preferimos la desviación estándar $(s)$?**
Porque la varianza te da el resultado en unidades al cuadrado (lo cual no tiene sentido físico). Al aplicarle la raíz cuadrada, la desviación estándar $s$ te da un valor en la misma unidad que medís. Si medimos $s=0.5$ segundos (en caso de Hamilton), significa que en promedio, sus tiempos fluctúan medio segundo por encima o por debajo de la media.
