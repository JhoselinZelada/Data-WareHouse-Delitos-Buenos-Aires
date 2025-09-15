# Data-WareHouse-Delitos-Buenos-Aires
Proyecto de Data Warehouse sobre delitos en Buenos Aires. 



Modelo multidimensional : 
Link: https://drive.google.com/drive/folders/19-tNfXBYhfnVHK1NRHPVyJeM5UfjabLg 
Para la creación del modelo multidimensional se deteminaron las dimensiones: 
-DimCaracteristica 
-DimTiempo
-DimTipo
-DimUbicacion

Tabla de hechos: 
-factDelitos con sus respectivas medidas (Cantidad de columna por comuna, cantidad de delitos por año, cantidad de delitos por mes, cantidad de delitos por día, cantidad de delitos por barrio, 
cantidad de delitos según tipo de delitos, porcentaje de delitos según tipo de delitos, tasa de variación mensual, tasa de variación anual, frecuencia de delitos por franja horaria.
Ádemas, la factDelitos contiene una dimensión degenerada, llamada franja_horaria.
