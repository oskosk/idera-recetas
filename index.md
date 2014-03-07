---
 layout: default
---

idera-recetas
=============

Recetas para el uso y abuso de los recursos geoespaciales publicados en la Infraestructura de Datos espaciales de 
la República Argentina

##Capas disponibles en IDERA

Las capas de datos geoespaciales son publicadas en estándares bien definidos basados en servicios web. Estos estándares se denominan [WMS](https://es.wikipedia.org/wiki/Web_Map_Service), [WFS](https://es.wikipedia.org/wiki/Web_Feature_Service).


Podés encontrar el listado de servicios de la IDE en:

* [IDERA - Servicios IDE](http://www.idera.gob.ar/portal/node/21).
* [JSON con las URL de los WMS de IDERA](http://mapa.ign.gob.ar/idera.jquery/servicios_wms.json),


##Recetas de Apps Web

* Todo el código que sigue se puede copiar y pegar y es funcional sin descargar ninguna librería.
* Todos los ejemplos utilizan OpenLayers o LeafletsJS, a partir de la versión hosteada en [CDNJS](http://cdnjs.com).

### Utilizando OpenLayers 2.13.1

###Mapas con SRS EPSG:3857

* [Mapa con una capa WMS de IDERA](ejemplos/idera-epsg3857-openlayers-una-capa-wms.html).
* [Mapa con dos capas de dos WMS distintos](ejemplos/idera-epsg3857-openlayers-dos-capas-wms.html).

###Mapas con SRS EPSG:4326

* [Mapa con una capa WMS de IDERA](ejemplos/idera-epsg4326-openlayers-una-capa-wms.html).
* [Mapa con dos capas de dos WMS distintos](ejemplos/idera-epsg4326-openlayers-dos-capas-wms.html).

##Cómo usar las recetas

### Descargando el zip

Te bajás el .zip de este repo y te manejás.

### Si tenés un servidor web

* Copiá el código HTML de los ejemplos y customizalo en tu servidor web usando un editor de texto.

###Si no tenés un servidor web

* Abrí uno de los ejemplos
* Abrí el código fuente del ejemplo.
* Copiá el código fuente
* Entrá a [JS Bin](http://jsbin.com)
* Pegá el código fuente que copiaste, en el panel de la izquierda. Previsualizá el ejemplo
* Customizá los parámetros `zoom`, `lat`, `lon` e `ideraLayers` (en el caso de los ejemplos con más de una capa. En los ejemplos con una sóla capa, la variable a modificar es `ideraLayer`.

## Incrustá el mapa en otro HTML.

<iframe src="http://oskosk.github.io/idera-recetas/ejemplos/idera-epsg3857-openlayers-una-capa-wms.html">
</iframe>

{% highlight html %}
<iframe src=""></iframe>
{% endhighlight %}

 

Como los ejemplos son de mapas fullscreen, podés 

* Entrar a [jsbin.com](http://jsbin.com).
* Acomodar las variables y capas que necesites mostrar
* Utilizar el link a tu Bin, pero en el modo output, *es decir, la URL de tu jsbin sin el `/edit`*



##Algunos términos

### Capas base disponibles para usar con IDERA.

Una capa base da contexto a los datos publicados por cada participantes de IDERA. Suelen publicarse a fin de ser desplegadas de manera de que para el usuario del mapa, las capas superpuestas, tenga un contexto territorial.

Entre las capas base que utilizo frecuentemente puedo mencionar 

Provistas por grandes empresas o proyectos

Estas capas que menciono  sólo pueden ser utilizadas junto con servidores WMS de IDERA que soporten los Sistemas de Referencia Espacial `EPSG:3857` o `EPSG:900913`. Este sistema se suele denominar Spherical Pseudo Mercator. El mapa base IGN puede ser usado en varias proyecciones soportadas por el WMS del IGN.

* Imágenes satelitales de Google Maps API.
* Imágenes satelitales de Bing Maps API: 
* Mapa base publicado por el proyecto [OpenStreetMap](http://openstreetmap.org). Esta capa también
* Mapa base IGN (`capabaseargenmap`), provista por el [Instituto Geográfico Nacional](http://ign.gob.ar). 


#### Capa base Argenmap

El IGN publica en su servicio WMS, una capa de nombre `capabaseargenmap`. Esta es una capa del tipo *grupo de capas* de Geoserver. Esta capa *grupal* presenta algunas de las capas publicadas por el IGN estilizadas (utilizand SLD) de manera de que puedan servir como *mapa base* para otras capas de datos.


