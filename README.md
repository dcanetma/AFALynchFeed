# AFALynchFeed
Soy un robot que destaca trabajos periodísticos e investigaciones que tratan sobre sobre el cáncer de colon y endometrio hereditarios o **#síndromedeLynch**. Puedes ver los resultados en my perfil de Twitter [@AFALynchFeed](https://twitter.com/AFALynchFeed). Este es un proyecto especial de [@AFALynch](https://twitter.com/AFALynch) basado en el trabajo de [@FreedomofPress](https://twitter.com/FreedomofPress).

## Publicación de resultados

Puedes seguir los artículos publicados en el perfil de Twitter [@AFALynchFeed](https://twitter.com/AFALynchFeed). 

## Medios de noticias, ('outlets')

El fichero [rssfeeds.json](https://github.com/dcanetma/AFALynchFeed/blob/master/config/rssfeeds.json) contiene el listado con todos los orígenes de noticias que son rastreados periódicamente en la búsqueda de entradas que tengan que ver con nuestro tema principal de interés, el **síndrome de Lynch** o el cáncer de colon y endometrio hereditarios.

En este listado hemos incluido desde medios generalistas de noticias, hasta otras fuentes más especializadas en medicina, investigación médica, ciencia o tecnología. 

## Proponer nuevas fuentes de artículos

_¿Crees que falta algún medio de noticias online en la lista? ¿Conoces algún diario médico online que podría ser interesante? Te explicamos cómo._

Para leer las noticias, el robot emplea una fuente RSS. En el primer paso, se debe encontrar la URL del RSS en la página web de noticias que desees añadir. Si la página web tiene más de un RSS disponible, escogeremos el que incluya todas las noticias del sitio. 

> @todo: nota sobre criterio a emplear y tipos de noticias que se incluyen.

Los medios deben añadirse al fichero [rssfeeds.json](https://github.com/dcanetma/AFALynchFeed/blob/master/config/rssfeeds.json) en el siguiente formato (aquí el ejemplo de 'Gizmodo'):

````
  {
    "url": "https://gizmodo.com/rss",
    "outlet": "Gizmodo",
    "delicateURLs": false, // opcional, default: false, si true, no limpia las URLs de los artículos (e.j. borrando todo despues de '#' o '?')
    "redirectLinks": false // opcional, default: false, si true, sigue las redirecciones hasta encontrar la url última
  },
````

Las solicitudes de 'Pull requests' son bienvenidas. De lo contrario, también puedes abrir [un nuevo 'Issue'](https://github.com/dcanetma/AFALynchFeed/issues/new) indicando las URLS de los medios de noticias que faltan, para que los añadamos cuando sea posible.

## Palabras clave para el filtrado de noticias, ('matchwords')

Para filtrar qué noticias tratan sobre el síndrome de Lynch empleo una lista de palabras clave guardadas en un fichero. Cada línea contiene una frase, de una o más palabras, que de aparecer en un artículo será guardado en nuestra base de datos y publicado.

La frase debe coincidir de manera completa en el artículo y existe la posibilidad de indicar si se desea que coincidan mayúsculas y minúsculas.

## Solicitud de acceso a la base de datos de noticias

Mientras no están disponibles otros medios de acceso abierto, es posible bajo demanda solicitar la base de datos completa de resultados de este proyecto, con todos los artículos que han sido identificados con esta herramienta.

El proyecto emplea una base de datos en formato SQLite, y podemos entregar los datos en formato 'csv' y hoja de datos. 

## Créditos

> @todo
> Mención a proyecto original trackthenews

## Licencia

Datos: CC0

Code: MIT
