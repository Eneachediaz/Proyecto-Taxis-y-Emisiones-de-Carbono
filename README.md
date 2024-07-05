![Cabeza](Recursos%20de%20Marca/Encabezado%20sin%20fondo.png)

Claro, aquí tienes una versión más detallada del plan del proyecto.

## Proyecto Movilidad Eléctrica para Taxis en Nueva York, EEUU

### Introducción:
Los taxis y servicios como Uber han transformado significativamente el transporte urbano. Estos servicios generan una enorme cantidad de datos que, si se analizan adecuadamente, pueden facilitar la transición hacia una movilidad más sostenible. Este proyecto busca explorar la viabilidad de expandir la flota de taxis hacia vehículos eléctricos (EVs) en Nueva York, utilizando análisis de datos avanzados para tomar decisiones informadas que reduzcan la huella de carbono, mejoren la eficiencia operativa y optimicen los costos.

### Planteo de Objetivos:

#### Objetivos Principales:
1. **Viabilidad de los autos eléctricos en Nueva York**:
    - **Pregunta central**: ¿Es viable implementar una flota de autos eléctricos para el transporte de pasajeros en Nueva York?
    - **Toma de decisiones estratégicas**: Proveer información sólida y accionable para apoyar la implementación de la flota de autos eléctricos.

2. **Empoderar la toma de decisiones informadas**:
    - **Análisis exhaustivo**: Considerar aspectos ambientales, económicos y logísticos.
    - **Generación de insights**: Proporcionar información accionable para guiar a la empresa hacia un futuro sostenible y rentable.

#### Objetivos Técnicos:
1. **Construir una infraestructura de datos en la nube**:
    - **Pipeline de datos robusto**: Procesar y almacenar eficientemente la gran cantidad de datos disponibles.

2. **Dashboard interactivo**:
    - **Facilidad de uso**: Presentar información relevante de manera comprensible para stakeholders de todos los niveles.
    - **Visualización de datos complejos**: Facilitar el análisis y la comprensión de los datos.

3. **Modelo de machine learning no supervisado**:
    - **Ubicaciones óptimas para estaciones de carga**: Entrenar y desplegar un modelo para identificar las mejores ubicaciones para las estaciones de carga de vehículos eléctricos.
    - **Optimización de ubicaciones**: Maximizar la eficiencia, la rentabilidad y la satisfacción del cliente.

### Productos:
1. **Panel de control para la era eléctrica**:
    - **Dashboard interactivo**: Presentar información crucial para la implementación de la flota eléctrica.
    - **Análisis espaciales, temporales y técnicos/logísticos**: Ofrecer una visión completa del panorama de movilidad eléctrica.

2. **Modelo de machine learning para la ubicación de estaciones de carga**:
    - **Identificación precisa de ubicaciones**: Implementar un modelo que identifique las mejores ubicaciones para las estaciones de carga.

### Equipo:
- **Rodrigo Nahuel Castro**: Data Engineer
- **Maximiliano Javier Lizarraga**: Cloud Engineer
- **Lucía Teresa Escobedo Villafane**: Data Analyst
- **Amelia Cristina Herrera Briceño**: Data Analyst
- **Nicolás Hernández Díaz**: Machine Learning Engineer

### Alcance del Proyecto:
- **Área de movilidad**: Soluciones de movilidad de pasajeros.
- **Área geográfica**: Ciudad de Nueva York, EEUU.
- **Fuentes de datos**: NYC Open Data, TLC Trip Record Data, EPA NY, entre otras.
- **Período de tiempo**: 2019 - 2023.

### KPIs:
1. **Tasa de Cambio en la Demanda de Taxis**:
    - **Objetivo**: Medir el cambio porcentual en la demanda de taxis mes a mes.
    - **Fórmula**: ((DemandaActual − DemandaAnterior) / DemandaAnterior) × 100
    - **Meta**: Crecimiento mensual constante en la demanda de taxis de al menos un 5%.

2. **Reducción Porcentual de Emisiones de CO2**:
    - **Objetivo**: Calcular la reducción potencial de CO2 al implementar vehículos eléctricos.
    - **Fórmula**: ((EmisionesCO2vehiculoConvencional − EmisionesCO2vehiculoElectrico) / EmisionesCO2vehiculoConvencional) × 100
    - **Meta**: Reducción del 10% anual en las emisiones de CO2 por milla.

3. **Porcentaje de Crecimiento en la Base de Usuarios de Servicios de Taxi**:
    - **Objetivo**: Medir el crecimiento en el número de usuarios de servicios de taxi.
    - **Fórmula**: ((NumeroDeUsuariosAlFinalDelPeriodo − NumeroDeUsuariosAlInicioDelPeriodo) / NumeroDeUsuariosAlInicioDelPeriodo) × 100
    - **Meta**: Incremento del 5% en la base de usuarios al final del período de análisis.

