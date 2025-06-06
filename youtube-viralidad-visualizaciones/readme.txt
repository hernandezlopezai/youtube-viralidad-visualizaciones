TÍTULO: Análisis de Viralidad en Vídeos de YouTube

DESCRIPCIÓN GENERAL:
Este proyecto de visualización interactiva analiza los factores que influyen en la viralidad de los vídeos musicales de YouTube. A través de tres visualizaciones principales, se exploran patrones relacionados con la franja horaria de publicación, la antigüedad del canal y la categoría del contenido. El proyecto forma parte de la asignatura "Visualización de Datos" del Máster Universitario en Ciencia de Datos (UOC).

VISUALIZACIONES INCLUIDAS:

1. Franja horaria óptima de publicación:
   Explora qué franjas horarias locales maximizan la probabilidad de que un vídeo entre en Tendencias en menos de 24 horas, desglosado por categoría.

2. Relación entre suscriptores, visualizaciones y antigüedad del canal:
   Analiza cómo la antigüedad del canal condiciona el número de visualizaciones en las primeras 24 horas, a igualdad de número de suscriptores.

3. Velocidad de viralización según la categoría:
   Compara el tiempo medio que tardan los vídeos en hacerse virales (entrar en Tendencias), según su categoría y año de publicación (2017-2018).

ESTRUCTURA DEL PROYECTO:

- data/: Carpeta con los archivos de datos ya procesados (formato CSV).
  Nota: El conjunto de datos ha sido reducido a las columnas necesarias para generar las visualizaciones, con el fin de optimizar su tamaño. No se incluye el proceso completo de limpieza para evitar redundancias.

- notebooks/: Notebook con el código de limpieza mínima, cálculo de métricas y visualizaciones (Jupyter).

- docs/: Carpeta donde se generan las visualizaciones exportadas (formato PNG y HTML).

- README.txt: Este archivo, con información general del proyecto.

- requirements.txt: Listado de dependencias necesarias para reproducir el entorno.

INSTRUCCIONES DE EJECUCIÓN:

1. Clonar el repositorio en local.
2. Crear un entorno virtual y activarlo.
3. Instalar dependencias con: pip install -r requirements.txt
4. Abrir el notebook principal: notebooks/visualizaciones_definitivo.ipynb
5. Ejecutar las celdas para generar las visualizaciones.

TECNOLOGÍAS EMPLEADAS:

- Python 3.10 o superior
- Pandas, NumPy
- Altair (para visualización interactiva)
- Matplotlib, Seaborn
- Jupyter Notebook
- YouTube Data API v3 (para enriquecer el conjunto de datos original)

VÍDEO EXPLICATIVO:
(Enlace al vídeo cuando esté disponible)

PUBLICACIÓN INTERACTIVA (opcional):
(Enlace a Observable o Tableau Public, si se publica)

LICENCIA:

El código fuente de este proyecto está disponible bajo la licencia MIT (ver archivo LICENSE).

Los datos utilizados se basan en una versión modificada del siguiente conjunto de datos:

"YouTube Trending Videos Dataset", disponible en:
https://www.kaggle.com/datasets/thedevastator/youtube-trending-videos-dataset

Autor original: thedevastator (Kaggle)
Se ha enriquecido y limpiado mediante procesos propios y el uso de la API de YouTube.
Esta versión no contiene datos personales ni sensibles y se distribuye exclusivamente con fines educativos. Se recomienda dar crédito al autor original si se reutiliza.

DICCIONARIO DE VARIABLES (versión reducida):

video_id: Identificador único del vídeo en YouTube.
title: Título del vídeo.
channel_title: Nombre del canal.
category_name: Categoría del vídeo (ej. "Music", "Entertainment").
time_frame: Franja horaria local en la que se publicó el vídeo.
views: Número de visualizaciones.
channel_subscribers: Suscriptores del canal en el momento de publicación.
time_to_trend_hours: Tiempo (en horas) que tardó el vídeo en entrar en Tendencias.
channel_age_days: Antigüedad del canal en días.
publish_date: Fecha de publicación del vídeo.
