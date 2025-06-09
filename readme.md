# Análisis de Viralidad en Vídeos de YouTube

## DESCRIPCIÓN GENERAL

Este proyecto de visualización interactiva analiza los factores que influyen en la viralidad de los vídeos musicales de YouTube. A través de tres visualizaciones principales, se exploran patrones relacionados con la franja horaria de publicación, la antigüedad del canal y la categoría del contenido. El proyecto forma parte de la asignatura "Visualización de Datos" del Máster Universitario en Ciencia de Datos (UOC).

## VISUALIZACIONES INCLUIDAS

1. **Franja horaria óptima de publicación**  
   Explora qué franjas horarias locales maximizan la probabilidad de que un vídeo entre en Tendencias en menos de 24 horas, desglosado por categoría.

2. **Relación entre suscriptores, visualizaciones y antigüedad del canal**  
   Analiza cómo la antigüedad del canal condiciona el número de visualizaciones en las primeras 24 horas, a igualdad de número de suscriptores.

3. **Velocidad de viralización según la categoría**  
   Compara el tiempo medio que tardan los vídeos en hacerse virales (entrar en Tendencias), según su categoría y año de publicación (2017–2018).

## ESTRUCTURA DEL PROYECTO

- **data/**: Carpeta con el archivo de datos reducido (`youtube_master_dataset.csv`). Solo incluye las columnas necesarias para las visualizaciones.  
- **docs/**: Visualizaciones exportadas en formato HTML y PNG.  
- **notebooks/**: Notebook principal (`notebook.ipynb`) con el código completo de generación de visualizaciones.  
- **README.md**: Este archivo.  
- **requirements.txt**: Listado de dependencias necesarias para reproducir el entorno.

## INSTRUCCIONES DE EJECUCIÓN

1. Clonar el repositorio en local.  
2. Crear un entorno virtual y activarlo.  
3. Instalar dependencias con: `pip install -r requirements.txt`  
4. Abrir el notebook principal: `visualizaciones.ipynb`  
5. Ejecutar las celdas para generar las visualizaciones (opcional si ya están en `/docs`).

## TECNOLOGÍAS EMPLEADAS

- Python 3.10 o superior  
- Pandas, NumPy  
- Altair (para visualización interactiva)  
- Matplotlib, Seaborn  
- Jupyter Notebook

## PUBLICACIÓN INTERACTIVA

https://hernandezlopezai.github.io/youtube-viralidad-visualizaciones/

## LICENCIA

El código fuente de este proyecto está disponible bajo la licencia MIT (ver archivo LICENSE).

Los datos utilizados se basan en una versión modificada del siguiente conjunto de datos:

"YouTube Trending Videos Dataset", disponible en: https://www.kaggle.com/datasets/thedevastator/youtube-trending-videos-dataset  
Autor original: thedevastator (Kaggle)  
Se ha enriquecido y limpiado mediante procesos propios y el uso de la API de YouTube.  
Esta versión no contiene datos personales ni sensibles y se distribuye exclusivamente con fines educativos. Se recomienda dar crédito al autor original si se reutiliza.

## DICCIONARIO DE VARIABLES (Versión Reducida)

- `video_id`: ID único del vídeo  
- `title`: Título del vídeo  
- `channel_title`: Nombre del canal  
- `publish_date`: Fecha de publicación  
- `time_frame`: Franja horaria local de publicación  
- `category_name`: Categoría del vídeo  
- `views`: Número de visualizaciones  
- `channel_subscribers`: Nº de suscriptores del canal  
- `channel_age_days`: Edad del canal en días  
- `time_to_trend_hours`: Tiempo (en horas) hasta entrar en Tendencias  
- `year`: Año de publicación

El resto de columnas han sido eliminadas del dataset por no ser utilizadas en el análisis actual.
