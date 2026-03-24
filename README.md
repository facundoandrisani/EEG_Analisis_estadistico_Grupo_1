# 📊 Detección de Crisis Epilépticas: Análisis Estadístico en el Dominio del Tiempo

[cite_start]Este proyecto se centra en el análisis temporal de señales electroencefalográficas (EEG) para identificar y caracterizar crisis epilépticas mediante el uso de descriptores estadísticos[cite: 3]. [cite_start]Se utiliza la base de datos **CHBMIT Scalp EEG Database** de PhysioNet[cite: 5].

## 🎯 ¿Qué hace este proyecto?
[cite_start]El flujo de trabajo segmenta las señales continuas de EEG en tres bloques temporales fundamentales: 2 minutos antes de la crisis (Before), la crisis en sí, y 2 minutos después (After) [cite: 18, 22-24]. Sobre estas ventanas temporales, el algoritmo extrae información valiosa calculando descriptores como:
* [cite_start]Varianza y desviación estándar[cite: 28].
* [cite_start]Promedio de variación absoluta[cite: 28].
* [cite_start]Covarianza, autocorrelación y covarianza cruzada[cite: 28].
* [cite_start]Coeficiente de correlación de Pearson[cite: 28].

## 🔍 ¿Qué buscamos?
El objetivo analítico es encontrar patrones numéricos que permitan diferenciar un estado cerebral de reposo frente a un evento ictal. Específicamente buscamos:
1. [cite_start]**Detección Automatizada:** Determinar un umbral de identificación (basado en un rango mínimo y máximo) y calcular el tiempo de retardo en la detección de la crisis para todos los canales evaluados[cite: 29, 30].
2. [cite_start]**Modelado Probabilístico:** Analizar diagramas de caja e histogramas para determinar qué función de densidad de probabilidad (PDF) se ajusta mejor a la naturaleza de los datos[cite: 31, 32].
3. [cite_start]**Optimización Algorítmica:** Evaluar la precondición, postcondición, invarianza y complejidad de cada rutina desarrollada[cite: 35]. 

## 🛠️ Tecnologías y Herramientas
* [cite_start]Python (Librería `pyedflib` para ingesta de formatos `.edf`)[cite: 6].
* [cite_start]Visualización de datos: Scatterplots, diagramas de caja e histogramas[cite: 31, 33].
