Este proyecto aborda un desafío de Big Data, analizar 3 millones de [reseñas de libros de Amazon obtenidos de Kaggle](https://www.kaggle.com/datasets/mohamedbakhet/amazon-books-reviews/data), un conjunto de datos de más de `2.6 GB`. 

El objetivo principal es **construir y evaluar un modelo de Machine Learning** capaz de **clasificar automáticamente el sentimiento** de una reseña como `"Positivo" (1.0)` o `"Negativo" (0.0).`

Para manejar este volumen de datos, el proceso se realiza con **Apache Spark (PySpark)**. El cuaderno "PortafolioAnalisisBigData.ipynb" documenta el flujo de trabajo completo:

1. **EDA:** Entendimiento de la composición de los archivos de los que se extraerá la información, así como la calidad de los datos para delimitar un alcance con el modelo a desarrollar. Usando la herramienta Tableau.

2. **ETL:** Carga, limpieza y unión de los datos de reseñas y metadatos de los libros.

3. **Feature Engineering:** Conversión del texto de las reseñas (NLP) y las categorías de los libros en características numéricas que el modelo pueda entender.

4. **Modelado:** Se entrenan dos modelos, Regresión Logística y Random Forest, para comparar su rendimiento. Utilizando una técnica de ponderación de clases para ayudar al Random Forest a manejar el desbalance entre reseñas.

5. **Evaluación:** Se evalúan los modelos usando métricas como Precisión, F1-Score.

6. **Visualización:** Se exportan los resultados para su visualización en Tableau.
