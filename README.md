# Análisis Distribuido de Movilidad Urbana con PySpark 🚍📊

Este proyecto aplica los fundamentos de Apache Spark para analizar datos simulados de movilidad urbana con un enfoque distribuido. Se trabaja con datos GPS de transporte público para obtener insights clave sobre rutas congestionadas, horarios pico y zonas con mayor flujo de vehículos.

## 📁 Dataset

El dataset utilizado simula registros de viajes con las siguientes columnas:

- `vehiculo_id`: Identificador del vehículo.
- `hora_salida`: Hora del día en formato 24h.
- `zona_origen`: Zona donde inicia el viaje.
- `zona_destino`: Zona donde termina el viaje.
- `tiempo_viaje_min`: Duración estimada del viaje.

📌 *Formato*: CSV  
📌 *Tamaño*: 100,000 registros (simulados)

## ⚙️ Tecnologías utilizadas

- **Apache Spark** (PySpark)
- **Pandas** y **Seaborn** para visualización
- **Jupyter Notebook** con **VS Code**

## 🔍 Objetivos del análisis

- Identificar las **rutas con mayor congestión**.
- Detectar los **horarios con más viajes**.
- Determinar las **zonas con más entradas y salidas** de vehículos.

## 🧠 Operaciones aplicadas

- Lectura del CSV con Spark (`spark.read.csv`)
- Transformaciones con `select`, `withColumn`, `groupBy`, `join`, `filter`
- Acciones como `count`, `orderBy`, `toPandas`
- Agregaciones distribuidas: `groupBy`, `reduceByKey` (implícito)
- Visualizaciones con Matplotlib / Seaborn

## 📊 Resultados y gráficos

Se generaron tres visualizaciones clave:

1. **Viajes por hora del día** (`grafico_viajes_por_hora.png`)
2. **Top 10 rutas más congestionadas** (`grafico_rutas_congestionadas.png`)
3. **Entradas y salidas por zona** (`grafico_entrada_salida_zonas.png`)

También se exportaron los siguientes archivos:

- `viajes_por_hora.csv`
- `top_rutas.csv`
- `zonas_entrada_salida.csv`

## 🤖 Uso de IA

Se utilizó IA para:

- Generar la estructura inicial del script PySpark.
- Consultar la sintaxis de operaciones como `join` y `withColumn`.
- Optimizar visualizaciones y exportación de datos.

Las consultas fueron fundamentales para acelerar el desarrollo y validar las mejores prácticas en Spark.

## 🧪 Ejecución local

1. Clona este repositorio:
   ```bash
   git clone 
