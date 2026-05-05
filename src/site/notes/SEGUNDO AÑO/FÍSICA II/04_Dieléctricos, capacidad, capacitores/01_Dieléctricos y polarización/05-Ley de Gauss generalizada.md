---
{"dg-publish":true,"permalink":"/segundo-ano/fisica-ii/04-dielectricos-capacidad-capacitores/01-dielectricos-y-polarizacion/05-ley-de-gauss-generalizada/","dgPassFrontmatter":true,"dg-note-properties":{}}
---

Tags: #dieléctrico #teorema-gauss #desplazamiento 

## 1. Las constantes del material
Cuando metemos un aislante en un campo, este reacciona. Para medir esa reacción, definimos tres niveles de "calidad" del material que están encadenados:
1. **Susceptibilidad ($\eta$):** Mide qué tan fácil se forman los dipolos.
$$\eta=\frac{\sigma_i}{E}$$
2. **Coeficiente dieléctrico ($K_e$):** Es el factor de escala. Nos dice cuántas veces es "mejor" que el vacío.
$$K_e=1+\frac{\eta}{\epsilon_0}$$
3. **Capacidad específica ($\epsilon$):** Es la constante definitiva del material que usaremos en las fórmulas.
$$\epsilon=K_e\cdot\epsilon_0$$

Como herramienta auxiliar aparece el desplazamiento ($D$):
$$D=\epsilon\cdot E$$
---
## 2. Ley de Gauss generalizada
Es el Teorema de Gauss de toda la vida ([[SEGUNDO AÑO/FÍSICA II/01_Ley de Coulomb y campo eléctrico/03_Leyes y teoremas/02-Teorema de Gauss\|02-Teorema de Gauss]]), pero usando nuestro vector $D$ para atravesar materiales:
$$\oint D\cdot\cos(\phi)\cdot dA=q_{libre}$$
>[!success] Método de resolución
>Con esta estructura, los problemas se resuelven siempre en dos pasos:
>1. Gauss para hallar $D$ (usando solo la carga que conocemos, la libre).
>2. Definición del material ($E=D/\epsilon$) para hallar el campo real final.



