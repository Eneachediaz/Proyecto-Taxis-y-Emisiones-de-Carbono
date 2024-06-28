![Encabezado](./Recursos%20de%20Marca/Encabezado%20sin%20fondo.png)

# Descripción del Modelo Relacional

## Tablas y Campos

### Light Duty Vehicles
- **Campos:**
  'Vehicle ID', 'Fuel ID', 'Fuel Configuration ID', 'Manufacturer ID', 'Category ID', 'Model', 'Model Year', 'Alternative Fuel Economy City', 'Alternative Fuel Economy Highway', 'Alternative Fuel Economy Combined', 'Conventional Fuel Economy City', 'Conventional Fuel Economy Highway', 'Conventional Fuel Economy Combined', 'Transmission Type', 'Engine Type', 'Engine Size', 'Engine Cylinder Count', 'Engine Description', 'Manufacturer', 'Manufacturer URL', 'Category', 'Fuel Code', 'Fuel', 'Fuel Configuration Name', 'Electric-Only Range', 'PHEV Total Range', 'PHEV Type', 'Notes', 'Drivetrain'


### Electric and Alternative Fuel Stations
- **Campos:**
  'Fuel Type Code', 'Station Name', 'Street Address', 'Intersection Directions', 'City', 'State', 'ZIP', 'Plus4', 'Station Phone', 'Status Code', 'Expected Date', 'Groups With Access Code', 'Access Days Time', 'Cards Accepted', 'BD Blends', 'NG Fill Type Code', 'NG PSI', 'EV Level1 EVSE Num', 'EV Level2 EVSE Num', 'EV DC Fast Count', 'EV Other Info', 'EV Network', 'EV Network Web', 'Geocode Status', 'Latitude', 'Longitude', 'Date Last Confirmed', 'ID', 'Updated At', 'Owner Type Code', 'Federal Agency ID', 'Federal Agency Name', 'Open Date', 'Hydrogen Status Link', 'NG Vehicle Class', 'LPG Primary', 'E85 Blender Pump', 'EV Connector Types', 'Country', 'Intersection Directions (French)', 'Access Days Time (French)', 'BD Blends (French)', 'Groups With Access Code (French)', 'Hydrogen Is Retail', 'Access Code', 'Access Detail Code', 'Federal Agency Code', 'Facility Type', 'CNG Dispenser Num', 'CNG On-Site Renewable Source', 'CNG Total Compression Capacity', 'CNG Storage Capacity', 'LNG On-Site Renewable Source', 'E85 Other Ethanol Blends', 'EV Pricing', 'EV Pricing (French)', 'LPG Nozzle Types', 'Hydrogen Pressures', 'Hydrogen Standards', 'CNG Fill Type Code', 'CNG PSI', 'CNG Vehicle Class', 'LNG Vehicle Class', 'EV On-Site Renewable Source', 'Restricted Access'


### taxi+_zone_lookup
- **Campos:**
  - Borough
  - **LocationID** (PK)
  - service_zone
  - Zone

### NYC Taxi Zones
- **Campos:**
  **'location_id'** (PK),'zone','borough','geometry'

### EmisionesCO2_EPA
- **Campos:**
  - Distancia anual
  - Economia combustible
  - Emisiones_xgallon

### TaxisCO2Emissions
- **Campos:**
  - CO2 Emissions Convencional
  - CO2 Emissions Electric
  - dispatching
  - dropOff datetime
  - **pickup_datetime** (FK)
  - Electric Efficiency

### EmisionesDiariasAgregadas
- **Campos:**
  - CO2 Emissions Daily
  - **pickup datetime** (FK)

### Date
- **Campos:**
  **'Date'** (PK), 'Year', 'Month', 'Month Number', 'Weekday', 'Day', 'Quarter'

### yellow_tripdata_2024-01
- **Campos:**
  'VendorID', 'tpep_pickup_datetime', 'tpep_dropoff_datetime',
  'passenger_count', 'trip_distance', 'RatecodeID', 'store_and_fwd_flag',
   **'PULocationID'** (FK),**'DOLocationID'** (FK), 'payment_type', 'fare_amount', 'extra',
  'mta_tax', 'tip_amount', 'tolls_amount', 'improvement_surcharge',
  'total_amount', 'congestion_surcharge', 'Airport_fee'

### green_tripdata_2024-01
- **Campos:**
  'VendorID', 'lpep_pickup_datetime', 'lpep_dropoff_datetime',
  'store_and_fwd_flag', 'RatecodeID', **'PULocationID'** (FK),**'DOLocationID'** (FK),
  'passenger_count', 'trip_distance', 'fare_amount', 'extra', 'mta_tax',
  'tip_amount', 'tolls_amount', 'ehail_fee', 'improvement_surcharge',
  'total_amount', 'payment_type', 'trip_type', 'congestion_surcharge'

