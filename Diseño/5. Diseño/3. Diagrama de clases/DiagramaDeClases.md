<!-- @startuml
!theme vibrant

!theme vibrant

skin rose

title Clases - Sistema de toma de asistencia mediante tarjeta MI

class Grupo{
  # identificadorGrupo : String
  # materia : String
  # alumnos : List<Alumnos>
}

class Alumno{
  + nombre : String
  + tarjetaNFC : String
  + numeroCuenta : String
  - crearAlumno(IAlumno)
  - modificarAlumno(IAlumno)
  - eliminarAlumno(IAlumno)
}

class Tarjeta {
  + numeroTarjeta : IdUnico
  - registrarTarjeta(ITarjeta)
  - eliminarTarjeta(ITarjeta)
  - modificarTarjeta(ITarjeta)
}

class PeriodoInforme{
  + crearInforme(Grupo)
}

class RegistrarAsistencia{
  - Asistencia : <List>
}

interface GrupoDAO{
  - registrarGrupo(Grupo)
  - eliminarGrupo(Grupo, List<Alumnos>)
  - modificarGrupo (Grupo, List <Alumnos>)
  - consultarGrupo(Grupo)
}

interface AlumnoDAO{
  - registrarAlumno(Alumno)
  - modificarAlumno(Alumno)
  - bajaAlumno(Alumno)
}

interface TarjetaDAO{
  - registrarTarjeta(Tarjeta)
  - modificarTarjeta(Tarjeta)
  - eliminarTarjeta(Tarjeta)
}

interface AsistenciaDAO extends Grupo{
  + RegistrarAsistencia(Grupo)

}

interface PeriodoDAO extends PeriodoInforme{
  + exportarInforme()
}


Grupo ..|> GrupoDAO
Alumno "*" o-- "1" Grupo
Alumno ..|> AlumnoDAO
Tarjeta ..|> TarjetaDAO
Tarjeta "1" --* "1" Alumno
PeriodoInforme <-- Grupo
AsistenciaDAO <-- RegistrarAsistencia

@enduml  -->
# Diagrama de clases
- El diagrama representa las clases e interfaces que conforman el sistema y como es que se relacionan entre ellas. 
![Diagrama de clases](https://github.com/amezcua04s/FCA-Proyecto-OO-01/assets/119078847/ec7094e5-bd84-4624-9ca6-bf2d60cec7cc)
