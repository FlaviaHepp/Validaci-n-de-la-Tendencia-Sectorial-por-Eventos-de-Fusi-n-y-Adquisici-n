# 📈Validación de la Tendencia Sectorial por Eventos de Fusión y Adquisición

## 📌Descripción del Proyecto

Este proyecto analiza cómo el contexto técnico de un sector influye en la reacción del mercado ante eventos de Fusión y Adquisición (M&A).
En particular, valida si las adquisiciones generan mejores rendimientos cuando ocurren dentro de sectores que ya presentan una tendencia alcista fuerte, frente a sectores débiles o bajistas.

La hipótesis central es que el mercado recompensa más las adquisiciones cuando el “viento sectorial” acompaña, reforzando la eficiencia del capital desplegado.

## 🎯Objetivo del Análisis

Responder a la siguiente pregunta estratégica:

¿Las adquisiciones realizadas en sectores con “Cruce Dorado” (SMA 50 > SMA 200) generan un mayor rendimiento post-evento que aquellas realizadas en sectores con tendencia bajista o lateral (“Cruce Muerto”)?

## 🧠Insight Clave

Un sector en Cruce Dorado indica:
- Tendencia alcista estructural
- Mayor confianza del mercado
- Flujo de capital sostenido

En este contexto, una adquisición:
- Es percibida como aceleradora de valor
- Tiene mayor probabilidad de continuidad alcista
- Por el contrario, adquisiciones en sectores débiles suelen interpretarse como defensivas o de rescate, con menor impacto positivo en precio.

## 🧩 Metodología

El análisis se divide en dos etapas principales:

1. Clasificación de la Tendencia Sectorial

Se calcula, por sector y fecha, el promedio de:
- SMA 50
- SMA 200

Se define:
- Cruce Dorado → SMA 50 promedio > SMA 200 promedio
- Cruce Muerto/Lateral → Caso contrario

2. Medición del Impacto del Evento

Se identifican eventos de tipo Adquisición

Para cada ticker:
- Se toma el precio de cierre el día del evento
- Se calcula el precio de cierre 10 días después
- Se mide el rendimiento porcentual post-evento

3. Comparación Final

Se agrupan los resultados por:
- Tipo de tendencia sectorial

Se compara:
- Rendimiento promedio post-adquisición
- Número de eventos analizados

## 📊Output Esperado

El resultado final muestra, para cada escenario sectorial:
- Tipo de tendencia (Cruce Dorado vs Cruce Muerto/Lateral)
- Cantidad de adquisiciones analizadas
- Rendimiento promedio a 10 días post-evento
- Ordenado para identificar qué contexto maximiza el retorno esperado.

## 💼Valor de Negocio

Este análisis es especialmente útil para:
- 📈 Estrategias event-driven
- 🏦 Fondos de arbitraje y M&A
- 🧭 Asset allocation sectorial

## ⚠️Evaluación de riesgo antes de operar eventos corporativos

Permite responder preguntas como:
- ¿Conviene operar adquisiciones solo cuando el sector acompaña?
- ¿Qué tan importante es el contexto macro-sectorial frente al evento puntual?

## ⚠️Consideraciones

- El análisis asume disponibilidad de datos suficientes post-evento (10 días).
- No incorpora ajuste por volatilidad; puede combinarse con métricas de riesgo (kurtosis, drawdown, Sharpe).
- La tendencia sectorial se evalúa en la fecha exacta del evento.

## 🚀Posibles Extensiones

- Ajustar el rendimiento por volatilidad post-evento
- Comparar horizontes temporales (3d, 5d, 20d)
- Filtrar adquisiciones hostiles vs amistosas
- Incorporar país de origen como tercera dimensión
  
## 👤Autora
Flavia Hepp Proyecto de SQL aplicó un análisis de riesgo basado en eventos.

