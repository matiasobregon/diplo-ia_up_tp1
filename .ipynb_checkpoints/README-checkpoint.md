<p align="left">
  <img src="https://img.shields.io/badge/Curso-Diplomatura%20en%20IA-blue?style=flat" alt="Diplomatura en IA">
  <img src="https://img.shields.io/badge/Año-2026-green?style=flat" alt="Año 2026">
  <img src="https://img.shields.io/badge/Universidad-Universidad%20de%20Palermo-purple?style=flat" alt="Universidad de Palermo">
  <img src="https://img.shields.io/badge/Autor-Matux-orange?style=flat" alt="Autor: Matux">
  <img src="https://img.shields.io/badge/Jupyter-F37626.svg?style=flat&logo=Jupyter&logoColor=white" alt="Jupyter">
  <img src="https://img.shields.io/badge/Python-3.9%2B-blue?style=flat&logo=python&logoColor=white" alt="Python 3.9+">
</p>

# Proyecto: Trabajo Práctico #1

```text
Proyecto: Trabajo Práctico #1
Carrera: Diplomatura en IA
Año: 2026
Universidad: Universidad de Palermo
Autor: Matías Obregón
```

# Objetivo
El objetivo del presente trabajo es el de desarrollar un análisis exploratorio de datos (EDA) a partir de un dataset de libre elección.
Se espera que, mediante el tratamiento, limpieza y visualización de los datos, se puedan responder un conjunto de hipótesis previamente definidas y extraer conclusiones relevantes.

# Acerca del Dataset
> 2024 Delitos CABA
> 
> Fuente: [https://data.buenosaires.gob.ar/dataset/delitos/resource/49f58c2e-21d7-4766-84e0-4bb753d28478](https://data.buenosaires.gob.ar/dataset/delitos/resource/49f58c2e-21d7-4766-84e0-4bb753d28478)

## Contexto
Este DataSet contiene fecha, hora y ubicación de los homicidios, hurtos (sin violencia), lesiones y robos (con violencia) que ocurrieron en el ámbito de la Ciudad de Buenos Aires durante el año 2024.

Incluye datos como:

- Fecha del evento
- Tipo de delito
- Subtipo de delito
- Ubicación
- Barrio/Comuna

## Variables de interés encontadas en el DataSet

| Variable                     | Por qué es relevante                                                                              |
| ---------------------------- | ------------------------------------------------------------------------------------------------- |
| `tipo` / `tipo_delito`       | Es probablemente la variable criminal principal. Permite analizar distribución delictiva general. |
| `subtipo` / `subtipo_delito` | Agrega granularidad al análisis                                                                   |
| `franja` / `franja_horaria`  | Para análisis temporal. Posibilita estudiar horarios críticos.                                    |
| `fecha`                      | Permite análisis cronológico, tendencias y estacionalidad.                                        |
| `dia`                        | Útil para comparar comportamiento entre días hábiles y fines de semana.                           |
| `mes`                        | Permite detectar variaciones mensuales o estacionales.                                            |
| `barrio`                     | Variable geográfica clave para concentración delictiva.                                           |
| `comuna`                     | Similar a barrio, pero más agregada y útil para análisis comparativos.                            |
| `uso_arma`                   | Relevante para caracterizar gravedad/modalidad de delitos.                                        |
| `uso_moto`                   | Potencialmente relevante si hay delitos asociados a uso de motocicletas.                          |
| `cantidad`                   | Es la métrica cuantitativa principal del dataset.                                                 |
| `latitud` / `longitud`       | Habilitan análisis espacial y mapas (según calidad de la informacíón).                            |


# Diccionario de datos

## Tipo de variables

- **Numéricas continuas**: Son variables cuantitativas que pueden tomar infinitos valores dentro de un rango.
- **Numéricas discretas**: Son variables numéricas que cuentan elementos. Sólo toman valores enteros.
- **Categóricas nominales**: Representan categorías sin orden natural.
- **Categóricas ordinales**: Son categorías con un orden implícito.
- **Fecha/hora**: Representan momentos, intervalos o referencias cronológicas en el tiempo.

| Nombre         | Tipo      | Tipo estadístico   | Descripción                                            |
| -------------- | --------- | ------------------ | ------------------------------------------------------ |
| id-mapa        | integer   | Numérica discreta  | Identificador único                                    |
| Año            | integer   | Numérica discreta  | Año en el que se registró el evento                    |
| Mes            | string    | Categórica ordinal | Mes en que ocurrió el evento                           |
| Dia            | string    | Categórica ordinal | Día de la semana en que ocurrió el evento              |
| Fecha          | date      | Fecha/hora         | Fecha exacta del evento                                |
| franja_horaria | integer   | Categórica ordinal | Franja horaria en la que ocurrió el evento             |
| tipo_delito    | string    | Categórica nominal | Clasificación del tipo de delito                       |
| subtipo_delito | string    | Categórica nominal | Subtipo del delito, más específico                     |
| uso_arma       | string    | Categórica nominal | Indicador de uso de arma (SI/NO)                       |
| uso_moto       | string    | Categórica nominal | Indicador de uso de moto en el evento (SI/NO)          |
| barrio         | string    | Categórica nominal | Barrio donde ocurrió el evento                         |
| comuna         | number    | Numérica discreta  | Comuna donde ocurrió el evento                         |
| lat            | geo_point | Numérica continua  | Latitud geográfica donde ocurrió el evento             |
| long           | geo_point | Numérica continua  | Longitud geográfica donde ocurrió el evento            |
| cantidad       | number    | Numérica discreta  | Número de eventos registrados en esa ubicación y fecha |




## Metodología aplicada
lorem ipsum

## Conclusiones y hallazgos relevantes
lorem ipsum

# Requisitos Previos




Para ejecutar este cuaderno sin inconvenientes, necesitarás:

- **Python** 3.9 o superior
- **Jupyter Notebook** o **JupyterLab**
- Opcional: **Visual Studio Code** con la extensión de Jupyter

### Estructura del Proyecto
```text
/
├── tp1_desarrollo.ipynb    # Cuaderno principal
├── data/                   # Repositorio de datos
|   └───delitos_2024.csv    # Archivo de datos CSV
├── LICENSE                 # Archivo de licencia
└── README.md               # Este archivo
```



### Contribuciones

Este proyecto es un trabajo práctico académico. Por favor, contactar al autor para cualquier sugerencia o colaboración.

### Licencia

Este proyecto se distribuye bajo la licencia MIT
Ver el archivo LICENSE para más detalles.
