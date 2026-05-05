---
{"dg-publish":true,"permalink":"/segundo-ano/fisica-ii/02-potencial-electrico/02-potencial-electrico/","dgPassFrontmatter":true,"dg-note-properties":{}}
---

## UNIDAD N°2 - Potencial eléctrico

**Plan académico:**
Energía potencial electrostática. Potencial. Potencial y distribución de cargas. Gradiente de potencial. Ecuaciones de Poisson y Laplace. Superficies equipotenciales. Reparto de cargas entre conductores. Generador de Van de Graff.

#### Conceptos
- [[SEGUNDO AÑO/FÍSICA II/02_Potencial eléctrico/01_Conceptos/01-Energía potencial electroestática\|01-Energía potencial electroestática]]
- [[SEGUNDO AÑO/FÍSICA II/02_Potencial eléctrico/01_Conceptos/02-Potencial y dif. de potencial\|02-Potencial y dif. de potencial]]
- [[SEGUNDO AÑO/FÍSICA II/02_Potencial eléctrico/01_Conceptos/03-Superficies equipotenciales\|03-Superficies equipotenciales]]

#### Relaciones matemáticas
- [[SEGUNDO AÑO/FÍSICA II/02_Potencial eléctrico/02_Relaciones matemáticas/01-Potencial y distr. de cargas\|01-Potencial y distr. de cargas]]
- [[SEGUNDO AÑO/FÍSICA II/02_Potencial eléctrico/02_Relaciones matemáticas/02-Gradiente de potencial\|02-Gradiente de potencial]]
- [[SEGUNDO AÑO/FÍSICA II/02_Potencial eléctrico/02_Relaciones matemáticas/03-Ecuaciones de Poisson y Laplace\|03-Ecuaciones de Poisson y Laplace]]

#### Conductores y aplicaciones
- [[SEGUNDO AÑO/FÍSICA II/02_Potencial eléctrico/03-Conductores y aplicaciones/01-Potencial de un conductor esférico cargado\|01-Potencial de un conductor esférico cargado]]
- [[SEGUNDO AÑO/FÍSICA II/02_Potencial eléctrico/03-Conductores y aplicaciones/02-Reparto de cargas entre conductores\|02-Reparto de cargas entre conductores]]
- [[SEGUNDO AÑO/FÍSICA II/02_Potencial eléctrico/03-Conductores y aplicaciones/03-Generador de Van de Graff\|03-Generador de Van de Graff]]

### Preguntas de repaso

**1. Por qué la energía potencial eléctrica de una carga de prueba que se mueve en un campo eléctrico es completamente independiente de la trayectoria seguida? ¿Qué ocurre con la suma de las energías cinética y potencial si la única fuerza actuante es la del campo?**
Es independiente porque el campo electrostático es conservativo; la integral curvilínea de la intensidad del campo a lo largo de una trayectoria cerrada es rigurosamente nula. Si la trayectoria importara, el concepto de energía potencial no tendría un valor único y carecería de sentido físico. Además, si la carga se mueve únicamente bajo la influencia del campo (sin fuerzas exteriores), el sistema conserva su energía, siendo la suma de las energías cinética y potencial siempre constante en todos los puntos de la trayectoria ($EC_a​+EP_a​=EC_b​+EP_b$​).

**2. Define estrictamente el concepto de "Volt" y explica la diferencia conceptual entre el "potencial" en un punto y la "diferencia de potencial" (voltaje) entre dos puntos.**
Un Volt se define como la diferencia de potencial que existe cuando, para traer una carga de un Coulomb desde el infinito hasta un punto (venciendo las fuerzas del campo), es necesario realizar un trabajo exacto de un Joule. El "potencial absoluto" en un punto se calcula midiendo el trabajo realizado asumiendo el nivel de energía cero en el infinito. En cambio, la "diferencia de potencial" entre dos puntos $a$ y $b$ ($V_{ab}$​) mide estrictamente el trabajo exterior necesario por unidad de carga para mover físicamente dicha carga desde $b$ hasta $a$, sin importar el infinito.

**3. ¿Qué cantidad de trabajo eléctrico se requiere para mover una carga a lo largo de una superficie equipotencial y qué relación geométrica inquebrantable existe entre estas superficies y las líneas de fuerza del campo eléctrico?**
El trabajo requerido es estrictamente nulo, ya que la energía potencial de un cuerpo cargado es la misma en todos los puntos de dicha superficie. Geométricamente, las superficies equipotenciales deben ser siempre perpendiculares a la dirección de las líneas de fuerza del campo eléctrico en cualquier punto; de lo contrario, el campo tendría una componente paralela a la superficie y habría que realizar trabajo para mover una carga contra ella.

