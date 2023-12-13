<!-- @startuml

left to right direction
actor "Profesor" as fc

rectangle SATMI{

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
# Diagrama de casos de uso de alumnos
### El siguiente diagrama muestra como es que se relacionan los caso de uso de alumnos entre ellos y con los casos de uso de las tarjetas, también muestra la relación con el actor que será el profesor que esté utilizando el sistema.

![image](https://github.com/amezcua04s/FCA-Proyecto-OO-01/assets/147119596/5a9e2382-182d-4857-af4f-72a1efc9a4a0)


