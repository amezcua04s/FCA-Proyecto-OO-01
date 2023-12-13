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
# Diagrama de casos de uso de grupos
### El siguiente diagrama muestra como es que se relacionan los caso de uso de grupos entre ellos, y con el actor que será el profesor que esté utilizando el sistema.
![image](https://github.com/amezcua04s/FCA-Proyecto-OO-01/assets/147119596/3309dfa1-1447-45f9-a26c-96ba169f2733)





