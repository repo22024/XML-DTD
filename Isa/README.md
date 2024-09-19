# Título del Proyecto

Paquetes de Agencia de Viajes, este archivo XML contiene la descripción de varios paquetes de viaje ofrecidos por una agencia de viajes.

## Descripción de los Elementos 

ELEMENTOS DEL XML:

Elemento raíz:
·agencia
Elemento que contiene todos los paquetes de viaje.

Elementos secundarios:
·paquetes
Contiene uno o más elementos paquete.

·paquete
Representa un paquete de viaje individual. Tiene un atributo idpaquete que identifica de manera única cada paquete.

Atributos:
 idpaquete: Identificador único del paquete, tipo ID, que es obligatorio (#REQUIRED).

Sub-elementos (paquete):
 ·destino: Destino del paquete de viaje. Utiliza CDATA para permitir caracteres especiales.
 ·precio: Precio del paquete de viaje, contiene datos de carácter (#PCDATA) numérico y decimal.
 ·actividad: Lista de actividades incluidas en el paquete. Contiene datos de carácter (#PCDATA).

Sub-elementos (actividad):
 nombre: Nombre de la actividad, contiene datos de carácter (#PCDATA).
 duracion: Duración de la actividad en horas, contiene datos de carácter (#PCDATA), numéricos y mayores que 0.
 descripcion: Descripción detallada de la actividad, contiene datos de carácter (#PCDATA).

VALIDACIONES CON EL DTD:

paquete: Debe tener un atributo idpaquete único y obligatorio, contiene los elementos destino, precio y uno o más elementos actividad.

paquetes: Debe contener al menos un elemento paquete.

actividad: Debe contener los elementos nombre, duracion y descripcion en ese orden.

Esta estructura asegura que cada paquete tenga un destino, un precio y al menos una actividad, y que cada actividad esté detallada con un nombre, una duración y una descripción. 

## Construido Con 🛠️

- [XML] - El lenguaje utilizado - lenguaje de marcado que proporciona reglas para definir cualquier dato
- [DTD]- Definición de tipo de documento - conjunto de reglas sintácticas para definir etiquetas
 

## Autor ✒️

- **Isana M. G.** - _Trabajo de práctica_ - XML y DTD



## Estructura del XML Y DTD

```xml
<?xml version="1.0" encoding="UTF-8"?>
<!DOCTYPE agencia PUBLIC "public-id" "agencia.dtd">
<agencia>
    <paquetes>
        <paquete idpaquete="P01">
            <destino><![CDATA[Londres, City Airport]]></destino>
            <precio>1500.00</precio>
            <actividad>
               <nombre>Primer día: centro de Londres</nombre>
               <duracion>9</duracion>
               <descripcion>Visita a Piccadilly Circus: plaza de Picadilly, visita al Museo The National Gallery, recorrido por la avenida The Mall para ver el Buckingham Palace,
                parada para almorzar, continuamos el recorrido para visitar la Abadía de Westminster, el Big Ben y, al cruzar el río Támesis, visitar la noria London Eye. </descripcion>
            </actividad>
            <actividad>
                <nombre>Segundo día: Bethnal Green y Camden Market</nombre>
                <duracion>6</duracion>
                <descripcion>Descubrir la vida en las calles londinenses y sus mercados: Visita a Bethnal Green Road, visita al mercadillo Broadway Market,
                 viaje hasta Camden para visitar su mercado y el Stables Market</descripcion>
             </actividad>
             <actividad>
                <nombre>Tercer día: Parque Olímpico o Hyde Park + British Museum</nombre>
                <duracion>6</duracion>
                <descripcion>Visita al Parque Olímpico Reina Isabel y los alrededores de Stratford, Alternativa: Hyde Park y Momias Egípcias</descripcion>
             </actividad>
        </paquete>
        <paquete idpaquete= "P02">
            <destino><![CDATA[Mediterráneo, crucero]]></destino>
            <precio>1030.00</precio>
            <actividad>
               <nombre>Crucero: Costa Deliziosa</nombre>
               <duracion>192</duracion>
               <descripcion>Itinerario de 8 días por el Mediterráneo: Bari (salida), Kotor, Corfú, Katákolo/Olimpia, Dubrovnik, Split, Marghera/Venecia, Bari (Llegada)</descripcion>
            </actividad>
        </paquete>
        <paquete idpaquete= "P03">
            <destino><![CDATA[Portugal, Aeropuerto de Oporto-Francisco Sá Carneiro]]></destino>
            <precio>980.00</precio>
            <actividad>
               <nombre>Primer día visita guiada por Oporto</nombre>
               <duracion>4</duracion>
               <descripcion>Visita a la Catedrál de Oporto, Palacio de la Bolsa, Ribeira, Vila Nova de Gaia, Puente de Don Luis; el resto del día libre</descripcion>
            </actividad>
            <actividad>
                <nombre>Segundo día visita guiada por Oporto</nombre>
                <duracion>5</duracion>
                <descripcion>Visita a las Iglesias do Carmo y Carmelitas, Librería Lello, Iglesia de San Ildefonso, Café Majestic (parada para tomar algo), Capilla de las Almas, Mercado do Bolhão,
                 Ayuntamiento de Oporto</descripcion>
             </actividad>
             <actividad>
                <nombre>Tercer día visita guiada por Oporto</nombre>
                <duracion>4</duracion>
                <descripcion>Visita a la Estación São Bento, Aveiro, Costa Nova, Jardines del Palacio de Cristal, Praia do Carneiro, Faro de Felgueiras</descripcion>
             </actividad>
        </paquete>
        <paquete idpaquete= "P04">
            <destino><![CDATA[Japón, Aeropuerto Internacional de Chubu Centrair (NGO)]]></destino>
            <precio>2350.00</precio>
            <actividad>
               <nombre>Día 1: Visita guiada por la prefectura de Aichi</nombre>
               <duracion>11</duracion>
               <descripcion>Recorrido en autobús de 1 día por el Parque Ghibli desde Nagoya, con descanso para almorzar y merendar</descripcion>
            </actividad>
            <actividad>
                <nombre>Día 2: Visita guiada por la prefectura de Aichi</nombre>
                <duracion>7</duracion>
                <descripcion>Excursión de un día a Shirakawago, Takayama y gujo hachiman desde Nagoya</descripcion>
             </actividad>
             <actividad>
                <nombre>Día 3: Visita guiada por la prefectura de Aichi</nombre>
                <duracion>6</duracion>
                <descripcion>Visita a los museos de Nagoya (traslado en vehículo): Museo Conmemorativo de Tecnología e Industria de Toyota, Nagoya City Science Museum,
                 Tokugawa Art Museum, Noritake no Mori, The Yamazaki Mazak Museum of Art, a mitad del tour se hará un recorrido a pie por la comida callejera de Nagoya de Osu</descripcion>
             </actividad>
             <actividad>
                <nombre>Día 4: Visita guiada por la prefectura de Aichi</nombre>
                <duracion>5</duracion>
                <descripcion> Visita a la Ciudad de Morioka y sus alrededores</descripcion>
             </actividad>
        </paquete>   
    </paquetes>
</agencia>

## Estructura del DTD

<!ELEMENT agencia (paquetes)>
<!ELEMENT paquetes (paquete+)>
<!ELEMENT paquete (destino, precio, actividad+)>

<!ATTLIST paquete idpaquete ID #REQUIRED>
<!ELEMENT destino (#PCDATA)>
<!ELEMENT precio (#PCDATA)>
<!ELEMENT actividad (nombre, duracion, descripcion)>

<!ELEMENT nombre (#PCDATA)>
<!ELEMENT duracion (#PCDATA)>
<!ELEMENT descripcion (#PCDATA)>
