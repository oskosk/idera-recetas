---
 layout: default
---

idera-recetas
=============

Recetas para el uso y abuso de los recursos geoespaciales publicados en la Infraestructura de Datos espaciales de 
la República Argentina

##Capas disponibles en IDERA

Las capas de datos geoespaciales son publicadas en estándares bien definidos basados en servicios web. Estos estándares se denominan [WMS](https://es.wikipedia.org/wiki/Web_Map_Service), [WFS](https://es.wikipedia.org/wiki/Web_Feature_Service).

##Recetas de Apps Web

* Todo el código que sigue se puede copiar y pegar y es funcional sin descargar ninguna librería.
* Todos los ejemplos utilizan OpenLayers o LeafletsJS, a partir de la versión hosteada en [CDNJS](http://cdnjs.com).

### Utilizando OpenLayers 2.13.1


* [Mapa con una capa WMS de IDERA](http://jsbin.com/rirojuno/1/edit).
* [Mapa con dos capas de dos WMS distintos](http://jsbin.com/rirojuno/1/edit).

##Cómo usar las recetas

### Con minimo esfuezo usando un IFRAME y JS Bin

Como los ejemplos son de mapas fullscreen, podés 

* Entrar a [jsbin.com](http://jsbin.com).
* Acomodar las variables y capas que necesites mostrar
* Utilizar el link a tu Bin, pero en el modo output, *es decir, la URL de tu jsbin sin el `/edit`*

### Descargarndo el zip

* Te bajás el .zip de este repo.* 

##Algunos términos

### Capa Base disponibles para usar con IDERA.

Una capa base da contexto a los datos publicados por cada participantes de IDERA. Suelen publicarse a fin de ser desplegadas de manera de que para el usuario del mapa, las capas superpuestas, tenga un contexto territorial.

Entre las capas base que utilizo frecuentemente puedo mencionar 

Provistas por grandes empresas o proyectos

Estas capa sólo pueden ser utilizadas junto con servidores WMS de IDERA que soporten los Sistemas de Referencia Espacial `EPSG:3857` o `EPSG:900913`. Este sistema se suele denominar Spherical Pseudo Mercator.

* Imágenes satelitales de Google Maps API.
* Imágenes satelitales de Bing Maps API: 
* Mapa base publicado por el proyecto [OpenStreetMap](http://openstreetmap.org). Esta capa también
* Mapa base IGN (`capabaseargenmap`), provista por el [Instituto Geográfico Nacional](http://ign.gob.ar). 


#### Capa base Argenmap

El IGN publica en su servicio WMS, una capa de nombre `capabaseargenmap`. Esta es una capa del tipo *grupo de capas* de Geoserver. Esta capa *grupal* presenta algunas de las capas publicadas por el IGN estilizadas (utilizand SLD) de manera de que puedan servir como *mapa base* para otras capas de datos.

### Capas transparentes (Overlays)






##Software de Escritorio
