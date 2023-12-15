<!--@startuml

!theme vibrant

skin rose

title Clases - "SATMI"

class Grupo{
  # identificadorGrupo : String
  # materia : String
  # alumnos : List<Alumnos>
}

class Alumno{
  + nombre : String
  + tarjetaNFC : UUID
  + numeroCuenta : String
}

class Tarjeta {
  + numeroTarjeta : UUID
}

class RegistrarAsistencia{
  - Asistencia : <List>
}

class Informe{
  + crearInforme(Grupo)
}

interface DataSource{
  + GrupoDAO()
  + AlumnoDAO()
  + TarjetaDAO()
  + AsistenciaDAO()
  + InformeDAO()
}

class GrupoDAO{
  - registrarGrupo(Grupo)
  - eliminarGrupo(Grupo, List<Alumnos>)
  - modificarGrupo (Grupo, List <Alumnos>)
  - consultarGrupo(Grupo)
}

class AlumnoDAO{
  - consultarAlumno(Alumno)
  - registrarAlumno(Alumno)
  - modificarAlumno(Alumno)
  - bajaAlumno(Alumno)
}

class TarjetaDAO{
  - registrarTarjeta(Tarjeta)
  - modificarTarjeta(Tarjeta)
  - eliminarTarjeta(Tarjeta)
}

class AsistenciaDAO{
  + RegistrarAsistencia(Grupo)
  - LeerTarjeta()
}

class InformeDAO{
  + exportarInforme()
}


Grupo -> DataSource
DataSource <- RegistrarAsistencia
Alumno "*" o-- "1" Grupo
Alumno -> DataSource
Tarjeta -> DataSource
Tarjeta "1" --* "1" Alumno
Informe ..> DataSource

DataSource -> GrupoDAO
DataSource -> AlumnoDAO
DataSource -> TarjetaDAO
DataSource -> AsistenciaDAO
DataSource -> InformeDAO
@enduml  -->
# Diagrama de clases
## El diagrama representa las clases e interfaces que conforman el sistema y cómo es que se relacionan entre ellas. 
![image](https://github.com/amezcua04s/FCA-Proyecto-OO-01/assets/147119596/71e6e091-83cb-4c5b-b89d-7409e4f833fc)

