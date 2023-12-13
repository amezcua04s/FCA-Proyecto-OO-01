<!-- @startuml

left to right direction
actor "Profesor" as fc

rectangle SistemaAsistencias{

    usecase "UC-002: Registrar Alumno" as UC2
    usecase "UC-005: Borrar Alumno" as UC5
    usecase "UC-007: Modificar Tarjeta" as UC7
    usecase "UC-008: Modificar Alumno" as UC8
    usecase "UC-010: Generar Informe" as UC10
    usecase "UC-011: Registro de asistencia" as UC11
    usecase "UC-003: Registrar Tarjeta MI" as UC3
    usecase "UC-006: Eliminar Tarjeta" as UC6

    UC2-left.>UC3: <<Include>>
    UC5-down.>UC6: <<Include>>
    UC7-left.>UC6: <<Include>>
    UC7-up.>UC3: <<Include>>
    UC8-down.>UC7: <<Extend>>
}

fc -> UC2
fc -> UC5
fc -> UC8
fc -> UC10
fc .-> UC11

@enduml -->

![image](https://github.com/amezcua04s/FCA-Proyecto-OO-01/assets/147119596/7352952c-4380-4b3d-aed4-0fe71c01d1d6)

