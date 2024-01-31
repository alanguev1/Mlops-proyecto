(https://raw.githubusercontent.com/alanguev1/Mlops-proyecto/master/clean_datasets/steam.png)


# Proyecto MLOps: Sistema de Recomendación de Videojuegos para Usuarios de Steam.

## Descripción del proyecto
Este proyecto tiene como objetivo crear un sistema de recomendación de los juegos basado en los datos suministrados por la plataforma. Se llevaran acabo 3 diferentes procesos, desde la extracción y tratamiento de los datos pasando por un análisis de los mismos hasta la implementación del sistema de recomendación. Se desarrolló un caso de negocio real utilizando conjuntos de datos públicos de la industria de videojuegos, específicamente de la plataforma en línea STEAM. 

## Objetivos
Creación del primer modelo de Machine Learning (end to end) que resuelva un problema de negocio en Steam, a través de un enfoque que involucra tareas de Data Engineering (ETL, EDA, API) hasta la implementación del ML. Se busca lograr un rápido desarrollo y tener un Producto Mínimo Viable (MVP).

# Etapa de ingeniería de datos
En esta etapa de ingeniería de datos se realizó un proceso de ETL, extracción, transformación y carga donde se recibieron 3 archivos JSON con información acerca de los videjuegos, los jugadores y las reseñas de estos.

Link: 

Fuente de los datos: https://drive.google.com/drive/folders/1HqBG2-sUkz_R3h1dZU5F2uAzpRn7BSpj

# Etapa de análisis de datos
En esta etapa se realizo el EDA, analisis exploratorio de datos donde empezamos con una conversión de los datos verificando datos nulos, duplicados, outliers y el formato de los datos para posteriormente realizar el análisis de estos mediante graficos.

Link: 

# Sistema de recomendación
Una vez completadas las etapas anteriores, los datos se encuentran preparados para las respectivas funciones y el sistema de recomendación los cuales podrán ser consultados mediante el framework FastAPI.

Linkl FastAPI :

- def developer( developer: str ): Devuelve la cantidad de items y porcentaje de contenido Free por año según empresa desarrolladora.

- def user_data( user_id: str ): Devuelve la cantidad de dinero gastado por el usuario y el porcentaje de recomendación.

- def user_for_genre( genre: str ): Devuelve el usuario que acumula más horas jugadas para el género dado y una lista de la acumulación de horas jugadas por año de lanzamiento.

- def best_developer_year( year: int): Devuelve el top 3 de desarrolladores con juegos mas recomendados por usuarios para el año dado.

- def developer_reviews_analysis( developer: str): Según el desarrollador, se devuelve un diccionario con el nombre del desarrollador como llave y una lista con la cantidad total de registros de reseñas de usuarios que se encuentren categorizados con un análisis de sentimiento como valor positivo o negativo.
Realizar un Modelo de Machine learning que retorne una lista de 5 juegos similares a uno suministrado en un endpoint.

- def game_recommendation( product_id: int): Ingresando el id de producto, devuelve una lista con 5 juegos recomendados similares al ingresado.

# Tecnologias
- Python <img src="clean_datasets/logopython.png" alt="Python" width="20"/>
- Pandas <img src="clean_datasets/logopandas.png" alt="Python" width="20"/>
- Matplotlib <img src="clean_datasets/logompl.png" alt="Python" width="20"/>
- Numpy <img src="clean_datasets/logonumpy.svg" alt="Python" width="20"/>
- Sklearn <img src="clean_datasets/logosk.png" alt="Python" width="20"/>
- FastAPI <img src="clean_datasets/logofastapi.png" alt="Python" width="20"/>
