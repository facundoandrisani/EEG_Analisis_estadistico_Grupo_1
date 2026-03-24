# 📊 Detección de Crisis Epilépticas: Análisis Estadístico en el Dominio del Tiempo

Este proyecto se centra en el análisis temporal de señales electroencefalográficas (EEG) para identificar y caracterizar crisis epilépticas mediante el uso de descriptores estadísticos. Se utiliza la base de datos **CHBMIT Scalp EEG Database** de PhysioNet.

## 🎯 ¿Qué hace este proyecto?
El flujo de trabajo segmenta las señales continuas de EEG en tres bloques temporales fundamentales: 2 minutos antes de la crisis (Before), la crisis en sí, y 2 minutos después (After). Sobre estas ventanas temporales, el algoritmo extrae información valiosa calculando descriptores como:
* Varianza y desviación estándar.
* Promedio de variación absoluta.
* Covarianza, autocorrelación y covarianza cruzada.
* Coeficiente de correlación de Pearson.

## 🔍 ¿Qué buscamos?
El objetivo analítico es encontrar patrones numéricos que permitan diferenciar un estado cerebral de reposo frente a un evento ictal. Específicamente buscamos:
1. **Detección Automatizada:** Determinar un umbral de identificación (basado en un rango mínimo y máximo) y calcular el tiempo de retardo en la detección de la crisis para todos los canales evaluados.
2. **Modelado Probabilístico:** Analizar diagramas de caja e histogramas para determinar qué función de densidad de probabilidad (PDF) se ajusta mejor a la naturaleza de los datos.
3. **Optimización Algorítmica:** Evaluar la precondición, postcondición, invarianza y complejidad de cada rutina desarrollada. 

## 🛠️ Tecnologías y Herramientas
* Python (Librería `pyedflib` para ingesta de formatos `.edf`).
* Visualización de datos: Scatterplots, diagramas de caja e histogramas.
