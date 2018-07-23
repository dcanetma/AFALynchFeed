# AFALynchFeed
Soy un robot que destaca trabajos periodísticos e investigaciones que tratan sobre sobre el cáncer de colon y endometrio hereditarios o #síndromedeLynch. Puedes ver los resultados en my perfil de Twitter @AFALynchFeed. Este es un proyecto especial de @AFALynch basado en el trabajo de @FreedomofPress.

## Medios de noticias, ('outlets')

El fichero 'config/rssfeeds.json' contiene el listado con todos los orígenes de noticias que son rastreados periódicamente en la búsqueda de entradas que tengan que ver con nuestro tema principal de interés, el síndrome de Lynch.

En este listado hemos incluido desde medios generalistas de noticias, hasta otras fuentes más especializadas en medicina, investigación médica, ciencia o tecnología. 

> ¿Crees que falta algún medio en la lista? ¿Conoces algún diario médico que podría ser interesante? Envíanos la dirección, o haz una solicitud de cambio en este proyecto, y la consideraremos. Ten en cuenta las siguientes instrucciones.

## Palabras clave para el filtrado de noticias, ('matchwords')

Para detectar qué noticias tratan sobre el síndrome de Lynch empleo una lista de palabras clave guardadas en un fichero. Cada línea contiene una frase, de una o más palabras, que de aparecer en un artículo será guardado en nuestra base de datos y publicado.

La frase debe coincidir de manera completa en el artículo y existe la posibilidad de indicar si se desea que coincidan mayúsculas y minúsculas.

Los ficheros que se ocupan de esta función són:

- config/matchwords.txt
- config/matchwords-matchcase.txt

## Publicación de resultados

Puedes seguir los artículos publicados en el perfil de Twitter @AFALynchFeed. 

## Solicitud de acceso a la base de datos de noticias

@todo

## Créditos

> @todo
> Mención a proyecto original trackthenews
