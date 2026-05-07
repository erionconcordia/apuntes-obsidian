---
{"dg-publish":true,"permalink":"/segundo-ano/fisica-ii/04-dielectricos-capacidad-capacitores/02-capacidad-y-capacitores/06-funciones-de-un-dielectrico-en-un-capacitor/","dgPassFrontmatter":true,"dg-note-properties":{}}
---

Tags: #capacitores #rigidez-dieléctrica #dieléctrico #dieléctricos 

## 1. Función mecánica (soporte)
El dieléctrico sólido sirve para mantener la separación física entre las dos placas metálicas.

Permite que las placas estén extremadamente cerca sin tocarse, lo cual es vital porque una separación pequeña ($d$) aumenta la capacitancia. Sin el sólido, las placas se atraerían por fuerzas electrostáticas y harían cortocircuito.

---
## 2. Aumento del voltaje máximo (rigidez dieléctrica)
El material permite que el capacitor soporte una diferencia de potencial mucho mayor antes de que ocurra la "ruptura".

>[!abstract] Relación con el campo eléctrico
>La rigidez dieléctrica no es otra cosa que el campo eléctrico máximo ($E_{max}$) que aguanta la estructura atómica de un material antes de romperse (ionizarse) y dejar pasar un chispazo.

Recordamos la relación entre el voltaje, el campo eléctrico y la distancia en un campo uniforme (con valores máximos):
$$V_{max}=E_{max}\cdot d$$
- El aire tiene un $E_{max}$ de aproximadamente $3\cdot10^6V/m$.
- Un plástico como el teflón tiene un $E_{max}$ de aproximadamente $60\cdot10^6V/m$

Matemáticamente, si reemplazamos el (por ej.) el aire por teflón en esa fórmula de relación, manteniendo exactamente la misma distancia $d$, el voltaje máximo que podemos aplicar antes de que el capacitor "explote" se multiplica por 20 ($3*20=60$). Por eso soporta más energía de forma segura.

*Entonces:*
Todo aislante tiene un límite llamado rigidez dieléctrica (el campo eléctrico máximo que soporta antes de ionizarse y volverse conductor). Como la mayoría de los sólidos tienen una rigidez mucho mayor que la del aire, el capacitor puede almacenar más energía de forma segura.

---
## 3. Aumento de la capacitancia ($C$)
El objetivo principal de un dieléctrico es permitir que el capacitor almacene más carga ($Q$) para una misma diferencia de potencial ($V$). Esto sucede por una reacción en cadena:

#### A. Polarización
Cuando metemos el aislante entre las placas, los electrones de sus átomos (que están "atados" y no son libres) se estiran hacia la placa positiva.

- **Imagen mental:** El átomo se deforma como un óvalo. Esto crea una capa de cargas inducidas en las superficies del dieléctrico.
- Estas cargas generan un campo eléctrico inducido ($E_{ind}$) que apunta en dirección al campo de las palcas ($E_0$).
#### B. Debilitamiento del campo
Como los dos campos se oponen, el campo total o campo neto ($E_{neto}$) dentro del material se reduce a:
$$E_{neto}=E_0-E_{ind}$$
#### C. Relación voltaje-capacidad
Si el campo eléctrico disminuye, el voltaje entre las placas también baja:
$$V=E\cdot d$$
Al bajar el voltaje ($V$) en la fórmula de capacitancia:
$$C=\frac{Q}{V}$$
El resultado final aumenta. Este aumento se resume con la constante dieléctrica ($K_e$):
$$C=K_e\cdot C_0$$
*Donde:*
- $C$ es la capacitancia final (con el material dieléctrico presente entre las placas).
- $C_0$ es la capacitancia inicial (cuando hay vacío o aire entre las placas).
- $K_e$ es la constante dieléctrica del material (número adimensional que siempre es mayor a 1).
