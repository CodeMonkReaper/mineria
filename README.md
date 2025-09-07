# Proyecto de Minería de Datos: Predicción Meteorológica en Australia 🌦️

## 📄 Descripción del Proyecto

Este proyecto de minería de datos tiene como objetivo principal analizar y modelar registros meteorológicos históricos de Australia para generar **modelos predictivos** y **obtener insights de negocio** valiosos. El enfoque está en cómo las predicciones de temperatura y lluvia pueden ayudar a los sectores agrícola, energético y de seguros a tomar decisiones estratégicas, optimizar recursos y mitigar riesgos asociados a la variabilidad climática.

El proyecto sigue la metodología **CRISP-DM** y se documenta el proceso completo, desde la comprensión del problema hasta la evaluación y las recomendaciones para el despliegue.

## 🎯 Objetivos de Negocio

El análisis de los datos se orientó a resolver problemas clave en la industria:

* **Reducir costos operativos** asociados a pronósticos imprecisos.
* **Aumentar los ingresos** mediante una mejor planificación en la agricultura y la generación de energía renovable.
* **Mejorar la satisfacción del cliente** en productos de seguros paramétricos al minimizar las reclamaciones falsas.

---

## ⚙️ Metodología

La solución se desarrolló siguiendo un pipeline de minería de datos que abarca las siguientes fases:

1.  **Comprensión del Negocio y de los Datos:** Se definió el problema, se identificaron los objetivos de negocio y se analizaron las fuentes de datos (archivos CSV).
2.  **Preparación de los Datos:** Se aplicaron técnicas de limpieza, imputación de datos faltantes (mediana y moda), y transformaciones como la estandarización de nombres de columnas y el escalado de variables con `StandardScaler`.
3.  **Análisis Exploratorio de Datos (EDA):** Se estudiaron las distribuciones de variables, se identificaron valores atípicos (outliers) mediante el método IQR y se visualizó la correlación entre las variables.
4.  **Modelado y Aplicación de Técnicas:** Se implementaron diversas técnicas de Machine Learning:
    * **Regresión:** `LinearRegression` y `DecisionTreeRegressor` para predecir la temperatura máxima (`maxtemp`).
    * **Clasificación:** `Naive Bayes` y `DecisionTreeClassifier` para predecir si lloverá al día siguiente (`RainTomorrow`).
    * **Clustering:** `K-Means` para segmentar perfiles climáticos.
    * **Dimensionalidad:** `PCA` para reducir las variables y facilitar la visualización.

---

## 📈 Evaluación y Resultados

Los modelos se validaron con métricas específicas para garantizar su rendimiento.

* **Regresión (`DecisionTreeRegressor`):** Se logró una **precisión** en la predicción de la temperatura con un MAE de aproximadamente 2.25 °C y un coeficiente de determinación R² de 0.810.
* **Clasificación (`Naive Bayes`):** Se obtuvo una **precisión del 80%** y un **ROC AUC de 0.784**, lo que indica una buena capacidad para discriminar entre días con y sin lluvia.

---

## 🛠️ Tecnologías

* **Jupyter Notebook:** Entorno de desarrollo para el análisis.
* **Python:** Lenguaje de programación principal.
* **Scikit-learn:** Librería para los modelos de Machine Learning.
* **Pandas & NumPy:** Manipulación y análisis de datos.
* **Matplotlib & Seaborn:** Visualización de datos.

---

## 🚀 Siguientes Pasos

Se recomienda continuar el desarrollo del proyecto con las siguientes acciones:

* **Escalado Geográfico:** Replicar el pipeline en otras regiones de Australia.
* **Modelos Avanzados:** Probar modelos de ensamble como **stacking** (por ejemplo, combinando Random Forest y SVM) para mejorar la predicción de eventos extremos.
* **Analítica Prescriptiva:** Vincular las predicciones a recomendaciones automatizadas para la toma de decisiones.

---

## 👨‍💻 Autor

* **Luis Salamanca**

Si tienes alguna pregunta o sugerencia, no dudes en abrir una _issue_ en este repositorio.
