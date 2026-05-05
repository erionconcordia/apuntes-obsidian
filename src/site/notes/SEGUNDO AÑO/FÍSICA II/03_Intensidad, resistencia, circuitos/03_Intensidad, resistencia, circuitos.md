---
{"dg-publish":true,"permalink":"/segundo-ano/fisica-ii/03-intensidad-resistencia-circuitos/03-intensidad-resistencia-circuitos/","dgPassFrontmatter":true,"dg-note-properties":{}}
---

## UNIDAD N°3 - Intensidad, resistencia, circuitos

**Plan académico:**
Intensidad. Densidad de corriente. Sentido de una corriente. Circuito completo. Conductibilidad, resistencia y resistividad. Ley de Ohm. Cálculo de resistencias. Ley de Joule. Valores medio y eficaz de una corriente. Fuerza electromotriz. Ecuación de circuito. Diferencia de potencial entre los puntos de un circuito. Voltaje en los bornes de un generador. Conexión de resistencias en serie y paralelo. Redes de resistencias que contienen fem. Reglas de Kirchhoff. Medidas de energía y potencia.

**Disparador:** Simulación de circuitos con Multisim, medición de corrientes y tensiones en distintas ramas del mismo

#### Conceptos
- [[SEGUNDO AÑO/FÍSICA II/03_Intensidad, resistencia, circuitos/01_Conceptos/01-Intensidad y densidad de corriente\|01-Intensidad y densidad de corriente]]
- [[SEGUNDO AÑO/FÍSICA II/03_Intensidad, resistencia, circuitos/01_Conceptos/02-Resistencia, resistividad y Ley de Ohm\|02-Resistencia, resistividad y Ley de Ohm]]

#### Energía y disipación
- [[SEGUNDO AÑO/FÍSICA II/03_Intensidad, resistencia, circuitos/02_Energía y disipación/01-Ley de Joule y Potencia\|01-Ley de Joule y Potencia]]
- [[SEGUNDO AÑO/FÍSICA II/03_Intensidad, resistencia, circuitos/02_Energía y disipación/02-Valores medio y eficaz\|02-Valores medio y eficaz]]

#### Generación y ecuaciones básicas
- [[SEGUNDO AÑO/FÍSICA II/03_Intensidad, resistencia, circuitos/03_Generadores y ec. básicas/01-Fuerza electromotriz (fem)\|01-Fuerza electromotriz (fem)]]
- [[SEGUNDO AÑO/FÍSICA II/03_Intensidad, resistencia, circuitos/03_Generadores y ec. básicas/02-Ecuación de circuito y voltaje en bornes\|02-Ecuación de circuito y voltaje en bornes]]

#### Análisis de redes
- [[SEGUNDO AÑO/FÍSICA II/03_Intensidad, resistencia, circuitos/04_Análisis de redes/01-Conexiones en serie y paralelo\|01-Conexiones en serie y paralelo]]
- [[SEGUNDO AÑO/FÍSICA II/03_Intensidad, resistencia, circuitos/04_Análisis de redes/02-Redes complejas y Reglas de Kirchhoff\|02-Redes complejas y Reglas de Kirchhoff]]

### Preguntas de repaso

**1. ¿Cuál es la diferencia conceptual entre la intensidad de corriente ($i$) y la densidad de corriente ($J$) en un hilo conductor?**
La intensidad de corriente es una magnitud escalar que mide la cantidad total de carga que atraviesa una sección completa del hilo metálico por unidad de tiempo (i$=dq/dt$). En cambio, la densidad de corriente ($J$) es un vector que tiene la misma dirección que el campo eléctrico y relaciona esa intensidad total con el área transversal ($A$) del conductor ($J=i/A$) para indicarnos qué tan concentrado está el flujo de cargas.

**2. ¿Cuál es el sentido convencional de una corriente eléctrica y cómo contrasta esto con la realidad del movimiento de los electrones libres en un metal?**
Por un convenio histórico universal, se considera el sentido de la corriente eléctrica como si las cargas que se mueven fuesen todas positivas. Por lo tanto, en un conductor metálico, el sentido convencional asignado a la corriente es siempre opuesto al sentido en el que realmente se mueven los electrones libres (que tienen carga negativa y viajan de menor a mayor potencial).

**3. ¿De qué variables geométricas y propias del material depende la resistencia de un conductor cilíndrico? ¿Es la Ley de Ohm ($V=i\cdot R$) una ley universal para toda la materia?**
La resistencia depende de la longitud del conductor ($L$), su área de sección transversal ($A$) y de la resistividad intrínseca del material ($\rho$), mediante la ecuación $R=\rho\cdot L/A$. La Ley de Ohm **no es universal**; expresa una característica particular de ciertas sustancias (como los metales puros) a las que se llama "conductores lineales", en los cuales la resistividad (y la conductibilidad) se mantiene constante independientemente de la densidad de corriente que circule, haciendo que la diferencia de potencial sea una función lineal estricta de la corriente.

