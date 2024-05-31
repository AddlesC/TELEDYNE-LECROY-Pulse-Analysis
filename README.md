# Análisis de Pulsos Experimentales para osciloscpio Teledyne Lecroy

Este repositorio contiene código para el análisis y visualización de datos de pulsos experimentales. Los datos se leen de archivos de texto (.txt), donde cada archivo contiene datos de un solo pulso. Estos datos deben unirse para formar gráficos completos y realizar un análisis detallado. A continuación, se detallan las diferentes funcionalidades implementadas:

## Procesamiento de Datos Experimentales para Análisis

Código diseñado para leer y organizar datos experimentales de archivos de texto en DataFrames de Pandas. Incluye:
- **Funciones para extracción de datos**: `parse_header()` para metadatos y `extract_data()` para convertir datos en DataFrame.
- **Estructuras de datos para organización**: Uso de diccionarios para agrupar datos por canales y pulsos, facilitando el acceso y manejo.
- **Procesamiento y acceso automatizado**: Iteración sobre archivos de un directorio, extracción y almacenamiento estructurado, con ejemplo de acceso a los datos.

## Visualización de Pulsos Filtrados por Canal

Este código genera subplots para visualizar los pulsos válidos de cada canal, permitiendo una comparación directa entre canales en un conjunto de datos filtrado.

## Corrección de Baseline y Comparación de Pulsos por Canal

Este código implementa un procedimiento para corregir el baseline de pulsos experimentales y visualizar comparativamente los datos originales y corregidos en subplots por canal.

## Visualización de Pulsos Corregidos por Offset

Este código grafica los pulsos después de haber sido corregidos para eliminar desviaciones de baseline, usando subplots para cada canal.

## Visualización de un Pulso Corregido Específico

Este fragmento de código está diseñado para graficar un pulso específico después de haber sido corregido para desviaciones de baseline.

## Cálculo de Métricas de Pulsos

Este código proporciona una funcionalidad para calcular métricas específicas de pulsos eléctricos, como el tiempo de subida y el ancho del pulso, bajo condiciones definidas.

## Visualización de Pulsos con Métricas de Tiempo de Subida y Ancho

Este código facilita la visualización de un pulso específico, marcando visualmente métricas clave como el tiempo de subida y el ancho del pulso.

## Cálculo de Métricas Promedio de Pulsos por Canal

Este código calcula el promedio del tiempo de subida y el ancho del pulso para cada canal basado en los datos previamente analizados.

## Filtrado de Datos por Ventanas de Tiempo y Visualización por Canal

Este código filtra y visualiza datos de pulsos para cada canal dentro de ventanas de tiempo específicas, facilitando la comparación y el análisis de características particulares de los pulsos.

## Histograma de Áreas Bajo la Curva por Canal

Este código calcula y visualiza el histograma de las áreas bajo la curva para los pulsos de cada canal dentro de ventanas de tiempo especificadas.

## Histograma de Amplitudes Máximas por Canal

Este código calcula y visualiza un histograma de las amplitudes máximas (mínimos en valor absoluto debido a amplitudes negativas) para pulsos dentro de ventanas de tiempo especificadas por canal.

## Análisis de Amplitud Promedio de Pulsos por Canal

Este código agrupa y visualiza la amplitud promedio de pulsos corregidos por canal, proporcionando una representación gráfica clara de la actividad promedio en cada canal.

## Requisitos

- Python 3.x
- Pandas
- NumPy
- Matplotlib

## Uso

Para ejecutar los scripts, asegúrese de tener todos los paquetes requeridos instalados y ejecute cada sección de código en un entorno de Jupyter Notebook o como scripts de Python independientes según sus necesidades experimentales.

---

Este repositorio proporciona herramientas robustas para el análisis y visualización de datos de pulsos experimentales, facilitando una evaluación detallada de las características de los pulsos en estudios de múltiples canales.
