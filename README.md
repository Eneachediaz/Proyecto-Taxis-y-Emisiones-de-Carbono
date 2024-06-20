```markdown
# Proyecto de Movilidad Eléctrica para Taxis

## Introducción

Los taxis y servicios como Uber, que han revolucionado la forma en que nos movemos, generan a la vez una avalancha de datos que, bien aprovechados, pueden ser la clave para un futuro más verde. Este proyecto busca expandir la flota hacia la movilidad eléctrica, tomando decisiones informadas basadas en un análisis profundo del movimiento de los taxis, su relación con la contaminación y la viabilidad de la electrificación. Este proyecto combina innovación, análisis y responsabilidad social para transformar el panorama del transporte en la ciudad, reduciendo la huella de carbono, mejorando la imagen pública y optimizando costos.

## Planteo de Objetivos

### Objetivos Principales

1. **Descifrando la viabilidad de los autos eléctricos en Nueva York:**
   - Abordar la pregunta central: ¿Es viable implementar una flota de autos eléctricos para el transporte en la ciudad de Nueva York?
   - Brindar información sólida para la toma de decisiones estratégicas para la implementación de la flota de autos eléctricos.

2. **Empoderando la toma de decisiones informadas:**
   - Realizar un análisis exhaustivo del problema, considerando aspectos ambientales, económicos y logísticos.
   - Generar insights accionables que guíen a la empresa hacia un camino sostenible y rentable.

### Objetivos Técnicos

1. **Construyendo la autopista de datos en la nube:**
   - Desarrollar un pipeline y arquitectura de datos robustos en la nube para procesar y almacenar de manera eficiente la gran cantidad de datos disponibles.
   - Garantizar la seguridad, escalabilidad y confiabilidad de la infraestructura de datos.

2. **Dashboard interactivo:**
   - Crear un dashboard interactivo y fácil de usar que presente información relevante para la toma de decisiones sobre la implementación de la flota eléctrica.
   - Facilitar la comprensión y el análisis de datos complejos para stakeholders de todos los niveles.

3. **Modelo de machine learning predictivo:**
   - Entrenar y desplegar un modelo de machine learning para identificar las ubicaciones óptimas para las estaciones de carga de vehículos eléctricos.
   - Optimizar la ubicación de las estaciones de carga para maximizar la eficiencia, la rentabilidad y la satisfacción del cliente.

## Productos

1. **Un panel de control para la era eléctrica:**
   - Desarrollar un dashboard interactivo que presente información crucial para la fase de implementación de la flota eléctrica.
   - Incluir análisis espaciales, temporales y técnicos/logísticos para una visión completa del panorama.

2. **El mapa del futuro: Un modelo de machine learning para la ubicación de estaciones de carga:**
   - Implementar un modelo de machine learning preciso para identificar las ubicaciones óptimas para las estaciones de carga de vehículos eléctricos.
   - Garantizar una distribución eficiente de las estaciones de carga que responda a la demanda y optimice la experiencia del usuario.

## Equipo

- **Rodrigo Nahuel Castro:** Data Engineer
- **Maximiliano Javier Lizarraga:** Cloud Engineer
- **Lucia Teresa Escobedo Villafane:** Data Analyst
- **Amelia Cristina Herrera Briceño:** Data Analyst
- **Nicolás Hernández Díaz:** Machine Learning Engineer

## Alcance del Proyecto

- **Área de movilidad:** Logística para soluciones de movilidad.
- **Área geográfica:** Ciudad de Nueva York.
- **Fuentes de datos:** NYC Open Data, TLC Trip Record Data, entre otras.
- **Periodo de tiempo:** 2017 - 2023.

## KPIs

1. **Tasa de Cambio en la Demanda de Taxis:**
   - **Objetivo:** Medir el cambio porcentual en la demanda de taxis mes a mes.
   - **Fórmula:** \((DemandaActual − DemandaAnterior) / DemandaAnterior × 100\)
   - **Meta:** Lograr un crecimiento mensual constante en la demanda de taxis de al menos un 5%.

2. **Reducción Porcentual de Emisiones de CO2:**
   - **Objetivo:** Calcular la reducción potencial de CO2 al implementar vehículos eléctricos.
   - **Fórmula:** \((EmisionesCO2vehiculoConvencional − EmisionesCO2vehiculoElectrico) / EmisionesCO2vehiculoConvencional × 100\)
   - **Meta:** Alcanzar una reducción del 30% anual en las emisiones de CO2 por kilómetro.

3. **Porcentaje de Crecimiento en la Base de Usuarios de Servicios de Taxi:**
   - **Objetivo:** Medir el crecimiento en el número de usuarios de servicios de taxi.
   - **Fórmula:** \((NumerodeUsuariosalfinaldelPeriodo − NumerodeUsuariosaliniciodelPeriodo) / NumerodeUsuariosaliniciodelPeriodo\)
   - **Meta:** Lograr un incremento del 10% en la base de usuarios al final del período de análisis.

4. **Accesibilidad espacial de las estaciones de carga:**
   - **Objetivo:** Medir la accesibilidad espacial de las estaciones de carga desde los puntos finales de los viajes de vehículos eléctricos.
   - **Fórmula:**
     \[
     D = \frac{1}{n} \sum_{i=1}^{n} \min_{j \in [1, m]} \text{Distancia}(PuntoFinal_i, EstacionDeCarga_j)
     \]
   - **Meta:** Reducir la distancia promedio a la estación de carga más cercana en un 10%.

## Implementación Detallada

1. **Configuración de Azure Data Factory:**
   - Crear y configurar pipelines en Azure Data Factory para conectar con las fuentes de datos (Azure Synapse, Flat Files).
   - Definir actividades de ingesta y transformación de datos, utilizando Databricks para la transformación de datos.

2. **Transformación de datos en Databricks:**
   - Utilizar Databricks para realizar transformaciones avanzadas en los datos utilizando PySpark.
   - Transformar datos en un formato adecuado y almacenarlos en Azure SQL Database.

3. **Almacenamiento de datos curados en Azure SQL Database:**
   - Configurar Azure SQL Database para recibir y almacenar datos curados.
   - Asegurar que los datos están limpios, transformados y listos para análisis y modelado.

4. **Construcción y despliegue de modelos en Azure Machine Learning:**
   - Usar los datos almacenados en Azure SQL Database para entrenar modelos de machine learning en Azure ML.
   - Desplegar los modelos entrenados y utilizar predicciones para mejorar las operaciones y decisiones empresariales.

5. **Visualización de datos y resultados en Power BI y Streamlit:**
   - Crear dashboards e informes en Power BI para visualizar datos y resultados de modelos de machine learning.
   - Desarrollar aplicaciones web interactivas en Streamlit para permitir una interacción más profunda con los datos y los modelos de ML.

## Stack Tecnológico

- **Azure Data Factory:** Orquestación y manejo de pipelines de datos.
- **Azure Synapse Analytics:** Almacenamiento y análisis de datos a gran escala.
- **Azure SQL Database:** Almacenamiento de datos estructurados.
- **Databricks:** Transformación avanzada de datos utilizando PySpark.
- **Azure Machine Learning:** Entrenamiento y despliegue de modelos de machine learning.
- **Scikit-Learn:** Implementación de modelos de machine learning, incluyendo K-Means y DBSCAN.
- **Power BI:** Visualización y creación de dashboards interactivos.
- **Streamlit:** Desarrollo de aplicaciones web interactivas para la visualización y análisis de datos.
- **NYC Open Data & TLC Trip Record Data:** Fuentes de datos para análisis y modelado.
```
