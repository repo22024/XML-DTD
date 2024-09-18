#OBJETIVO

El propósito del proyecto es aprender la estructura de los archivos XML y su validación mediante su correspondiente archivo DTD.

#INFORMACIÓN GENERAL

El lenguaje de marcado extensible (XML por sus siglas en inglés) es un formato simple basado en texto para representar la 
información de manera estructurada: documentos, datos, configuraciones, libros, transacciones, facturas, y mucho más.

XML
permite el intercambio de información entre sistemas informáticos, como sitios web, bases de datos y aplicaciones de terceros. 
Las reglas predefinidas facilitan la transmisión de datos como archivos XML a través de cualquier red, ya que el destinatario puede 
usar esas reglas para leer los datos de forma precisa y eficiente.

DTD - (Document Type Definition). 
Define la gramática a seguir en el documento XML para que éste sea considerado como válido. 
Puede incluirse en un fichero externo al XML, y/o incluirse dentro del propio fichero XML. raíz (también conocido como elemento documento).

#INFORMACIÓN DEL PROYECTO

El proyecto se base en la creación de un archivo XML, de nombre "tienda.xml" que agrupa los datos de dos subgrupos (Comidas y Clientes), estos subgrupos están compuestos por:
Comidas: comida (los datos de cada comida)
Clientes: cliente (los datos de cada cliente)
Comida:(idcomida, nombrecomida,especie, precio, peso)
Cliente:(idcliente, nombrecliente,telefono)

Toda la información y la estructura está validada por el fichero "tienda.dtd", que está vinculado internamente con el fichero (tienda.xml)