### fhvhv_tripdata_2024-01
- **Campos:**
  'hvfhs_license_num', 'dispatching_base_num', 'originating_base_num',
  'request_datetime', 'on_scene_datetime', 'pickup_datetime',
  'dropoff_datetime', **'PULocationID'** (FK),**'DOLocationID'** (FK), 'trip_miles',
  'trip_time', 'base_passenger_fare', 'tolls', 'bcf', 'sales_tax',
  'congestion_surcharge', 'airport_fee', 'tips', 'driver_pay',
  'shared_request_flag', 'shared_match_flag', 'access_a_ride_flag',
  'wav_request_flag', 'wav_match_flag'

### ElectricCarData_Clean
'Brand', **'Model'** (PK), 'AccelSec', 'TopSpeed_KmH', 'Range_Km', 'Efficiency_WhKm', 'FastCharge_KmH', 'RapidCharge', 'PowerTrain', 'PlugType', 'BodyStyle', 'Segment', 'Seats', 'PriceEuro'


### Alternative Fuel Vehicle
 'Category', **'Model'** (PK), 'Model Year', **'Manufacturer'** (FK), 'Fuel', 'All-Electric Range', 'PHEV Total Range', 'Alternative Fuel Economy City', 'Alternative Fuel Economy Highway', 'Alternative Fuel Economy Combined', 'Conventional Fuel Economy City', 'Conventional Fuel Economy Highway', 'Conventional Fuel Economy Combined', 'Transmission Type', 'Transmission Make', 'Engine Type', 'Engine Size', 'Engine Cylinder Count', 'Number of Passengers', 'Heavy-Duty Power System', 'Notes', 'Drivetrain'


### Vehicle Fuel Economy Data
'Year', **'Manufacturer'** (FK), **'Model'** (PK), 'barrels08', 'barrelsA08', 'charge240', 'city08', 'city08U', 'cityA08', 'cityA08U', 'cityCD', 'cityE', 'cityUF', 'co2', 'co2A', 'co2TailpipeAGpm', 'co2TailpipeGpm', 'comb08', 'comb08U', 'combA08', 'combA08U', 'combE', 'combinedCD', 'combinedUF', 'cylinders', 'displ', 'drive', 'engId', 'eng_dscr', 'feScore', 'fuelCost08', 'fuelCostA08', 'fuelType', 'fuelType1', 'ghgScore', 'ghgScoreA', 'highway08', 'highway08U', 'highwayA08', 'highwayA08U', 'VClass', 'highwayCD', 'highwayE', 'highwayUF', 'hlv', 'hpv', 'id', 'lv2', 'lv4', 'mpgData', 'phevBlended', 'pv2', 'pv4', 'range', 'rangeCity', 'rangeCityA', 'rangeHwy', 'rangeHwyA', 'trany', 'UCity', 'UCityA', 'UHighway', 'UHighwayA', 'youSaveSpend', 'guzzler', 'trans_dscr', 'tCharger', 'sCharger', 'atvType', 'fuelType2', 'rangeA', 'evMotor', 'mfrCode', 'c240Dscr', 'charge240b', 'c240bDscr', 'createdOn', 'modifiedOn', 'startStop', 'phevCity', 'phevHwy', 'phevComb'


## Relaciones entre Tablas

## Relaciones
### Relaciones con `taxit_zone_lookup`
- **fhv_tripdata_2024-01**.DOLocationID → **taxit_zone_lookup**.LocationID
- **fhv_tripdata_2024-01**.PULocationID → **taxit_zone_lookup**.LocationID
- **fhvhv_tripdata_2024-01**.DOLocationID → **taxit_zone_lookup**.LocationID
- **fhvhv_tripdata_2024-01**.PULocationID → **taxit_zone_lookup**.LocationID
- **green_tripdata_2024-01**.DOLocationID → **taxit_zone_lookup**.LocationID
- **green_tripdata_2024-01**.PULocationID → **taxit_zone_lookup**.LocationID
- **yellow_tripdata_2024-01**.DOLocationID → **taxit_zone_lookup**.LocationID
- **yellow_tripdata_2024-01**.PULocationID → **taxit_zone_lookup**.LocationID

### Relaciones con `Date`
- **fhv_tripdata_2024-01**.pickup_date → **Date**.Date
- **fhvhv_tripdata_2024-01**.pickup_date → **Date**.Date
- **green_tripdata_2024-01**.pickup_date → **Date**.Date
- **yellow_tripdata_2024-01**.pickup_date → **Date**.Date

### Relaciones con `EmisionesDiarias`
- **Date**.Date → **EmisionesDiariasAgrupadas**.pickup_datetime
- **Date**.Date → **EmisionesDiariasElectricas**.pickup_datetime

### Relaciones con `NYC_Taxi_Zones`
- **taxit_zone_lookup**.LocationID → **NYC_Taxi_Zones**.location_id

### Relaciones con Alternative Fuel Vehicle
- **ElectricCarData_Clean**.Model → **Alternative Fuel Vehicle**.Model


![Footer](./Recursos%20de%20Marca/Pie%20de%20Pagina.png)