**4. ¿Cómo varía el comportamiento eléctrico (resistividad) de un metal puro al aumentar la temperatura, y en qué se diferencia del comportamiento de aisladores y electrolitos?**
En los metales, la resistividad aumenta con el incremento de la temperatura (poseen un coeficiente de temperatura $\alpha$ positivo). Por el contrario, los aisladores (no metales) y los electrolitos tienen un coeficiente α negativo, lo que significa que al elevarse la temperatura, su resistividad disminuye y conducen la electricidad más fácilmente.

**5. ¿Cuál es la explicación física a nivel microscópico por la cual un circuito transforma irreversiblemente energía eléctrica en calor (Ley de Joule)?**
El movimiento de los electrones en un conductor no es uniformemente libre. El campo eléctrico los acelera, pero chocan constantemente con las partículas fijas de la red cristalina del conductor (frenándose). En cada choque, los electrones ceden a las partículas fijas la energía cinética que acaban de ganar. Esta energía adquirida aumenta la amplitud de vibración de la red atómica del metal, lo cual se convierte irreversiblemente en calor a una razón dictada por $P=i^2\cdot R$.

**6. Para corrientes variables, ¿qué miden físicamente el "Valor Medio" y el "Valor Eficaz"?**
El Valor Medio es la intensidad constante equivalente que transportaría exactamente la misma carga total en el mismo intervalo de tiempo, y sirve para medir efectos como la deposición de masa en una electrólisis.
El Valor Eficaz (o RMS) es la intensidad constante equivalente que desarrollaría la misma cantidad de calor en la misma resistencia en un intervalo de tiempo dado. En el caso de una onda sinusoidal, equivale al valor máximo dividido por $\sqrt{2}​$ ($\approx0.707\cdot I_0$​).

**7. Define qué hace exactamente un generador de fuerza electromotriz (ε) y por qué se diferencia del comportamiento de una resistencia.**
Un generador de FEM es cualquier dispositivo capaz de realizar una transformación de energía reversible en sentido termodinámico entre la energía eléctrica y otras formas de energía (como la energía química interna de una batería o la mecánica de un motor), excluyendo el calor. La FEM se define como esa energía transformada (trabajo) por unidad de carga ($\epsilon=dW/dq$). Se diferencia de una resistencia porque la disipación en esta última ($i^2\cdot R$) genera calor, un proceso termodinámicamente irreversible.

**8. Si mides con un voltímetro los bornes de una batería de automóvil mientras está alimentando a las luces ($i>0$), ¿marcará exactamente el valor de su FEM? ¿Por qué?**
No, medirá un voltaje menor. Todo generador real posee una resistencia interna ($r$). Cuando la batería suministra una corriente, parte de su energía ideal (su FEM, $\epsilon$) se pierde internamente en forma de calor por efecto Joule ($r\cdot i^2$). La ecuación del voltaje real en sus bornes es $V_{ab}=\epsilon-i\cdot r$. Solo marcará la FEM exacta cuando se mida a circuito abierto ($i=0$).

**9. Al agrupar un número cualquiera de resistencias en paralelo en un circuito, ¿cuál es la característica fundamental del voltaje y cómo se calcula la resistencia equivalente?**
La característica clave de las resistencias en paralelo es que la diferencia de potencial (voltaje) entre los bornes de cada una de ellas debe ser exactamente la misma, ya que están conectadas a los mismos dos puntos comunes, mientras que la intensidad se reparte. La inversa de la resistencia equivalente se calcula como la suma de las inversas de las capacidades individuales ($1/R_{eq}=1/R_1+1/R_2+...$).

**10. ¿Qué establecen las dos reglas de Kirchhoff utilizadas para resolver redes complejas y qué principio físico de conservación respalda a cada una?**
Regla de nodos: La suma algebraica de las corrientes que se dirigen a cualquier nodo es cero ($\sum i=0$). Deriva del principio de **conservación de la carga** eléctrica; la carga no se acumula ni desaparece en las bifurcaciones.
Regla de mallas: La suma algebraica de las FEM (ε) en una malla cerrada es igual a la suma algebraica de las caídas de potencial ($i\cdot R$) en la misma malla ($\sum\epsilon=\sum i\cdot R$). Deriva del principio de conservación de la energía, indicando que la diferencia de potencial neta tras recorrer un camino cerrado completo es nula.