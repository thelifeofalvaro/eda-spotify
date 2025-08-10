# 📊 Análisis de Tendencias Musicales en Spotify
## 1. Introducción
   
  Este proyecto analiza datos de Spotify Charts (A nivel Global en cada uno de los 72 paises con TOP propio) para identificar tendencias, patrones y diferencias en la música a   nivel global y regional. El objetivo es comprender cómo varían las características musicales entre países y continentes, y cómo se comportan las canciones en el tiempo según   su popularidad.
El trabajo combina el uso de Python (para limpieza, tratamiento de datos y análisis exploratorio) y Power BI (para un dashboard interactivo que permita la visualización dinámica de resultados)

## 2. Datos y Metodología

Fuente de datos:
universal_top_spotify_songs.csv - Dataset con toda la información relativa a las canciones y sus caracteristicas:
continents2.csv" - Dataset con información geográfica.
spotify_dataset_final.csv – Dataset que ha quedado tras fusionar y limpiar los dos anteriores. Incluye: Información de canciones y artistas, rankings diarios globales y por país, atributos musicales (danceability, energy, speechiness, acousticness, instrumentalness, liveness, valence, loudness, tempo, duration).

Una vez teniamos el dataset final, se ha procedido a afinar la limpieza de datos, y se han realizado las transformaciones pertinentes (por ejemplo conversión de duración de mm:ss a valor decimal en minutos (duration_decimal)), para facilitar el analisis. Se han creado métricas como promedio de ranking, recuento de apariciones y agregaciones por continente, etc...

Herramientas utilizadas:

Python (Pandas, Matplotlib, Seaborn, NumPy).

Power BI (medidas DAX, relaciones, slicers y visualizaciones interactivas).

## 3. Análisis Descriptivo
📌 Métricas clave:
Canciones únicas: 38,542 (dataset completo)

Artistas únicos: 14,926 (dataset completo)

Álbumes únicos: 8,213 (dataset completo)

📌 Escalas musicales:
Escala mayor predominante en Asia (65%) y Oceanía (62%).

Escala menor más frecuente en África (58%) y América (55%).

Europa con un reparto equilibrado (mayor 51%, menor 49%).

📌 Características musicales por continente:
Continente	Danceability	Energy	Speechiness	Acousticness	Instrumentalness	Liveness	Valence
África	0.73	0.68	0.14	0.26	0.02	0.29	0.54
América	0.71	0.70	0.15	0.21	0.03	0.27	0.57
Asia	0.68	0.66	0.11	0.31	0.01	0.23	0.61
Europa	0.70	0.69	0.13	0.28	0.02	0.25	0.59
Oceanía	0.75	0.72	0.13	0.19	0.03	0.24	0.60

## 4. Análisis Relacional
El análisis de correlación en Python reveló:

Energy y loudness: correlación positiva alta (~0.82).

Acousticness correlaciona negativamente con energy (-0.65) y danceability (-0.52).

Valence y danceability: correlación positiva moderada (~0.48).

## 5. Visualizaciones Destacadas (Dashboard)

Canciones, albumes y artistas unicos (permitiendo filtar a nivel global, por continente y pais)

Top 10 de canciones más populares

Claves musicales más usadas

Artistas con más apariciones como artitas principal

Distribución de escala musical y contenido explicito por canción

Caracteristicas por canción (nombre  del album al que pertenece, arstista princial y colaboradores, fecha de lanzamiento, asi como las caracteristicas musicales)

## 6. Conclusiones
Oceanía y África muestran perfiles musicales opuestos: alta energía y bailabilidad vs. mayor presencia de acústica y menor tempo.

Las canciones con alta energía suelen tener mayor volumen percibido, confirmando la relación energy–loudness.

El uso de escalas mayores y menores parece tener un patrón geográfico consistente.

El dashboard interactivo permite explorar y validar hipótesis en tiempo real, algo que con análisis estáticos sería más limitado.

## 7. Posibles Aplicaciones
Marketing musical: campañas adaptadas a tendencias regionales.

Curación de playlists: contenido personalizado por región.

Estudios culturales: relación entre música y contexto sociocultural.

## 8. Vista previa del Dashboard

![Captura Dashboard](https://github.com/thelifeofalvaro/eda-spotify/blob/main/imagenes/Dashboard_general.png "Pestaña General")
![Captura Dashboard 2](https://github.com/thelifeofalvaro/eda-spotify/blob/main/imagenes/Dashboard_porcancion.png "Pestaña Por Canción")

## 9. 💻 Requisitos técnicos
Python 3.x
Visual Studio Code
Power BI Desktop

Librerías: pandas, numpy, matplotlib, seaborn

💡 Incluye en el repositorio el Notebook con el análisis en Python y el archivo .pbix para que cualquiera pueda explorar el dashboard.
