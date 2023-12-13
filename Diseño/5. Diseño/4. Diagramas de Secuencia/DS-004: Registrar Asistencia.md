# Diagrama de secuencia: DS-004: Registrar Asitencia
- El diagrama representa la forma en la que se registra la asistencia de los alumnos dentro de la la aplicación [SATMI](/Diseño/1.%20Propósito/Propósito.md), representa de forma simbólica los módulos involucrados y como se comunican entre sí para realizar la operación.
    - El diagrama inicia en el contexto donde la aplicación ya ha sido inicializada con éxito y ya existe un grupo registrado en el sistema con al menos un alumno.

![DS 04 Registrar Asistencia](https://github.com/amezcua04s/FCA-Proyecto-OO-01/assets/119078847/d7003117-fbd0-492c-ab1e-4cec3a65d707)

<!--@startuml

title DS - 004: Registrar asistencia
  
  Usuario -> AppUI: Selecciona\n"RegistrarAsistencia"
  AppUI --> 
  <!--Usuario: "Esperando tarjeta"
  Usuario -> AppUI: acercaTarjeta
  AppUI -> DataSource: leerTarjeta()
  DataSource -> AsistenciaDAO: leerTarjeta()
  AsistenciaDAO -> SQLite: RegistrarAsistencia(Grupo)
  SQLite --> 
  <!--DataSource: returnAsistencia()
  DataSource --> 
  <!--AppUI: returnAsistencia()
  alt Asistencia registrada
  AppUI --> 
  <!--Usuario: "Asistencia registrada"
  else Asistencia previamente registrada
  AppUI --> 
  <!--Usuario: "Asistencia previamente registrada"
  else Tarjeta no reconocida
  AppUI --> 
  <!--Usuario: "Tarjeta inválida"
  end
@enduml-->
