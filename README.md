# Retail Analysis

# 1 Proyecto: Análisis de una empresa de telecomunicaciones

## 📂 Contenido del repositorio
Jupyter Notebook
Python: pandas, numpy, seaborn, matplotlib

plans.csv: Catálogo de planes con sus precios y beneficios. Descárgalo aquí.
users_latam.csv: Información de cada usuario (datos personales, plan, fecha de registro, churn). Descárgalo aquí.
usage.csv: Actividad generada por los usuarios: llamadas, mensajes, duración, longitud.

## 🧠 Objetivo del análisis

El objetivo de este proyecto fue analizar el comportamiento de los clientes de ConnectaTel a partir de información demográfica y registros de uso del servicio.

El análisis buscó:

identificar problemas de calidad en los datos,
limpiar y preparar la información,
estudiar patrones de uso de llamadas y mensajes,
segmentar clientes según edad y nivel de uso,
detectar outliers y comportamientos extremos,
y generar recomendaciones de negocio para mejorar los planes de la compañía.

# 2 Proyecto RappiPlus: De datos a decisiones de negocio
## 📂 Contenido del repositorio

## 📌 Descripción

Este proyecto analiza el desempeño del servicio RappiPlus con el objetivo de transformar datos en insights accionables para la toma de decisiones de negocio.

El análisis integra diferentes fuentes de información para evaluar:
Calidad y confiabilidad de los datos.
Revenue, costos y rentabilidad.
Comportamiento de ventas.
Funnel de conversión de usuarios.
Retención por cohortes.
Impacto de cambios mediante pruebas estadísticas.
Visualización de KPIs mediante un dashboard de Business Intelligence.
El proyecto fue desarrollado como un ejercicio integral de Data Analytics, combinando Python, SQL, análisis estadístico y Business Intelligence.

## 🎯 Objetivos del proyecto

Validar y preparar los datos antes del análisis.
Medir los principales indicadores financieros y comerciales.
Identificar puntos de pérdida dentro del funnel de conversión.
Analizar la retención de usuarios mediante cohortes.
Evaluar experimentalmente el impacto de cambios en la interfaz de checkout.
Comunicar los resultados mediante dashboards orientados a negocio.

## 🗂️ Fuentes de datos

El proyecto contempla las siguientes fuentes: Dataset / Fuente, rappiplus_orders_raw.csv, rappiplus_catalog.csv, rappiplus_marketing_spend.csv, experiment_checkout_ui.csv

## 🔎 Metodología

1. Calidad de datos:

Se realiza una revisión inicial de los datasets para:

Validar formatos de fecha.
Revisar variables numéricas.
Detectar valores inválidos.
Verificar consistencia de montos.
Identificar y eliminar duplicados.
Revisar variables categóricas.
Exportar los datasets limpios para su posterior uso en BI.

Archivos de salida:

orders_clean.csv,
catalog_clean.csv,
marketing_clean.csv,

2. Análisis de rentabilidad

Se calculan indicadores clave del negocio, entre ellos:

-Revenue total.
-Costo total.
-Inversión total en marketing.
-Profit.
-Ticket promedio por orden.
-Cantidad promedio de productos por orden.
-Producto más vendido.
-Gasto de marketing por canal.

El objetivo es determinar la situación financiera y comercial del servicio y encontrar oportunidades de mejora.

3. Funnel de conversión

Mediante SQL se analiza la tabla events para construir el funnel de usuarios.
El análisis permite:

- Contabilizar usuarios únicos por etapa.
- Ordenar los eventos según el flujo de conversión.
- Calcular la conversión entre etapas.
- Identificar el principal punto de abandono.
- Obtener la tasa de conversión final.

4. Retención por cohortes

Se utilizan las tablas users y user_activity para analizar el comportamiento posterior al registro.
Las cohortes se construyen utilizando el mes de registro y se calcula la retención semanal.

El análisis permite identificar qué tan efectivamente la plataforma consigue mantener activos a los nuevos usuarios.


5. Business Intelligence

Los datasets limpios se preparan para construir dashboards en Power BI.
El dashboard propuesto contempla:

Dashboard 1 — Overview Ejecutivo

KPIs:

- Revenue total.
- Profit total.
- Gasto total en marketing.
- Ticket promedio.
- Cantidad promedio de productos por orden.

## 🛠️ Tecnologías utilizadas:

 Tecnología--------------Uso

- Python-----------------Limpieza, transformación y análisis de datos

- Pandas-----------------Manipulación de DataFrames

- SQL--------------------Consultas y análisis de datos relacionales

- SQLAlchemy-------------Conexión con PostgreSQL

- SciPy / estadística----Evaluación del experimento A/B

- Power BI----------------Visualización y dashboard

- Jupyter Notebook--------Desarrollo y documentación del análisis
