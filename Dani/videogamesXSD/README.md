# Sistema de Biblioteca de Videojuegos

#### *Autor: Marcelo Daniel Choque Mamain*
#### *Curso: Sistema de Gestion de información*
#### *Modulo: Creacion y gestion de repositorios de contenidos*

## Descripción
Este proyecto implementa un sistema de biblioteca para registrar videojuegos utilizando un documento XML validado mediante un fichero XSD [fichero](https://github.com/repo22024/XML-DTD/blob/main/Dani/videogamesXSD/videogamesVal.xsd). Cada videojuego cuenta con detalles como su título, plataforma, precio y stock disponible.

## Archivos del Proyecto

1. **videojuegos.xml**: Archivo XML que contiene la información sobre los videojuegos.
2. **videojuego.dtd**: Archivo DTD que define y valida la estructura de `videojuego.xml`.
3. **README.md**: Archivo explicativo sobre el proyecto y las validaciones implementadas.

## Descripción del XML

El documento XML contiene una lista de videojuegos, representados con el elemento `<videojuego>`. Cada videojuego tiene la siguiente información:

- **Título**: Nombre del videojuego (`<titulo>`).
- **Plataforma**: La plataforma en la que está disponible (PC, PS5, Xbox).
- **Precio**: El costo del videojuego, expresado en formato decimal (`<precio>`).
- **Stock**: La cantidad de unidades disponibles en el inventario (`<stock>`).

Además, cada elemento `<videojuego>` tiene un atributo `id`, que es un identificador único para cada videojuego.

### Ejemplo de Estructura XML

```xml
    <videojuego idvendedor="V001" plataforma="PS5">
        <titulo>Grand Theif Auto San Andreas</titulo>
        <precio>59.99</precio>
        <stock>20</stock>
    </videojuego>
