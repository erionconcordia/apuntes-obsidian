---
{"dg-publish":true,"permalink":"/segundo-ano/probabilidad-y-estadistica/01-estadistica-descriptiva/01-conceptos/05-estad-inferencial/","dgPassFrontmatter":true,"dg-note-properties":{}}
---

Tags: #estadística #análisis_de_datos #fórmulas 

## Estadística inferencial
Mientras que la probabilidad usa el *razonamiento deductivo* (conocer la población para predecir la muestra), la estadística inferencial usa el razonamiento inductivo: parte de la información incompleta de una muestra para sacar conclusiones, hacer generalizaciones o tomar decisiones sobre la población general.

Sus dos áreas principales de aplicación son:
#### 1. Estimación de parámetros
Busca deducir el valor de una característica poblacional desconocida (parámetro, como $\mu$ o $\sigma$) basándose en un estadístico de la muestra (como $\bar{x}$ o $s$).
- **Estimación puntual:** Se calcula un único número para representar el parámetro. Por ejemplo, el estimador puntual $\hat{\mu}=\bar{x}$.
- **Estimación por intervalos (intervalos de confianza):** Proporciona un rango de valores plausibles para el parámetro, incorporando el margen de error y un nivel de confianza (ej. 95%).
#### 2. Pruebas de hipótesis
Es un procedimiento de decisión basado en datos. Se plantean dos aseveraciones contradictorias sobre un parámetro del sistema científico y se determina si la evidencia muestral apoya rechazar la conjetura inicial.
- **Hipótesis nula ($H_0$):** La afirmación de "no cambió" o el status quo (ej. $H_0:\mu=50$)
- **Hipótesis alternativa ($H_1$ o $H_a$):** Lo que el ingeniero intenta demostrar (ej. $H_1:\mu>50$)
- **Valor P (P-Value):** Es la probabilidad de observar datos tan extremos como los obtenidos si la hipótesis nula fuera cierta. Sirve como cuantificador de la evidencia.

>[!informacion]
>**Aplicación en ingeniería en manufactura, ciencia de materiales o control de calidad**: nunca se miden componentes idénticos debido a la variación (ej. densidad de un material, resistencia de vigas, vida útil de baterías). Usamos la estadística descriptiva ($\bar{x}$, $s$) para auditar una muestra de esa producción y la estadística inferencial para garantizar matemáticamente (con un % de error controlado) que todo el lote futuro cumplirá con las especificaciones.

