# Diagrama de secuencia: DS-005: Generar informe
- El diagrama representa la forma en la que se generará el informe de las asistencias dentro de la aplicación [SATMI](/Diseño/1.%20Propósito/Propósito.md), representa de forma simbólica los módulos involucrados y como se comunican entre sí para realizar la operación.
    - El diagrama inicia en el contexto donde la aplicación ya ha sido inicializada con éxito y ya existe un grupo registrado en el sistema con al menos un alumno.

![image](https://github.com/amezcua04s/FCA-Proyecto-OO-01/assets/147119596/30953652-df31-48fa-8086-05c0a3874666)


<!--@startuml 

title DS - 005: Generar Informe

Usuario -> AppUI: selecciona\n"Generar informe"
AppUI -> DataSource: generaInforme
DataSource -> InformeDAO: exportarInforme(Grupo)
InformeDAO -> SQLite: buscarAsistencia(Grupo)
SQLite --> 
<!--InformeDAO: List<registrosAsistencia>
InformeDAO --> 
<!--DataSource: Informe
AppUI -->
 <!--Usuario: "Ingrese el nombre\ndel archivo:"
Usuario --> 
<!--AppUI: nombreArchivo
AppUI --> 
<!--DataSource: nombreArchivo
DataSource --> 
<!--SQLite: nombreArchivo
SQLite -> SQLite: exportarInforme()
SQLite -->
<!--DataSource: returnInforme()
DataSource -->
<!--Usuario: Importe exitoso
@enduml
-->
