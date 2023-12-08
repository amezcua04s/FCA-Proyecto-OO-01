# Diagrama de datos
- Cada tabla representa una entidad de la base de datos, y convergen si es que existe una entidad que use dos de ellas, creando una nueva entidad
<!--
@startuml

' avoid problems with angled crows feet
skinparam linetype ortho

entity "Alumno" as lmn {
  ID_Alumno : String
  Nombre_Alumno : String
  Estatus_Alumno : Boolean

}

entity "Grupo" as grp {
  ID_Grupo : String
  Materia_Grupo : String
  Estatus_Grupo : Boolean
}

entity "Tarjeta" as trj {
  ID_Tarjeta : String
  Estatus_Tarjeta : Boolean
}

entity "Alumno_Grupo_Asistencia" as AGP {
  ID_Asistencia : String
  ID_Alumno : String
  ID_Grupo : String
  Fecha : Date.now
  Estatus_Asistencia : Boolean
}

entity "Alumno_Grupo" as ALG{
  ID_NumeroLista : String
  ID_Alumno : String

  ID_Grupo : String
  Estatus_Alumno_Grupo : Boolean
}

entity "Alumno_Tarjeta" as LMTR{
  ID_Alumno : String
  ID_Tarjeta : String
  ID_Alumno_Tarjeta : String
  Estatus_Alumno_Tarjeta : Boolean

}

lmn }..|| AGP
trj ||..|| LMTR
lmn ||..|| LMTR
grp ||..|| AGP
grp ||..|| ALG
lmn }..|{ ALG

@enduml
-->
![Diagrama de datos](https://github.com/amezcua04s/FCA-Proyecto-OO-01/assets/119078847/b6a1f1c1-2d46-423b-a3a0-04bab819b0a3)
