<!-- @startuml
!theme vibrant

skin rose

title Clases - Sistema de toma de asistencia mediante tarjeta MI

class IdUnico{
  + identificador(codigoEntrada: String) : String
}

class Grupo extends IdUnico{
  # identificadorGrupo : IdUnico
  # materia : String
  # alumnos : List<Alumnos>
  # horasDeClase : HoraDeClase
  # diasDeClase : DiasDeClases
  - crearGrupo(IGrupo)
  - eliminarGrupo(IGrupo)
  - modificarGrupo (IGrupo)
}

enum HoraDeClase {
  · 7:00 
  · 9:00
  · 11:00
  · 13:00
  · 16:00
  · 18:00
  · 20:00
}

enum DiasDeClases{
  · Lunes
  · Martes
  · Miércoles
  · Jueves
  · Viernes
  · Sabádo
}

class Alumno  extends IdUnico{
  + nombre : String
  + tarjetaNFC : String
  + numeroCuenta : IdUnico
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
  + grupoInforme : Grupo
  + periodo : Date
  + exportarInforme (IPeriodo)
}

interface IGrupo extends IAlumno{
  # crearGrupo()
  # eliminarGrupo()
  # modificarGrupo()
}

interface IAlumno {
  # crearAlumno()
  # modificarAlumno()
  # eliminarAlumno()
}

interface ITarjeta extends Alumno{
  # registrarTarjeta()
  # eliminarTarjeta()
  # modificarTarjeta()
}

interface IPeriodo extends PeriodoInforme{
  + exportarInforme()
}


Grupo ..|> IGrupo : realización
Grupo "1"--"2..3" DiasDeClases
Grupo "1"--"1..2" HoraDeClase
Alumno "*" o-- "1" Grupo
Alumno ..|> IAlumno
Tarjeta ..|> ITarjeta
Tarjeta "1" --* "1" Alumno
Tarjeta ..> Alumno 
PeriodoInforme <-- Grupo

@enduml  
-->
# Diagrama de clases
![Diagrama de clasesv2](https://github.com/amezcua04s/FCA-Proyecto-OO-01/assets/119078847/3d3ab1c4-69be-4032-bb6d-b300f85df4c8)
