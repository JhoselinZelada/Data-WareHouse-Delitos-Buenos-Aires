# Data-WareHouse-Delitos-Buenos-Aires

Proyecto de creación de un **Data Warehouse** sobre delitos en la ciudad de Buenos Aires, consolidando información de diferentes fuentes para facilitar el análisis y la visualización de los datos, convirtiéndolos en **insights** de valor para la toma de decisiones.


## Objetivo
El objetivo de este proyecto es poder consolidar y organizar los datos de delitos en Buenos Aires para **analizarlos de manera efectiva**, detectar patrones y tendencias, generar **información útil y visualizaciones claras**, y así apoyar la **toma de decisiones basada en datos**..

## Herramientas
Para el desarrollo de este proyecto se utilizaron las siguientes herramientas:

- **SQL / PL-SQL** → Para el proceso ETL y creación del Modelo Multidimensional.
- **Power BI** → para la visualización y creación de dashboards interactivos.  
- **Archivos CSV** → como fuente de datos inicial para cargar la información en el Data Warehouse.  
- **GitHub** → Para la gestion de almacenamiento del proyecto.
- **Draw.io** →  Para el diseño del Modelo multidimensional.


## Datos
Los datos recolectados para este proyecto corresponden a los delitos ocurridos en Buenos Aires, Argentina, desde el año 2016 hasta el 2022 (inclusive), dando un total de **939.684 registros iniciales**.  

Luego del proceso ETL, en el que se eliminó una columna (CANTIDAD) que no aportaba valor al análisis, se estandarizaron y normalizaron los datos, se eliminaron duplicados, valores nulos y caracteres erróneos.  

La base de datos final está compuesta por **912.764 registros**.

## Modelo multidimensional

En base al siguiente modelo multidimensional, se crearon las respectivas **dimensiones** y la **tabla de hechos** para cargar los datos ya transformados.

![Modelo multidimensional](MODELO_MULTIDIMENSIONAL/MODELO_ESTRELLA_V2.png)



Para la creación del modelo multidimensional se deteminaron las dimensiones: 
  -DimCaracteristica 
  -DimTiempo
  -DimTipo
  -DimUbicacion

Tabla de hechos:
  -FactDelitos


Finalmente, realice la conexión con Power bi para generar los siguientes Dashboards:


![Modelo multidimensional](POWER_BI_V2/dashboards/DASHBOARD_1.png)









-factDelitos con sus respectivas med
Ádemas, la factDelitos contiene una dimensión degenerada, llamada franja_horaria.
