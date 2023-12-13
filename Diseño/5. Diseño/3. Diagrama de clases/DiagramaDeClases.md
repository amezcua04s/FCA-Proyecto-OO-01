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
## El diagrama representa las clases e interfaces que conforman el sistema y como es que se relacionan entre ellas. 
![Diagrama de clases](https://github.com/amezcua04s/FCA-Proyecto-OO-01/assets/119078847/e30956d9-a36e-4822-bffc-a7aa37e3e822)
