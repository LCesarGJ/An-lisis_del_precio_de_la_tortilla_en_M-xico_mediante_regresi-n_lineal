## Análisis del Precio de la Tortilla en México mediante Regresión Lineal
Descripción del Proyecto

Este proyecto analiza la evolución del precio de la tortilla en México utilizando modelos de regresión lineal.
El objetivo principal es evaluar la relación entre el precio por kilogramo y el paso del tiempo, así como estimar el precio promedio esperado para el siguiente año.

Se desarrolló un análisis completo que incluye:

Exploración inicial del dataset

Revisión de nulos y estructura

Visualización de tendencias

Matriz de correlación

Modelos de regresión lineal con sklearn y statsmodels

Evaluación del modelo mediante métricas y residuos

Predicción del precio para el siguiente año

Comparación entre precios reales y precios estimados por el modelo

El proyecto está pensado con fines educativos y como demostración de buenas prácticas en análisis de datos.

Dataset

El análisis utiliza un archivo llamado tortilla_prices.csv, el cual contiene las siguientes columnas:

State

City

Year

Month

Day

Store type

Price per kilogram

El dataset contiene información histórica sin valores nulos, lo que facilita un análisis directo sin necesidad de imputación.

Metodología

La estructura del análisis es la siguiente:

1. Exploración inicial

Se analizan:

Tipos de datos

Dimensiones

Estadísticos descriptivos

Calidad de datos (valores nulos)

2. Visualización

Se grafica el precio promedio por año para observar tendencias globales.

3. Correlación

Se genera un heatmap de correlaciones entre las variables numéricas.
Year presenta la correlación más fuerte con el precio.

4. Modelos de regresión

Se emplean dos enfoques:

Regresión con sklearn

Modelo multivariable utilizando:

Year

Month

Regresión con statsmodels

Modelo interpretable:

price ~ Year

5. Evaluación del modelo

Se utilizan métricas como:

R²

MSE

RMSE

MAE (para Statsmodels)

Se grafican precios reales vs predicciones, así como residuos.

6. Predicción del precio del siguiente año

El modelo lineal permite estimar el precio promedio esperado para el año siguiente, basado en la tendencia histórica general.

7. Comparación real vs. predicho

Se calcula:

Precio real promedio por año

Precio estimado por el modelo

Diferencia absoluta

Diferencia porcentual

Y se grafica la evolución comparativa.

Resultados Clave

El precio de la tortilla presenta una tendencia creciente a lo largo del tiempo.

La regresión lineal simple explica alrededor del 50% de la variabilidad del precio.

El precio real del último año no coincide exactamente con la predicción del modelo, lo cual es esperado en regresiones lineales, ya que ajustan una tendencia global y no forzosamente pasan por el último valor observado.

La predicción del modelo para el siguiente año se alinea con la tendencia estimada.

Conclusiones

El año es un predictor significativo del precio de la tortilla en México.

El modelo lineal captura adecuadamente la tendencia general, aunque no explica toda la variabilidad debido a factores no incluidos (estado, tipo de tienda, efectos regionales, estacionalidad local, entre otros).

El enfoque es adecuado como análisis introductorio o línea base.

Futuras mejoras podrían incluir modelos multivariables o modelos de series de tiempo que capturen estacionalidad y patrones no lineales.

Requisitos

Python 3.8+
Librerías utilizadas:

numpy

pandas

matplotlib

seaborn

scikit-learn

statsmodels

Autor

Luis César Guadarrama Jiménez
Data Science Specialist | Forecasting & Supply Chain
