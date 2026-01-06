# Evaluación de Modelos de Machine Learning para Engagement en Juegos Online

## Descripción del Proyecto

Este proyecto analiza el rendimiento de distintos modelos de machine learning en la predicción del nivel de engagement de jugadores de un videojuego online (`Low`, `Medium`, `High`).

El objetivo principal no es únicamente entrenar un modelo predictivo, sino comparar métricas entre diferentes enfoques y estudiar cómo influye la incorporación de nuevas variables derivadas, como clustering de comportamiento o reducción de dimensionalidad mediante PCA, en el rendimiento de los modelos.

El proyecto sigue un enfoque experimental y comparativo, similar al utilizado en entornos reales de data science.

---

## Objetivos

- Comparar distintos modelos de clasificación multiclase y evaluar cuál obtiene mejores métricas
- Analizar el impacto de añadir variables derivadas (clustering y PCA) al conjunto de datos original
- Evaluar si estas nuevas variables aportan información relevante o introducen ruido
- Utilizar métricas adecuadas para problemas de clasificación multiclase

---

## Tipo de Problema

- Aprendizaje supervisado  
- Clasificación multiclase

---

## Dataset

- Archivo: `online_gaming_behavior_insights.csv`
- Registros: 40.034 jugadores
- Variables: 13 variables originales (numéricas y categóricas)
- Valores nulos: no existen

El conjunto de datos incluye información demográfica, comportamiento de juego y progresión del jugador.  
La variable objetivo es el nivel de engagement (`Low`, `Medium`, `High`).

---

## Modelos Evaluados

- Regresión Logística (modelo baseline)
- Árboles de Decisión
- Comparación de configuraciones:
  - Modelos entrenados únicamente con variables originales
  - Modelos con variable adicional de clustering

---

## Pipeline de Trabajo

1. Análisis exploratorio de datos (EDA)
2. Preprocesado de datos:
   - Codificación de variables categóricas
   - Escalado de variables numéricas
   - División train / test
3. Entrenamiento y evaluación de modelos base
4. Incorporación de variables derivadas (clusters y PCA)
5. Comparación de métricas entre modelos y configuraciones

---

## Métricas de Evaluación

Las métricas utilizadas para la comparación de modelos son:

- **F1-score (macro)** como métrica principal
- **Accuracy** como métrica complementaria
- **Matriz de confusión** para el análisis detallado de errores entre clases

Estas métricas permiten evaluar el rendimiento de forma equilibrada en un problema de clasificación multiclase.

---

## Resultados

El análisis permite evaluar de forma comparativa:

- Qué modelo obtiene mejores métricas utilizando únicamente las variables originales
- Cómo varía el rendimiento al añadir información agregada mediante clustering
- El impacto de la reducción de dimensionalidad mediante PCA en la capacidad predictiva de los modelos