**4. Al momento de calcular el efecto generado por múltiples cargas en un punto del espacio, ¿qué gran ventaja matemática presenta calcular el potencial en lugar de calcular la intensidad del campo eléctrico?**
La inmensa ventaja es que el potencial es una magnitud escalar (energía por unidad de carga). Por lo tanto, el potencial resultante en un punto se calcula realizando una simple suma algebraica de los potenciales individuales de cada carga ($V=\sum V_i​$), evitando por completo la compleja descomposición trigonométrica y suma vectorial que requiere el cálculo del campo eléctrico $E$.

**5. Escribe la relación matemática entre la intensidad del campo eléctrico (E) y el potencial (V). ¿Qué nos indica físicamente el signo negativo de esta relación?**
La intensidad del campo eléctrico en una dirección determinada es exactamente igual a la derivada del potencial respecto a la distancia en dicha dirección, cambiada de signo ($E=−dV/ds$). Esta relación se denomina Gradiente de Potencial. El signo negativo indica físicamente que el vector del campo eléctrico apunta siempre hacia la dirección en la cual el nivel de potencial eléctrico disminuye.

**6. En qué se diferencian físicamente los escenarios donde aplicamos la ecuación de Poisson y donde aplicamos la ecuación de Laplace para calcular un potencial en tres dimensiones?**
Ambas ecuaciones relacionan las derivadas espaciales segundas del potencial. La ecuación de Poisson se aplica cuando en la región de análisis existe una "carga espacial" (una densidad de carga volumétrica $\rho$ distinta de cero), quedando igualada a $-\rho/\epsilon_0$. Por su parte, la ecuación de Laplace es un caso especial que se utiliza cuando en el espacio de análisis no hay ninguna carga libre ($\rho=0$), igualando la suma de las derivadas segundas a cero.

**7. Describe cómo es el valor del campo eléctrico (E) y del potencial (V) en el interior de una esfera conductora cargada maciza en comparación con su superficie.**
En el interior de un conductor en equilibrio electrostático, el campo eléctrico es rigurosamente nulo ($E=0$). Como consecuencia matemática de que el gradiente es nulo, el potencial ($V$) en todo el volumen interior no cambia; se mantiene constante y posee exactamente el mismo valor que tiene en la superficie metálica de la esfera.

**8. Explica, utilizando el concepto de rigidez dieléctrica, por qué el potencial que puede alcanzar una esfera conductora en el aire está directamente condicionado por su radio de curvatura.**
El aire tiene una rigidez dieléctrica limitada (aprox. $3\cdot10^6V/m$); si el campo eléctrico supera este valor, el aire se ioniza y se vuelve conductor, produciendo descargas (chispas). El potencial máximo antes de la rotura depende directamente del radio de la esfera ($V_m=E_m\cdot a$). Si el radio es minúsculo (como en una punta aguda), el límite de rigidez del aire se rompe a potenciales mucho más bajos; por ende, solo esferas de gran tamaño (gran radio) pueden almacenar altos voltajes, como se requiere en un generador de Van de Graff.

**9. Si conectamos mediante un hilo conductor una esfera muy pequeña cargada y una esfera muy grande descargada, ¿qué condición dictamina cuándo dejará de fluir carga entre ellas y cuál quedará con mayor densidad superficial de carga?**
El flujo de cargas cesará únicamente cuando todos los puntos de ambos conductores alcancen exactamente el mismo potencial eléctrico ($V_A=V_B$​). Aunque la esfera de mayor radio almacenará casi toda la carga total del sistema, la esfera pequeña quedará con una densidad superficial de carga (σ) muchísimo mayor, reafirmando que las cargas se aprietan densamente en las zonas de menor radio de curvatura.

**10. ¿Cuál es el principio electrostático mágico o fundamental que permite que un generador de Van de Graff reciba cargas continuamente y acumule un voltaje enorme, venciendo la repulsión de las cargas que ya tiene en su domo?**
El principio es el contacto interno entre conductores. Cuando la correa ingresa cargas a la cavidad hueca del domo y hace contacto con la escobilla interior, toda la carga pasa inevitable e íntegramente hacia el exterior del conductor hueco. Esto ocurre porque el interior siempre queda a un potencial superior al del exterior mientras tenga carga, forzando a que la transferencia sea siempre del 100%, sin importar cuán inmenso sea el potencial repulsivo que el domo exterior ya haya acumulado.