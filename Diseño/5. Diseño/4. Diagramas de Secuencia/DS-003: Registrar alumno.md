# Diagrama de secuencia: DS-003: Registrar alumno
- El diagrama representa la forma en la que se registra un nuevo alumno dentro de la la aplicación [SATMI](/Diseño/1.%20Propósito/Propósito.md), representa de forma simbólica los módulos involucrados y como se comunican entre sí para realizar la operación.
    - El diagrama inicia en el contexto donde la aplicación ya ha sido inicializada con éxito y ya existe un grupo registrado en el sistema.

![DS 003 RegistrarAlumno](https://github.com/amezcua04s/FCA-Proyecto-OO-01/assets/119078847/8b2ce012-9763-4ab7-87f1-ef365c3a123b)
    
<!--@startuml 

title DS - 003: Registrar Alumno

Usuario -> AppUI: selecciona\n"Alta Alumno"
AppUI -->
<!-- Usuario: "Ingrese datos: "
Usuario --> 
<!--AppUI: ingresaDatos()
alt Campos completos
AppUI -> DataSource: registraAlumno
DataSource -> alumnoDAO: altaAlumno\n(datosAlumno)
alumnoDAO -> alumnoDAO: nuevoAlumno
alumnoDAO -> SQLite: guardarRegistro\n(alumnoNuevo)
SQLite --> 
<!--DataSource: returnResult(alumnoNuevo)
DataSource --> 
<!--AppUI: returnResult\n(alumnoNuevo)
alt Registro exitoso
AppUI --> 
<!--Usuario: "Alumno\nregistrado"
else Registro no exitoso
AppUI --> 
<!--Usuario: "Alumno\nno registrado"
end
else Campos Incompletos
AppUI -> Usuario: "Campos\nincompletos")
end

@enduml-->