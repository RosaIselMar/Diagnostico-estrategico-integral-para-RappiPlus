Proyecto RappiPlus | Análisis y preparación de datos con Python y SQL

Este repositorio contiene el desarrollo del proyecto RappiPlus, enfocado en la exploración, limpieza, transformación y análisis de datos para obtener información relevante sobre las operaciones, el comportamiento de los usuarios y el rendimiento de la plataforma.

El proyecto integra diferentes fuentes de información: archivos CSV y tablas almacenadas en una base de datos, con el propósito de preparar los datos, construir indicadores de negocio y generar insights que apoyen la toma de decisiones.

📂 Contenido del repositorio

1. Limpieza y preparación de datos

Se utilizaron tres datasets para evaluar la calidad de la información, identificar inconsistencias y generar conjuntos de datos limpios para su posterior análisis y visualización.

datasets/rappiplus_orders_raw.csv: Información de pedidos y transacciones.

datasets/rappiplus_catalog.csv: Información del catálogo de productos.

datasets/rappiplus_marketing_spend.csv: Información sobre inversión en marketing.

Objetivo:

- Evaluar la calidad de los datos.
- 
- Detectar valores nulos, duplicados e inconsistencias.
- 
- Validar tipos de datos y relaciones entre variables.
- 
- Identificar y evaluar valores atípicos (outliers).
- 
- Limpiar, transformar y estructurar los datasets.
- 
- Generar archivos depurados para su posterior análisis y construcción de un dashboard.

2. Análisis del comportamiento y conversión de usuarios

Para esta etapa se utilizó la tabla events, almacenada en una base de datos. La conexión se realiza directamente desde Jupyter Notebook mediante consultas SQL.

Tabla events: Contiene información sobre los eventos e interacciones de los usuarios dentro de la plataforma.

Objetivo del análisis:

-Analizar el recorrido de los usuarios dentro de la plataforma.

-Construir un funnel de conversión completo.

-Identificar los puntos de abandono durante el proceso.

-Calcular las tasas de conversión entre etapas.

-Detectar la etapa con mayor pérdida de usuarios (Drop-off).

3. Análisis de cohortes y retención de usuarios

Para esta etapa se utilizaron dos tablas adicionales, consultadas desde la base de datos:

Tabla users: Contiene información relacionada con el registro de los usuarios.

Tabla user_activity: Registra la actividad de los usuarios después de su registro.

Objetivo del análisis:

-Analizar el comportamiento de los usuarios a lo largo del tiempo.

-Construir cohortes según el periodo de registro.

-Calcular indicadores de retención de usuarios.

-Evaluar la evolución de la actividad después del registro.

-Identificar patrones de retención y oportunidades de mejora.

4. Análisis de experimento A/B – Checkout UI

Se utilizó el dataset:

datasets/experiment_checkout_ui.csv: Información correspondiente a un experimento A/B relacionado con la interfaz del proceso de checkout.

Objetivo del análisis:

-Evaluar los resultados del experimento.

-Comparar el comportamiento de los grupos de control y tratamiento.

-Analizar las tasas de conversión.

-Aplicar pruebas estadísticas para evaluar diferencias entre las variantes.

-Determinar si los cambios en la interfaz presentan mejoras significativas en la conversión.

📘 Cómo reproducir el análisis

Clona o descarga este repositorio.

Abre los notebooks correspondientes a cada etapa del proyecto.

Instala las librerías necesarias.

Ejecuta las celdas en orden.

Para los análisis que utilizan las tablas events, users y user_activity, configura la conexión a la base de datos desde Jupyter Notebook.

Importante: El acceso a la base de datos requiere las credenciales y parámetros de conexión correspondientes. Estos deben configurarse localmente y no incluirse directamente en el repositorio.

🛠️ Herramientas y tecnologías

-Python: Procesamiento y análisis de datos.

-Pandas: Limpieza, transformación y manipulación de datos.

-NumPy: Operaciones y validaciones numéricas.

-SQL: Consultas, uniones, agregaciones y análisis de datos almacenados en bases de datos.

-Matplotlib y Seaborn: Visualización y análisis exploratorio.

-Jupyter Notebook: Desarrollo y documentación de los análisis.

-Power BI: Construcción de dashboards e indicadores de negocio.

📊 Resultados esperados del proyecto

El desarrollo del proyecto permite obtener cuatro entregables principales:

-Datasets limpios: Información de pedidos, catálogo e inversión en marketing preparada para construir un dashboard en Power BI.

-Funnel de conversión: Identificación de las etapas del recorrido del usuario, tasas de conversión y principales puntos de abandono.

-Análisis de retención: Construcción de cohortes e identificación de patrones de comportamiento de los usuarios a lo largo del tiempo.

-Evaluación A/B: Análisis estadístico de los resultados del experimento de checkout para evaluar el impacto de los cambios en la interfaz.

💡 Habilidades desarrolladas

-Limpieza y preparación de datos (Data Cleaning).

-Análisis exploratorio de datos (EDA).

-Consultas y manipulación de bases de datos con SQL.

-Análisis de funnels de conversión.

-Análisis de cohortes y retención.

-Evaluación de experimentos A/B.

-Análisis estadístico e interpretación de resultados.

-Visualización de datos y construcción de dashboards.

-Generación de insights para la toma de decisiones.

-Documentar supuestos y limitaciones.

-Convertir hallazgos en recomendaciones de negocio.
