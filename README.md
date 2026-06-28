# Google-Play-Store-apps-and-reviews-
# 📱 Análisis y Predicción de Éxito de Apps en Google Play Store

## 📖 Descripción General
Este proyecto realiza un análisis exhaustivo del mercado de aplicaciones de Android utilizando un conjunto de datos de más de 10,000 aplicaciones de la Google Play Store y sus reseñas de usuarios. El objetivo principal es extraer *insights* valiosos sobre las estrategias de categorización, monetización (tamaño y precio) y retención, para culminar en el desarrollo de modelos de Machine Learning capaces de predecir el éxito comercial y la calidad de una aplicación antes o durante su lanzamiento.

## 🎯 Objetivos del Proyecto
1. **Análisis Exploratorio de Datos (EDA):** Identificar qué categorías dominan el mercado y cuáles presentan áreas de oportunidad.
2. **Estrategia de Monetización y Diseño:** Evaluar cómo el tamaño (MB) y el precio de una aplicación afectan la calificación y aceptación de los usuarios.
3. **Análisis de Sentimiento:** Relacionar las reseñas de los usuarios con la polaridad de sus sentimientos (positivo, negativo, neutral) comparando aplicaciones gratuitas vs. de paga.
4. **Modelado Predictivo (Clasificación):**
   * Predecir la **rentabilidad/popularidad** de una app (clasificando si superará los 50 millones de instalaciones).
   * Predecir la **calidad o aceptación** (clasificando si obtendrá un Rating >= 4.0), aislando variables obvias como el número de reseñas para encontrar las características estructurales que realmente definen una buena app.

## 🛠️ Metodología y Flujo de Trabajo
* **Limpieza de Datos (Data Cleaning):** Tratamiento de valores nulos, conversión de tipos de datos, y uso de funciones lambda para limpiar caracteres especiales en precios e instalaciones (`,`, `+`, `$`).
* **Visualización de Datos:** Creación de gráficos de barras, histogramas y diagramas de dispersión (jointplots) para entender distribuciones y correlaciones.
* **Preprocesamiento para ML:** Codificación de variables categóricas (Label Encoding) y agrupación de versiones de Android por niveles de compatibilidad.
* **Machine Learning:** Implementación de modelos `RandomForestClassifier` abordando el desbalanceo de clases (`class_weight`) y optimización de hiperparámetros. Evaluación mediante reportes de clasificación, matrices de confusión y métricas ROC AUC.

## 📊 Hallazgos Clave (Insights)
* Categorías como *Family* y *Game* dominan el mercado en volumen, pero nichos específicos (como *Medical* o *Business*) presentan excelentes promedios de calificación.
* El modelo demostró que características como la **frecuencia de actualización (Last Updated)**, el **tamaño optimizado (Size)** y el nicho adecuado (**Category/Genres**) son predictores fundamentales del éxito, incluso antes de que la aplicación empiece a generar reseñas masivas.
* Las aplicaciones de paga tienen un umbral de exigencia mayor por parte de los usuarios, lo que se refleja en análisis de polaridad de sentimientos más polarizados.

## 💻 Tecnologías Utilizadas
* **Lenguaje:** Python
* **Manipulación de Datos:** Pandas, NumPy
* **Visualización:** Matplotlib, Seaborn
* **Machine Learning:** Scikit-Learn (`RandomForestClassifier`, `LabelEncoder`, `train_test_split`, métricas de evaluación)

## ✍️ Autor
**Hiram Cruz** - *Data Scientist*
[LinkedIn](https://www.linkedin.com/in/hiram-cruz-data-science)

--- 
*Nota: Este proyecto demuestra habilidades tanto analíticas como predictivas, orientadas a la toma de decisiones estratégicas en el desarrollo de software.*
