TRAXIÓN - Modelo Predictivo de Churn de Conductores  
Autor: Mtra. Gabriela Durán Meza  
Fecha: Marzo 2025

==================================================
📌 Descripción del Proyecto
==================================================
Esta solución fue desarrollada como parte de una prueba técnica para la posición de Científico de Datos en TRAXIÓN. El objetivo principal es identificar a los conductores con alta probabilidad de retirarse de la empresa, utilizando datos sintéticos realistas que simulan quejas registradas por conductores a través de una app interna.

==================================================
📁 Archivos Incluidos
==================================================
1. 1synthetic_data_drivers.ipynb  
   - Generación de una base de datos sintética de más de 3000 registros.
   - Se incluyen variables sociodemográficas, laborales y de viajes.
   - En este repositorio, se considera una generacion de mensajes estándar empleando herrmientas de pandas y numpy.
   - La implementación de GenAI (LangChain + GPT-4o) para crear mensajes realistas de queja, se encuantra en el repositorio local, debido a que es una tecnología desarrollada con herramientas de OpenAI que funcionan on-line, en su lugar se muestra una generación regular de datos sinteticos con pandas y herramientas de numpy.

2. 2eda_drivers_churn.ipynb  
   - Análisis exploratorio de datos.
   - Evaluación de correlaciones y distribución de variables.
   - Visualización de patrones relevantes para el análisis de churn.

3. 3model_drivers_churn.ipynb  
   - Entrenamiento y evaluación de modelos de clasificación (Random Forest y Gradient Boosting).
   - Optimización con GridSearchCV y validación cruzada.
   - Métricas clave: accuracy, recall, F1-score, matriz de confusión.

4. Presentacion_Churn_Conductores.pptx.pdf  
   - Defensa técnica del proyecto en formato presentación.
   - Incluye objetivos, metodología, resultados, insights y recomendaciones de negocio.

==================================================
⚙️ Requisitos de Ejecución
==================================================
- Python >= 3.7  
- Recomendado: entorno virtual (virtualenv, conda)

Paquetes principales:
- pandas, numpy, matplotlib, seaborn
- scikit-learn

==================================================
💡 Instrucciones de Uso
==================================================
1. Clonar el repositorio en tu máquina local.
2. Ejecutar los notebooks en orden:
   - Primero: 1synthetic_data_drivers.ipynb
   - Luego: 2eda_drivers_churn.ipynb
   - Finalmente: 3model_drivers_churn.ipynb
3. Revisar la presentación para entender el enfoque general y los resultados.
4. Si se desea ejecutar el pipeline con generación de mensajes, se recomienda contar con una clave válida de OpenAI y acceso a modelos como GPT-4o.
5. Las notebooks 2 y 3 consumen el archivo driver_data_with_messages_fe.csv, este archivo contiene los mensajes generados por GenAI en la columna 'message'.

==================================================
📈 Próximos Pasos (Recomendaciones)
==================================================
- Implementar el pipeline en entorno offline usando un modelo LLM local.
- Evaluar el modelo con datos reales cuando estén disponibles.

==================================================
📬 Contacto
==================================================
Gabriela Durán Meza  
[igabypy@gmail.com / https://www.linkedin.com/in/igabypy/ / https://github.com/igabypy]


