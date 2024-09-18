# Estudio de Música

## Descripción

El archivo XML musica.xml contiene información sobre canciones en un estudio d musica, incluye una lista de canciones con sus respectivos detalles.

## Estructura del archivo

El archivo XML tiene la siguiente estructura:

* `estudio`: elemento raíz que representa el estudio de música.
* `canciones`: elemento que contiene una lista de canciones.
* `cancion`: elemento que representa una canción individual, con los siguientes atributos y elementos:
 + `id_cancion`: atributo que identifica de manera única a la canción.
 + `categoria`: atributo que indica la categoría de la canción ( "rock","pop" o "jazz").
 + `titulo`: elemento que contiene el título de la canción.
 + `artista`: elemento que contiene el nombre del artista o artistas que interpretan la canción.
 + `album`: elemento que contiene el título del álbum en el que se encuentra la canción.
 + `duracion`: elemento que contiene la duración de la canción en formato "minutos:segundos".

## Ejemplo de contenido

El archivo XML incluye los siguientes ejemplos de canciones:

* "Propuesta" de Buena Fe, del álbum "Corazonero", con una duración de 3:15 minutos.
* "Así fue" de Juan Grabiel e Isabel Pantoja, del álbum "Desde Andalucía", con una duración de 3:42 minutos.
* "Copacabana" de Barry Manilow, del álbum "Even Now", con una duración de 4:07 minutos.

## Uso

Este archivo XML puede ser utilizado para almacenar y recuperar información sobre canciones en un estudio de música. Puede ser parseado y procesado utilizando herramientas de procesamiento de XML para obtener la información deseada.

## Notas

* El archivo XML utiliza la codificación UTF-8 para garantizar la compatibilidad con caracteres especiales y símbolos.
* El archivo XML incluye una declaración de tipo de documento (DTD) para definir la estructura y los elementos permitidos en el archivo.