# Diagrama de datos
- Cada tabla representa una entidad de la base de datos, y como es que se relacionan, para guardar la información de forma óptima.
    - La entidad transitiva "Alumno_Grupo" representa la lista de alumnos que pertenecen a un grupo.
    - La entidad transitiva "Asistencia" representa la asistencia que tuvo cada alumno en un grupo en específico.
<!--
@startuml

' avoid problems with angled crows feet
skinparam linetype ortho

entity "Alumno" as lmn {
  ID_Alumno : String
  Nombre_Alumno : String
}

entity "Grupo" as grp {
  ID_Grupo : String
  Materia_Grupo : String
}

entity "Tarjeta" as trj {
  ID_Tarjeta : UUID
}

entity "Asistencia" as AGP {
  ID_Asistencia : String
  ID_Alumno : String
  ID_Grupo : String
  Materia_Grupo : String
  Nombre_Alumno : String
  Fecha : Date.now
}

entity "Alumno_Grupo" as ALG{
  ID_NumeroLista : String
  Nombre_Alumno : String
  Materia_Grupo : String
}

AGP ||..|{ lmn
lmn ||..|| trj
grp ||..|| AGP
grp ||..|| ALG
lmn }..|{ ALG

@enduml-->
![image](https://github.com/amezcua04s/FCA-Proyecto-OO-01/assets/147119596/cf895be2-1d8a-40b3-b78b-6bf7ea3072af)

