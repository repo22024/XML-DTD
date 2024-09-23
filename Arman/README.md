# 👨🏻‍💼 Empresa y Empleado

En este repositorio encontrara dos archivos: empresa.xml y empresa.dtd donde se registra información sobre los empleados y los proyectos en que trabajan

# 🛠️ Estructura del Archivo

La raíz `Empresa` contiene dos elementos `Empleados` y `Proyectos` 

En Empleados se recoge el id del empleado, el nombre, departamento al que pertenece, los proyectos en los que trabaja y la fecha de contratación.

En Proyectos esta registrado el id del proyecto, el nombre y el estado en que se encuentra, dentro de tres opciones posibles. 

```xml
<Empresa>
	<Empleados>
	  <Empleado IdEmpleado="" FechaContrato="AAAA-MM-DD">
	    <NombreEmpleado></NombreEmpleado>
      <Departamento></Departamento>
      <ProyectoAsignado></ProyectoAsignado>
    </Empleado>
        
	<Proyectos>
		<Proyecto Estado="Activo" IdProyecto="">
	    <NombreProyecto></NombreProyecto>
    </Proyecto>
  </Proyectos>
</Empresa>
```

# ⚠️Restricciones y consideraciones

- Cada empleado debe de tener un Id único
- Cada empleado puede tener asignado uno o mas proyectos
- La fecha de contratación debe de tener el formato AAA-MM-DD
- Los proyectos solo pueden tener uno de los siguientes estados: activo, completado, pausado

# 📝 Notas

Los archivos están codificados bajo el estándar UTF8 y CRLF

# 💾 Autoría

Realizado por Armando Malavé como práctica de XML y DTD
