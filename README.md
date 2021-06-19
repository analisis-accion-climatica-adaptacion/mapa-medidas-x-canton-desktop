# Mapa de medidas de acción climática por cantón - versión escritorio
Este repositorio contiene los archivos necesarios para la construcción de un mapa que muestra la cantidad de medidas de acción climática en cada cantón de Costa Rica. Se desarrolló en el sistema de información geográfica de escritorio [QGIS](https://www.qgis.org/).

El mapa puede visualizarse en:  
[https://github.com/analisis-accion-climatica-adaptacion/mapa-medidas-x-canton-desktop/blob/main/salidas/mapa-medidas-x-canton.pdf](https://github.com/analisis-accion-climatica-adaptacion/mapa-medidas-x-canton-desktop/blob/main/salidas/mapa-medidas-x-canton.pdf)

## Entradas
**1. Archivo GeoJSON con capa geoespacial de cantones de Costa Rica en el SRS CRTM05**  

Nombre del archivo: ```datos/cantones-medidas-crtm05.geojson```  

Se obtuvo al copiar el archivo ```datos/cantones-medidas.geojson``` del [repositorio de la versión web de este mapa](https://github.com/analisis-accion-climatica-adaptacion/mapa-medidas-x-canton-web) y aplicar los comandos:

```
cd datos
ogr2ogr -t_srs EPSG:5367 cantones-medidas-crtm05.geojson cantones-medidas.geojson
rm cantones-medidas.geojson
```

**2. Archivos GPKG con capas geoespaciales de Nicaragua y Panamá**  

Se descargaron de [GDAM](https://gadm.org/).

## Procesamiento
Los datos de entrada se procesaron en el proyecto QGIS:  
```mapa-medidas-x-canton-desktop.qgz```

## Salidas
El mapa resultante puede visualizarse en:  
[https://github.com/analisis-accion-climatica-adaptacion/mapa-medidas-x-canton-desktop/blob/main/salidas/mapa-medidas-x-canton.pdf](https://github.com/analisis-accion-climatica-adaptacion/mapa-medidas-x-canton-desktop/blob/main/salidas/mapa-medidas-x-canton.pdf)
