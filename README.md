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
Nombre del Dataset: Uber Ride Analytics Dataset 2024

## Contexto
Este dataset contiene información detallada de operaciones de Uber durante el año 2024.

Incluye datos como:

- Fecha y Hora de cada reserva
- Estado del viaje (realizado, cancelado, interrumpuido)
- Tipo de vehículo que hizo el viaje
- Valoraciones del conductor y del pasajero
- Valor del viaje

## Variables de interés encontadas en el DataSet
| Tipo de dato |	Ejemplos de columnas|
|:------------|:--------------------|
| Tiempo y ubicación	|Date, Time, Pickup Location, Drop Location|
| Estado del viaje	|Booking Status (Completed, Cancelled, Incomplete, etc.)|
| Vehículo	|Vehicle Type (Go Mini, Go Sedan, Auto, UberXL, etc.)
| Financiero	|Booking Value, Payment Method (UPI, Cash, Credit Card, etc.)
| Calidad	| Driver Ratings, Customer Rating
| Cancelaciones	| Driver Cancellation Reason, Reason for cancelling by Customer |
| Viajes incompletos	| Incomplete Rides Reason|

# Diccionario de datos

## Tipo de variables

- **Numéricas continuas**: Son variables cuantitativas que pueden tomar infinitos valores dentro de un rango.
- **Numéricas discretas**: Son variables numéricas que cuentan elementos. Sólo toman valores enteros.
- **Categóricas nominales**: Representan categorías sin orden natural.
- **Categóricas ordinales**: Son categorías con un orden implícito.
- **Fecha/hora**: Representan momentos, intervalos o referencias cronológicas en el tiempo.

| Columna | dtype | Representa | Tipo|
|:------------|:------------|:---------|:------------|
| Date | str | Fecha de la reserva | Fecha/hora |
| Time | str | Hora de la reserva | Fecha/hora |
| Booking ID | str | Identificador único para cada viaje | Categórica nominal |
| Booking Status | str | Estado de la reserva (Completed, Cancelled by Customer, Cancelled by Driver, etc.) | Categórica nominal |
| Customer ID | str | Identificador único del cliente | Categórica nominal |
| Vehicle Type | str | Tipo de vehículo (Go Mini, Go Sedan, Auto, eBike/Bike, UberXL, Premier Sedan) | Categórica nominal |
| Pickup Location | str | Lugar donde inicia el viaje | Categórica nominal |
| Drop Location | str | Lugar donde finaliza el viaje | Categórica nominal |
| Avg VTAT | float64 | Tiempo promedio en minutos que tarda el conductor en llegar al punto de inicio | Numérica continua |
| Avg CTAT | float64 | Tiempo promedio en minutos que tarda el viaje desde donde inició hasta donde terminó | Numérica continua |
| Cancelled Rides by Customer | float64 | Marca si el cliente canceló el viaje | Booleana |
| Reason for cancelling by Customer | str | Motivo por el cual el cliente canceló el viaje | Categórica nominal |
| Cancelled Rides by Driver | float64 | Marca si el conductor canceló el viaje | Booleana |
| Driver Cancellation Reason | str | Motivo por el cual el conductor canceló el viaje | Categórica nominal |
| Incomplete Rides | float64 | Marca si el viaje se interrumpió | Boolean |
| Incomplete Rides Reason | str | Motivo por el cual el viaje se interrumpió | Categórica nominal |
| Booking Value | float64 | Importe del viaje | Numérica continua |
| Ride Distance | float64 | Distancia del viaje en Km | Numérica continua|
| Driver Ratings | float64 | Puntuación dada por el cliente al conductor (1-5 con decimales) | Categórica Ordinal |
| Customer Rating | float64 | Puntuación dada por el conductor al cliente (1-5 con decimales) | Categórica Ordinal |
| Payment Method | str | Método de pago usado para el viaje | Categórica nominal | 


----
Ideas y preguntas de análisis sobre el dataset
- ¿Cómo varía la demanda de viajes según el horario del día?
- ¿Existen horarios en los que se concentran más solicitudes de viajes?
- ¿Qué diferencias pueden observarse entre los patrones de demanda de días hábiles y fines de semana?
- ¿Existen zonas con una mayor concentración de solicitudes de viaje?
- ¿Cómo se comportan los distintos tipos de vehículos en términos de ingresos generados?
- ¿Qué tipos de vehículos presentan mayores tasas de cancelación?
- ¿Existen diferencias en los tiempos de espera según el tipo de vehículo solicitado?
- ¿Cómo se distribuyen los montos facturados por viaje?
- ¿Qué relación existe entre la distancia recorrida y el valor del viaje?
- ¿Existen franjas horarias con mayor facturación total?
- ¿Cómo varían las cancelaciones según el horario y el nivel de demanda?
- ¿Cuáles son las razones de cancelación más frecuentes registradas en el dataset?
- ¿Qué tipos de vehículos presentan mayores cancelaciones por parte de los conductores?
- ¿Qué relación existe entre el tiempo de espera y la calificación otorgada por los clientes?
- ¿Cómo impactan las cancelaciones o incidencias en las valoraciones de los usuarios?
- ¿Existen diferencias en las calificaciones promedio según el tipo de vehículo utilizado?
----

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
├── tp1.ipynb    # Cuaderno principal
├── data/        # (Opcional) Datos utilizados
├── LICENSE      # Archivo de licencia
└── README.md    # Este archivo
```



### Contribuciones

Este proyecto es un trabajo práctico académico. Por favor, contactar al autor para cualquier sugerencia o colaboración.

### Licencia

Este proyecto se distribuye bajo la licencia MIT
Ver el archivo LICENSE para más detalles.