4. **Accesibilidad espacial de las estaciones de carga**:
    - **Objetivo**: Medir la accesibilidad espacial de las estaciones de carga desde los puntos finales de los viajes de vehículos eléctricos.
    - **Fórmula**: \[ D = \frac{1}{n} \sum_{i=1}^{n} \min_{j \in [1, m]} \text{Distancia}(PuntoFinal_i, EstacionDeCarga_j) \]
    - **Meta**: Reducir la distancia promedio a la estación de carga más cercana en un 10%.

### Implementación Detallada:

#### Configuración de Databricks:
- **Ingesta y transformación de datos**: Utilizar Databricks para realizar ETL (Extracción, Transformación y Carga) avanzado de los datos.
- **Almacenamiento**: Transformar los datos y almacenarlos en Azure SQL Database siguiendo la arquitectura Medallion (Bronce, Plata y Oro).

#### Almacenamiento de datos curados en Azure SQL Database:
- **Recepción y almacenamiento de datos curados**: Asegurar que los datos están limpios y listos para análisis y modelado.

#### Construcción y despliegue de modelos en Azure Machine Learning:
- **Entrenamiento de modelos**: Usar los datos almacenados para entrenar modelos de machine learning.
- **Despliegue**: Procesar la información y encontrar patrones para mejorar las decisiones empresariales.

#### Visualización de datos y resultados en Power BI:
- **Dashboards e informes**: Crear dashboards en Power BI para visualizar los datos y resultados de los modelos.

### Stack Tecnológico:
- **Databricks**: Transformación avanzada de datos utilizando PySpark.
- **Azure SQL Database**: Almacenamiento de datos estructurados.
- **Power BI**: Visualización y creación de dashboards interactivos.

### Carta Gantt: Movilidad en la Gran Manzana: Taxis, autos compartidos y la carrera hacia la sostenibilidad

#### Sprint 1 (1 semana):
- **Semana 1**:
  - Definición del alcance y objetivos del proyecto.
  - Configuración del repositorio en GitHub.
  - Elaboración de un cronograma general y Carta Gantt.
  - Implementación del stack tecnológico.
  - Metodología de trabajo y repartición de tareas.
  - Análisis preliminar de los datos (EDA) para definir KPIs y el modelo de machine learning.

#### Herramientas:
- **Lenguajes de programación**: Python.
- **Bibliotecas de análisis de datos**: Pandas, NumPy, scikit-learn.
- **Herramientas de visualización de datos**: Matplotlib, Seaborn, Plotly.
- **Entornos de desarrollo integrados**: Jupyter Notebook, Visual Studio Code.
- **Plataformas de cloud computing**: Microsoft Azure.
- **Software de gestión de proyectos**: Ganttpro.
- **Herramientas de comunicación**: App.gather.town, Zoom.
- **Presentaciones finales**: Power BI.

#### Sprint 2 (1 semana):
- **Semana 2**:
  - Revisión de ETL de los datos completos.
  - Automatización del pipeline de ETL.
  - Implementación de la estructura de los datos.
  - Diseño del modelo de entidad-relación (ER).
  - Configuración de pipelines para alimentar al Data Warehouse (DW).
  - Validación de los datos.
  - Documentación de cada punto anterior.
  - Análisis de datos de muestra.
  - Prueba del concepto del producto MVP.

#### Herramientas:
- **Lenguajes de programación**: Python.
- **Bibliotecas de análisis de datos**: Pandas, NumPy, scikit-learn.
- **Herramientas de visualización de datos**: Matplotlib, Seaborn, Plotly.
- **Entornos de desarrollo integrados**: Jupyter Notebook, Visual Studio Code.
- **Plataformas de cloud computing**: Microsoft Azure.
- **Software de gestión de proyectos**: Ganttpro.
- **Herramientas de comunicación**: App.gather.town, Zoom.
- **Herramientas de ETL**: Pandas, NumPy, etc.
- **Herramientas de modelado de datos**: K-means, clustering.
- **Herramientas de documentación**: Readme.md, Markdown, pdf.
- **Herramientas de dashboarding**: Power BI.
- **Herramientas de Machine Learning**: scikit-learn.

#### Sprint 3 (1 semana):
- **Semana 3**:
  - Diseño del dashboard.
  - Implementación de KPIs.
  - MLOps.
  - Modelo de machine learning.
  - Modelo de ML en producción.
  - Presentación general (informe del análisis).

![Pie](Recursos%20de%20Marca/Pie%20de%20Pagina.png)
