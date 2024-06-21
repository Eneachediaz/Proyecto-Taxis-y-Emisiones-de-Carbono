![Logo](ruta_del_logo.png)

# Análisis de la Calidad de los Datos

---

## 1. Revisión de Datos Faltantes

### Datasets NYK Taxis:
- **Presencia de Valores Nulos**: Encontramos valores nulos en columnas como `PUlocationID`, `DOlocationID`, `airport_fee`. Además, valores en `0` para `passenger_count` y `trip_distance`.
- **Impacto en el Análisis**: Consideramos que los valores faltantes podrían afectar los análisis posteriores y decidimos eliminar los valores nulos de `PUlocationID`, `DOlocationID`. En el resto de las columnas, se suprimieron al agrupar.

### Alternative Fuel Vehicles:
- **Presencia de Valores Nulos**: Alta tasa de valores nulos en columnas como `All-Electric Range` (660), `PHEV Total Range` (839) y `Number of Passengers` (761) con más del 70% de datos faltantes. Tasa moderada en `Alternative Fuel Economy Combined` (620) y `Conventional Fuel Economy Combined` (438) con alrededor del 50-70% de datos faltantes. Baja tasa en `Model Year`, con 288 valores faltantes (aproximadamente el 33%).
- **Impacto en el Análisis**: Los valores faltantes podrían afectar los análisis posteriores, por lo que serán tomados en consideración en transformaciones futuras.

### Electric and Alternative Charging Stations:
- **Presencia de Valores Nulos**: La columna `Intersection Directions` tiene un nivel alto de valores nulos.
- **Impacto en el Análisis**: Consideramos eliminarla en transformaciones futuras debido a su alto nivel de valores nulos.

### Light Duty Vehicles:
- **Presencia de Valores Nulos**: Alta tasa de valores nulos en `Economía Combinada de Combustible Alternativo` (85%), `Economía Combinada de Combustible Convencional` (75%), `Rango Eléctrico Puro` (88%) y `Rango Total PHEV` (96%).
- **Impacto en el Análisis**: Los valores faltantes podrían afectar los análisis posteriores, por lo que consideramos eliminar estos valores nulos y centrarnos en los datos completos para análisis específicos.

### Calidad del Aire:
- **Presencia de Valores Nulos**: Pocos valores nulos en las columnas `geo_join_id` y `geo_place_name`.
- **Impacto en el Análisis**: Consideramos eliminar las filas afectadas en transformaciones futuras.

### Vehicle Fuel Economy:
- **Presencia de Valores Nulos**: Valores nulos en varias columnas, con la mayoría de los datos completos en `Year` y `Manufacturer`, mientras que otras columnas como `fuelType2` tienen más del 90% de valores nulos. Columnas relacionadas con la autonomía (`range`, `rangeCity`, `rangeHwy` y `youSaveSpend`) también tienen una cantidad considerable de datos faltantes (alrededor del 5%).
- **Impacto en el Análisis**: Los valores faltantes podrían afectar los análisis posteriores, por lo que es importante tener en cuenta la presencia de estos valores nulos y decidir cómo manejarlos antes de realizar cualquier análisis.

---

## 2. Consistencia de Datos

### Datasets NYK Taxis:
- **Presencia de Valores Erróneos**: Encontramos fechas con referencia a años futuros como 2050 en columnas como `pickup_datetime` y `dropOff_datetime`.
- **Impacto en el Análisis**: Estas fechas erróneas podrían afectar los análisis posteriores y serán tratadas en la etapa de transformaciones.

### Annotations:
- **Presencia de Valores Duplicados**: Encontramos una cantidad alta de valores duplicados (46047 filas).
- **Impacto en el Análisis**: Los valores duplicados podrían afectar los análisis posteriores y serán eliminados en la etapa de transformaciones.

### Alternative Fuel Vehicles:
- **Presencia de Valores Duplicados**: Encontramos columnas duplicadas.
- **Impacto en el Análisis**: Serán eliminadas en la etapa de transformaciones.

### Vehicle Fuel Economy:
- **Presencia de Valores Duplicados**: Alta cantidad (11783 filas) de valores duplicados en este dataset.
- **Impacto en el Análisis**: Las filas duplicadas podrían afectar los análisis posteriores, por lo que serán tratadas en la etapa de transformaciones.

---

## 3. Revisión de Rango de Valores

### Datasets NYK Taxis:
- **Presencia de Outliers**: Encontramos outliers en columnas como `trip_duration_hours` en el mes de julio 2021.
- **Impacto en el Análisis**: Suprimimos los datos correspondientes a julio 2021, los demás serán tratados en transformaciones posteriores.

### Alternative Fuel Vehicles:
- **Presencia de Outliers**: Encontramos outliers en la columna `Conventional Fuel Economy Combined`.
- **Impacto en el Análisis**: Serán tratados en transformaciones posteriores.

### Electric Car Data:
- **Presencia de Outliers**: Encontramos outliers en las columnas como `PriceEuro`, `Efficiency_WhKm`, `FastCharge_KmH`, `Range_Km`, `TopSpeed_KmH`.
- **Impacto en el Análisis**: Los outliers encontrados son pocos, serán considerados en el proceso de transformaciones.

### Light Duty Vehicles:
- **Presencia de Outliers**: Encontramos outliers en la columna `Conventional Fuel Economy Combined`.
- **Impacto en el Análisis**: Serán tratados en transformaciones posteriores.

### Vehicle Fuel Economy:
- **Presencia de Outliers**: Encontramos outliers en las columnas como `co2`, `co2A`, `comb08`, `combA08`, `fuelCost08`, `fuelCostA08`, `range`, `rangeCity`, `rangeHwy`.
- **Impacto en el Análisis**: Se encontraron gran cantidad de outliers, serán considerados en el proceso de transformaciones.

---

---

![Footer](ruta_del_pie_de_pagina.png)