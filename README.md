# Mapa de medidas de acción climática por cantón - versión escritorio
Este repositorio contiene los archivos necesarios para la construcción de un mapa que muestra la cantidad de medidas de acción climática en cada cantón de Costa Rica. Se desarrolló en el sistema de información geográfica de escritorio [QGIS](https://www.qgis.org/).

El mapa puede visualizarse en:  
???

## Entradas
Los datos de entrada iniciales están descritos en el [repositorio de la versión web de este mapa](https://github.com/analisis-accion-climatica-adaptacion/mapa-medidas-x-canton-web). Estos datos se copiaron al directorio ```/datos``` de este repositorio. El mapa se basa en el archivo con la capa de cantones y los datos de cantidad de medidas para cada uno.

```cantones-medidas.geojson```

Este archivo se transformó al SRS CRTM05 (EPSG = 5367) con el comando:

```
cd datos
ogr2ogr -t_srs EPSG:5367 cantones-medidas-crtm05.geojson cantones-medidas.geojson
```

El comando generó el archivo:

```cantones-medidas-crtm05.geojson```

## Procesamiento
Los datos de entrada se procesaron en el proyecto QGIS:  
```mapa-medidas-x-canton-desktop.qgz```

## Salidas
El resultante mapa puede visualizarse en:  
???
