# Registrar Asistencia
- El diagrama de estados de "Registrar Asistencia" representa visualmente los diferentes estados y transiciones que experimenta el sistema cuando se quiere hacer el registro de Asistencia en el sistema SATMI, desde el inicio hasta la finalización del proceso.

![Captura de Pantalla 2023-12-12 a la(s) 0 04 01](https://github.com/amezcua04s/FCA-Proyecto-OO-01/assets/125850397/068134ec-790c-4a39-8ebf-667ae4e94892)



<!--
@startuml
scale 500 width
scale 300 


state Registrar_Asistencia {
state c <<choice>>


[*] -- Grupo_Seleccionado : Selecciona Grupo
Grupo_Seleccionado -- c : Acerca Tarjeta a Lector
c -- Tarjeta_Leída : Aceptada
c -- Tarjeta_No_Leída : En espera
Tarjeta_No_Leída -- [*]
Tarjeta_Leída --  Asistencia_Registrada : Confirma Asistencia
Asistencia_Registrada -- [*]
}

@enduml

-->
