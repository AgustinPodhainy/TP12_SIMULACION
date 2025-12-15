# Estudio de Estrategias del Uso de Pesticidas y su Impacto en el Rendimiento Agrícola y la Sustentabilidad Apícola mediante Simulación Dinámica

Este repositorio contiene el desarrollo del Trabajo Práctico Nº12 de la materia **Simulación** (UTN FRBA), enfocado en el análisis del trade-off entre producción agrícola, uso de pesticidas y preservación de las abejas, mediante un modelo de simulación dinámica basado en datos reales y distribuciones de probabilidad ajustadas.

El trabajo estudia cómo distintas políticas de manejo agrícola impactan simultáneamente en la producción, la supervivencia de las abejas y la acumulación de residuos químicos en el suelo, con el objetivo de identificar estrategias productivas sostenibles en el largo plazo.

## Descripción General

El objetivo principal del trabajo es modelar, simular y analizar el impacto de diferentes combinaciones de:

- Cantidad de hectáreas cultivadas (HC)
- Toneladas de pesticidas aplicadas por hectárea (TPH)
sobre el desempeño global del sistema agrícola.

El modelo considera explícitamente el rol de las abejas como servicio ecosistémico de polinización, así como los efectos negativos del uso intensivo de pesticidas, que incrementan la mortalidad de colonias y la saturación química del suelo.

A partir de un horizonte de simulación de largo plazo (20 años), se evalúan distintas estrategias productivas, analizando sus consecuencias en:

- Producción Agrícola Promedio anual (PAP)
- Porcentaje Final de la población original de abejas que logra sobrevivir (PAV)
- Porcentaje de Producción atribuible a las Abejas (PPA)
- Nivel Promedio de Saturación Química del suelo (NPSQ)

## Estructura del Repositorio

- **FDPS**  
  Resultados del ajuste de funciones de densidad de probabilidad (fdp) para los modelos de simulación.

- **Presentación**  
  Archivo con la exposición utilizada para la defensa del trabajo.

- **Diagrama**  
  Esquema del modelo de simulación dinámica, incluyendo stocks, flujos y relaciones causales entre pesticidas, abejas, suelo y producción.

- **Paper**  
  Documento con la definición de variables, eventos y estructura de la simulación.


## Metodología

 **Simulación Avance del Tiempo por Intervalos Fijos:**  

El modelo se implementa mediante **simulación dinámica de sistemas**.

El tiempo de simulación avanza con un **delta t (Δt) fijo de 1 año**, adecuado para representar procesos agrícolas y ecológicos de evolución lenta, como la dinámica poblacional de las abejas y la acumulación y degradación de pesticidas en el suelo.

Para cada escenario se realizan **dos simulaciones**, una de **corto plazo (5 años)** y otra de **largo plazo (20 años)**, permitiendo comparar los efectos inmediatos y acumulativos de las distintas estrategias de manejo.

En cada paso anual se actualizan la cantidad de colonias vivas, el impacto residual de pesticidas en el suelo y el rendimiento agrícola anual, en función de las decisiones de control (HC y TPH).


## Escenarios Analizados

**Escenario Intensivo (E1):**
Alta superficie cultivada y uso intensivo de pesticidas. Maximiza la producción inicial, pero genera una fuerte degradación ecológica y una caída de la producción en el largo plazo.

**Escenario de Transición (E2):**
Uso moderado de pesticidas y superficie intermedia. Permite alcanzar una producción estable y competitiva, preservando parcialmente la población de abejas y manteniendo controlada la saturación química del suelo.

**Escenario Ecológico (E3):**
Superficie intermedia cultivada con uso mínimo de pesticidas. Preserva la población de abejas y reduce el impacto químico, pero no alcanza niveles de producción competitivos.

## Cómo usar este repositorio

1. **Revisar los archivos de análisis previo** para entender la estructura y variables del modelo.
2. **Consultar las FDPS** para ver cómo se modelan los tiempos y distancias reales.
3. **Utilizar la presentación y el diagrama** para entender el flujo de la simulación.

## Autoría

Trabajo realizado por:  
- María Emilia Andersen
- Priscila Sharon D’Antoni 
- Agustín Podhainy Vignola  

Materia: **Simulación**  
Universidad Tecnológica Nacional, Facultad Regional Buenos Aires


