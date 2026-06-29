# Sistema de recomendaciones de películas

Este proyecto implementa un sistema recomendador de películas usando metadatos del dataset MovieLens/TMDB.

## Archivos principales

- `sistema_recomendaciones_peliculas.ipynb`: notebook principal del proyecto.
- `data/movies_metadata.csv`: metadatos de películas.
- `data/keywords.csv`: palabras clave de películas.
- `requirements.txt`: dependencias necesarias.

## Funcionalidades

El notebook incluye:

- Carga de datos.
- Limpieza de identificadores.
- Unión de `movies_metadata.csv` con `keywords.csv`.
- Extracción de géneros y palabras clave.
- Creación de una "sopa" de contenido.
- Vectorización con `CountVectorizer`.
- Cálculo de similitud coseno.
- Recomendador básico por similitud.
- Recomendador mejorado con filtro de popularidad.
- Calificación ponderada estilo IMDb.

## Instalación

Crear entorno virtual:

```bash
python -m venv venv
```

Activar entorno en Windows:

```bash
venv\Scripts\activate
```

Activar entorno en Mac/Linux:

```bash
source venv/bin/activate
```

Instalar dependencias:

```bash
pip install -r requirements.txt
```

## Ejecución

Abrir el notebook:

```bash
jupyter notebook sistema_recomendaciones_peliculas.ipynb
```

También se puede ejecutar en Google Colab subiendo el notebook y los archivos CSV.

## Conclusión

El proyecto demuestra cómo construir un sistema recomendador basado en contenido. Además, se mejora la calidad de las recomendaciones al combinar similitud con una calificación ponderada que toma en cuenta popularidad y número de votos.