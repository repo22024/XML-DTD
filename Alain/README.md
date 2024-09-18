# Clínica Veterinaria DB XML

Este proyecto gestiona datos para una Clinica Veterinaria, con estructuras XML y verificadores DTD. La gestión de datos del XML abarca el control de varias especies, como pacientes de la clínica, y sus dueños. 

## Comenzando

### Instalación

* Clon the repository: `https://github.com/repo22024/XML-DTD/tree/ea714b3cbd5fcfc6ac1b064d760a49be133f8573/Alain`

### Uso

* La gestión de datos del XML, como estructura de BD, abarca el control de varias especies, como pacientes de la clínica, y sus dueños. De la forma que está estructurado el XML admite la escalabilidad horizontal y vwertical que se requiera en un futuro.

* Actualmente consta de la seccion <clinica> como raiz del documento que contiene:
    * sección <pacientes> en un segundo nivel 
        * sección <mascotas> en un tercer nivel que contiene como padre la sección pacientes
            * sección <mascota> en un cuarto nivel que contiene como padre la sección mascotas
                * dentro de la sección <mascota> en un quinto  nivel los elementos:    
                    *                   <nombre>
                                        <especie>
                                        <raza>
                                        <edad>
                                        <id_dueño>
        * sección <dueños_mascotas> en un tercer nivel que contiene como padre la sección pacientes
            * sección <dueño_mascota> en un cuarto nivel que contiene como padre la sección dueños_mascotas
                * dentro de la sección <dueño_mascota> en un quinto  nivel los elementos: 
                    *                           <nombre>
                                                <telefono>
                                                  

## Autor

* AlainBC

## Licencia

This project is licensed under the MIT License.

