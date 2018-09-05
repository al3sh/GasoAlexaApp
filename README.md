# GasoAlexaApp

## Gasolineras API

## Endpoints

## Endpoint para precios (Prices)

Obtener todo: Regresa todos los registros almacenados en la base de datos. Ejemplo: /prices/all
Por id: Permite buscar las gasolineras por el id asociado. Ejemplo: /prices/place/2039
Por typo de combustible: Permite obtener las gasolineras que surten un tipo de combustible. Ejemplo: /prices/type/premium

## Endpoint para lugares (Places)

Obtener todo: Regresa todos los registros almacenados en la base de datos. Ejemplo: /places/all
Por id: Permite buscar las gasolineras por el id asociado. Ejemplo: /places/place/2039
Por ubicación: Como parametros recibe latitud, longitud y radio para regresar las gasolineras en ese rango. Ejemplo: /places/location/32.47641,-116.9214/6

## Archivo cron

Este archivo consulta el registro de estaciones de servicio gasolineras y precios comerciales de gasolina y diesel proporcinado por la comisión reguladora de energia (https://datos.gob.mx/busca/dataset/estaciones-de-servicio-gasolineras-y-precios-comerciales-de-gasolina-y-diesel). Es necesario ejecutarlo al menos una vez y se recomienda agregar un cron de unix cada 24 horas para la ingesta de los datos. En la base de datos se almacena el registro historico para futuras implementaciones de análisis de datos.
