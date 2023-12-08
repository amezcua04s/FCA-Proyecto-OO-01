<!--@startuml

left to right direction
actor "Profesor" as fc

rectangle SistemaAsistencias{

    usecase "UC-001: Registrar Grupo" as  UC1
    usecase "UC-004: Baja Grupo" as UC4
    usecase "UC-005: Borrar Alumno" as UC5 
    usecase "UC-009: Modificar Grupo" as UC9

    UC4.>UC5: <<Include>>
    UC9.>UC4: <<Extend>>


}
fc .-> UC1 
fc .-> UC4
fc .-> UC9 
@enduml 
-->

![image](https://github.com/amezcua04s/FCA-Proyecto-OO-01/assets/147119596/9ab622b0-8e48-4151-bd5c-a1dae660239a)

