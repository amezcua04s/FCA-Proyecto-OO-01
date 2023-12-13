# Diagrama de secuencia: DS-002: Registrar grupo
- El diagrama representa la forma en la que se registra un grupo dentro de la aplicación [SATMI](/Diseño/1.%20Propósito/Propósito.md), representa de forma simbólica los módulos involucrados y como se comunican entre sí para realizar la operación.
<!-- @startuml 

title DS - 002: Registrar Alumno

Usuario -> AppUI: selecciona\n"Alta Grupo"
AppUI --><!-- Usuario: "Ingrese datos: "-->
<!-- Usuario --><!-- AppUI: ingresaDatos()
<!-- alt Campos completos
AppUI -> DataSource: registrarGrupo
<!--DataSource -> GrupoDAO: registrarGrupo\n(Grupo)
GrupoDAO -> GrupoDAO: nuevoGrupo
GrupoDAO-> SQLite: guardarRegistro\n(nuevoGrupo)
SQLite --><!-- DataSource: returnResult(nuevoGrupo)
<!--DataSource --><!-- AppUI: returnResult\n(nuevoGrupo)
<!--alt Registro exitoso
AppUI --><!-- Usuario: "Grupo\nregistrado"
<!--else Registro no exitoso
AppUI --><!-- Usuario: "Grupo\nno registrado"
<!--end
else Campos Incompletos
AppUI -> Usuario: "Campos\nincompletos")
end

@enduml-->
![DS 02 REGISTRAR GRUPO](https://github.com/amezcua04s/FCA-Proyecto-OO-01/assets/119078847/6565bcce-1095-469d-b128-d0bf603c4d0c)
