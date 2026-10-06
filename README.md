# 📊 Spotify Charts: Tendencias musicales a escala global

> Análisis Exploratorio de datos (EDA) de Spotify Charts para estudiar tendencias 
> musicales y diferencias entre paises y continentes

![Captura Dashboard](https://github.com/thelifeofalvaro/eda-spotify/blob/main/imagenes/Dashboard_general.png "Pestaña General")

## 🎯 Objetivo

¿Existen diferencias en las características musicales de las canciones que alcanzan los rankings de Spotify según el país o la región?

Este proyecto explora los datos de Spotify Charts procedentes de 72 países para analizar tendencias musicales, comportamiento en los rankings y características de las canciones.

## 📊 Datos

El proyecto utiliza datos de Spotify Charts procedentes de 72 países.

El conjunto de datos utilizado contiene:

- 38.542 canciones
- 14.926 artistas
- 8.213 álbumes
- 72 países

Además de información sobre rankings, los datos incluyen diferentes
características musicales de las canciones, como:

- Danceability
- Energy
- Speechiness
- Acousticness
- Instrumentalness
- Liveness
- Valence
- Loudness
- Tempo
- Duration

## 🔄 Proceso de análisis

El proyecto se divide en cuatro etapas principales:

### 01. Preparación

Carga y preparación inicial de los datos para su posterior análisis.

### 02. Transformación

Limpieza, transformación y adaptación de los datasets para facilitar
el análisis.

### 03. Análisis exploratorio

Exploración de los datos mediante Python para identificar tendencias,
distribuciones, relaciones y diferencias entre regiones.

### 04. Visualización

Construcción de un dashboard interactivo en Power BI para explorar
los resultados.
```
Datos
  ↓
Preparación
  ↓
Transformación
  ↓
EDA
  ↓
Power BI
  ↓
Dashboard
```

## 📓 Notebooks

| Notebook | Contenido |
|---|---|
| `01. Preparacion`    | Preparación inicial de los datos |
| `02. Transformación` | Limpieza y transformación |
| `03. Eda_spotify`    | Análisis exploratorio y visualización

## 📊 Dashboard

Los resultados del análisis se presentan mediante un dashboard
interactivo desarrollado en Power BI.

### Vista general

![Captura Dashboard](https://github.com/thelifeofalvaro/eda-spotify/blob/main/imagenes/Dashboard_general.png "Pestaña General")

### Análisis por canción

![Captura Dashboard 2](https://github.com/thelifeofalvaro/eda-spotify/blob/main/imagenes/Dashboard_porcancion.png "Pestaña Por Canción")

## 🔎 Principales resultados

### Energy y Loudness

Se observa una correlación positiva alta entre energy y loudness
(≈ 0,82).

### Acousticness

acousticness presenta una relación negativa con energy
(≈ -0,65) y danceability (≈ -0,52).

### Danceability y Valence

Se observa una correlación positiva moderada entre danceability
y valence (≈ 0,48).

### 🗺️ Diferencias regionales

El análisis permite observar diferencias en las características musicales de las canciones según países y continentes.

## 🛠️ Tecnologías

*Análisis:* Python · Pandas · NumPy  
*Visualización:* Matplotlib · Seaborn  
*Business Intelligence:* Power BI · DAX

## 📁 Estructura del proyecto

```text
eda-spotify/
│
├── Dashboard/
│   └── Dashboard_spotify.pbix
│
├── Data/
│   └── enlace a datos.md
│
├── imagenes/
│   ├── Dashboard general
│   └── Dashboard por canción
│
├── Notebooks/
│   ├── 01. Preparación
│   ├── 02. Transformación
│   └── 03. Eda_spotify
│
└── README.md
```

# 11. Datos
Los datasets utilizados en el proyecto se encuentran alojados
externamente debido a su tamaño. Los enlaces de acceso están disponibles [aquí](Data/enlace_datos.md)

## 🎓 Contexto

Proyecto final de primer curso del Máster en Data & Analytics.

El proyecto reúne las distintas etapas del trabajo con datos: Preparación, transformación, análisis exploratorio y visualización mediante Power BI.
