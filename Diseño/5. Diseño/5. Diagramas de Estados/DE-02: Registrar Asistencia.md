# Registrar Asistencia

![Captura de Pantalla 2023-12-08 a la(s) 0 05 39](https://github.com/amezcua04s/FCA-Proyecto-OO-01/assets/125850397/7b371ce8-a25c-422a-bc91-58d35b2ace5e)



<!--
@startuml
scale 500 width
scale 300 


state Registrar_Asistencia {
state c <<choice>>


[*] --> Grupo_Seleccionado : Selecciona Grupo
Grupo_Seleccionado --> c : Acerca Tarjeta a Lector
c --> Tarjeta_Leída : Aceptada
c --> Tarjeta_No_Leída : En espera
Tarjeta_No_Leída --> [*]
Tarjeta_Leída --> Asistencia_Registrada : Confirma Asistencia
Asistencia_Registrada --> [*]
}

@enduml

-->
