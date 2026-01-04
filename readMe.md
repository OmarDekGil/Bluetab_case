# 🎮 Predicción del Engagement en Juegos Online mediante Machine Learning

## 📌 Descripción del Proyecto

Este proyecto tiene como objetivo desarrollar un **modelo de machine learning** capaz de predecir el **nivel de engagement (compromiso)** de los jugadores de un videojuego online a partir de sus patrones de comportamiento y características demográficas. Además, se analiza **qué variables influyen más** en el engagement, proporcionando información útil para estrategias de retención, diseño de juego y personalización.

El dataset utilizado está completamente limpio y estructurado, lo que permite centrarse directamente en el análisis y el modelado. Es un proyecto ideal tanto para **aprendizaje**, como para **portfolio profesional** o **preparación de entrevistas técnicas**.

---

## 🎯 Objetivos

* Predecir el **nivel de engagement del jugador** (`Low`, `Medium`, `High`) mediante aprendizaje supervisado
* Identificar los **factores clave** que influyen en el engagement
* Comparar distintos modelos de machine learning
* (Opcional) Segmentar a los jugadores según su comportamiento

---

## 🧠 Tipo de Problema

* **Aprendizaje supervisado**
* **Clasificación multiclase**

---

## 📂 Descripción del Dataset

* **Archivo:** `online_gaming_behavior_insights.csv`
* **Registros:** 40.034 jugadores
* **Variables:** 13
* **Tipos de datos:** Numéricos y categóricos
* **Valores nulos:** No existen

### Grupos de Variables

**Datos demográficos**

* Edad
* Género
* Localización

**Comportamiento de juego**

* Tiempo total de juego
* Frecuencia de sesiones
* Duración media de las sesiones

**Progresión del jugador**

* Nivel del jugador
* Logros desbloqueados

**Variable objetivo**

* Nivel de engagement (`Low`, `Medium`, `High`)

---

## 🛠️ Herramientas y Tecnologías

* Python
* Pandas y NumPy
* Matplotlib y Seaborn
* Scikit-learn
* SHAP (interpretabilidad de modelos)
* Jupyter Notebook

---

## 🔄 Pipeline de Machine Learning

### 1️⃣ Análisis Exploratorio de Datos (EDA)

* Distribución de los niveles de engagement
* Análisis de correlaciones
* Comparación de métricas por nivel de engagement
* Identificación de patrones y outliers

### 2️⃣ Preprocesado de Datos

* Codificación de variables categóricas (One-Hot Encoding)
* Escalado de variables numéricas (StandardScaler)
* División Train / Test (80% / 20%)
* Uso de Pipeline y ColumnTransformer

### 3️⃣ Modelos Entrenados

* Regresión Logística (baseline)
* Random Forest Classifier
* Gradient Boosting / XGBoost (opcional)

### 4️⃣ Métricas de Evaluación

* Accuracy
* F1-score (macro)
* Matriz de confusión
* ROC-AUC multiclase (opcional)

---

## 🔍 Importancia de Variables e Interpretabilidad

* Importancia de variables en Random Forest
* Coeficientes en Regresión Logística
* Valores SHAP para interpretación global y local

Preguntas clave que responde el proyecto:

* ¿Qué comportamientos influyen más en el engagement?
* ¿Es más importante jugar más tiempo o jugar con mayor frecuencia?
* ¿Las variables demográficas tienen impacto real?

---

## 📊 (Opcional) Segmentación de Jugadores

* Clustering con K-Means
* Selección del número óptimo de clusters (Elbow y Silhouette)
* Identificación de perfiles de jugadores
* Relación entre clusters y niveles de engagement

---

## 📁 Estructura del Proyecto

```
gaming-engagement-ml/
│
├── data/
│   └── online_gaming_behavior_insights.csv
│
├── notebooks/
│   ├── 01_eda.ipynb
│   ├── 02_clasificacion.ipynb
│   ├── 03_importancia_variables.ipynb
│   └── 04_clustering.ipynb
│
├── src/
│   ├── preprocessing.py
│   ├── train.py
│   └── evaluate.py
│
└── README.md
```

---

## 📈 Resultados Principales (por completar)

* Mejor modelo: *Pendiente*
* F1-score (macro): *Pendiente*
* Variables más influyentes: *Pendiente*

---

## 🚀 Posibles Mejoras Futuras

* Optimización de hiperparámetros (GridSearch / Optuna)
* Redes neuronales
* Predicción temporal del engagement
* Despliegue como API o dashboard interactivo

---

## 👤 Autor

**Omar Deknache Gil**

---

## 📜 Licencia

Proyecto con fines educativos y de investigación.
