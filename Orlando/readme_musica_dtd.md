# musica.dtd README
=====================

## Descripción general
-----------

Este archivo de definición de tipo de documento (DTD) `musica.dtd` define la estructura y organización de un documento XML para almacenar datos relacionados con la música.

## Propósito
----------

El propósito de este DTD es proporcionar una forma estandarizada de representar datos de música en un formato XML, lo que permite un intercambio y procesamiento fácil de la información de música entre diferentes sistemas y aplicaciones.

## Estructura
------------

El archivo `musica.dtd` define los siguientes elementos y atributos:

### Elementos

* **canción**: representa una canción individual, con atributos:
	+ **título**: el título de la canción
	+ **artista**: el artista o banda que interpreta la canción
	+ **género**: el género de la canción (por ejemplo, rock, pop, jazz, etc.)
	+ **duración**: la duración de la canción en segundos
* **álbum**: representa un álbum de música, con atributos:
	+ **título**: el título del álbum
	+ **artista**: el artista o banda que interpreta el álbum
	+ **fecha de lanzamiento**: la fecha de lanzamiento del álbum
	+ **canciones**: una lista de elementos **canción**

### Atributos

* **id**: un identificador único para cada elemento **canción** o **álbum**

## Ejemplo de uso
----------------

Aquí hay un ejemplo de cómo podrías utilizar el archivo `musica.dtd` para definir un documento XML:
```xml
<?xml version="1.0" encoding="UTF-8"?>
<!DOCTYPE musica SYSTEM "musica.dtd">
<musica>
  <álbum título="El muro" artista="Pink Floyd" fecha de lanzamiento="1979-11-30">
    <canciones>
      <canción título="Otro ladrillo en el muro (Parte 2)" artista="Pink Floyd" género="rock" duración="240"/>
      <canción título="Madre" artista="Pink Floyd" género="rock" duración="210"/>
      <!-- más canciones -->
    </canciones>
  </álbum>
</musica>