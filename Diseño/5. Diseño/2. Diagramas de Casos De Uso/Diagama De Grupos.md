<!--@startuml

left to right direction
actor "Profesor" as fc

rectangle SATMI{

    usecase "UC-001: Registrar Grupo" as  UC1
    usecase "UC-004: Baja Grupo" as UC4
    usecase "UC-005: Borrar Alumno" as UC5 
    usecase "UC-009: Modificar Grupo" as UC9
    usecase "UC-006: Eliminar Tarjeta" as UC6

    UC4.>UC5: <<Include>>
    UC9.>UC4: <<Extend>>
    UC5.>UC6: <<Include>>


}
fc .-> UC1 
fc .-> UC4
fc .-> UC9 
@enduml 
-->

![image](https://github.com/amezcua04s/FCA-Proyecto-OO-01/assets/147119596/60e43e5e-5df8-445d-bb13-62c27e27a477)




