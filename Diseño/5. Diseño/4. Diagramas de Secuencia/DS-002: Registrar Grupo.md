# Diagrama de secuencia: DS-002: Registrar Grupo
- El diagrama representa la forma en la que se registra un grupo dentro de la aplicación [SATMI](/Diseño/1.%20Propósito/Propósito.md), representa de forma simbólica los módulos involucrados y como se comunican entre sí para realizar la operación.
    - El diagrama inicia en el contexto donde la aplicación ya ha sido inicializada con éxito.

<!-- @startuml 

title DS - 002: Registrar Grupo

Usuario -> AppUI: selecciona\n"Alta Grupo"
AppUI -->
<!-- Usuario: "Ingrese datos: "-->
<!-- Usuario -->
<!-- AppUI: ingresaDatos()
 alt Campos completos
AppUI -> DataSource: registrarGrupo
<!--DataSource -> GrupoDAO: registrarGrupo\n(Grupo)
GrupoDAO-> SQLite: guardarRegistro\n(nuevoGrupo)
SQLite -->
<!-- DataSource: returnResult(nuevoGrupo)
DataSource -->
<!-- AppUI: returnResult\n(nuevoGrupo)
<!--alt Registro exitoso
AppUI -->
<!-- Usuario: "Grupo\nregistrado"
else Registro no exitoso
AppUI -->
<!-- Usuario: "Grupo\nno registrado"
end
else Campos Incompletos
AppUI -> Usuario: "Campos\nincompletos")
end

@enduml-->
![image](https://github.com/amezcua04s/FCA-Proyecto-OO-01/assets/147119596/715d35c1-0212-4163-ad5f-221dc88fb9ee)

