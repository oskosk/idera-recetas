---
 layout: default
---

idera-recetas
=============

Recetas para el uso y abuso de los recursos geoespaciales publicados en la Infraestructura de Datos espaciales de 
la República Argentina

##Capas disponibles en IDERA

Las capas de datos geoespaciales son publicadas en estándares bien definidos basados en servicios web. Estos estándares se denominan [WMS](https://es.wikipedia.org/wiki/Web_Map_Service), [WFS](https://es.wikipedia.org/wiki/Web_Feature_Service).

##Definiciones

### Capas Base

Estas son capas que dan contexto a los datos publicados por cada participantes de IDERA. Suelen publicarse a fin de ser desplegadas sin transparencias, de manera que las capas superpuestas, sean generalmente transparentes a fin de que el usuario de las capas, no pierda contexto para su capa de interés. Entre las capas base que utilizo frecuentemente puedo mencionar * Imágenes satelitales de Google Maps API.

* Imágenes satelitales de Bing Maps API.
* Mapa base generada por el proyecto [OpenStreetMap](http://openstreetmap.org). 
* Mapa base IGN (`capabaseargenmap`), provista por el [Instituto Geográfico Nacional](http://ign.gob.ar). 


#### Capa base Argenmap

El IGN publica en su servicio WMS, una capa de nombre `capabaseargenmap`. Esta es una capa del tipo *grupo de capas* (así lo permite Geoserver). La capa presenta las capas publicadas por el IGN estilizadas (utilizand SLD) de manera de que puedan servir como soporte a otros datos que se deseen desplegar sobre un mapa.

### Capas transparentes (u Overlays)

##Apps Web

* Todo el código que sigue se puede copiar y pegar y es funcional sin descargar ninguna librería.
* Todos los ejemplos utilizan OpenLayers o LeafletsJS, a partir de la versión hosteada en [CDNJS](http://cdnjs.com). [CDN](https://es.wikipedia.org/wiki/Content_delivery_network)s.

### Utilizando OpenLayers 2.13.1


* [Mapa con una capa WMS de IDERA](http://jsbin.com/rirojuno/1/edit).
* [Mapa con dos capas de dos WMS distintos](http://jsbin.com/rirojuno/1/edit).


http://jsbin.com/rirojuno/1/edit




##Software de Escritorio
