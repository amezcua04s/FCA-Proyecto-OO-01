# Registrar Asistencia
- El diagrama de estados de "Registrar Asistencia" representa visualmente los diferentes estados y transiciones que experimenta el sistema cuando se quiere hacer el registro de Asistencia en el sistema [SATMI](/Diseño/Proposito.md), desde el inicio hasta la finalización del proceso.

![image](https://github.com/amezcua04s/FCA-Proyecto-OO-01/assets/147119596/d37ff796-35ee-465b-8277-9ca361e5a24f)




<!--
@startuml
scale 500 width
scale 300 


state Registrar_Asistencia {
state c <<choice>>


[*] -- Mateia_Seleccionaa: Selecciona Materia
Grupo_Seleccionado : Selecciona Grupo
Grupo_Seleccionado -- c : Acerca Tarjeta a Lector
c -- Tarjeta_Leída : Aceptada
c -- Tarjeta_No_Leída : En espera
Tarjeta_No_Leída -- [*]
Tarjeta_Leída --  Asistencia_Registrada : Confirma Asistencia
Asistencia_Registrada -- [*]
}

@enduml

-->
