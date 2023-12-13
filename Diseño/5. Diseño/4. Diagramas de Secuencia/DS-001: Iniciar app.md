# Diagrama de secuencia DS - 001: Iniciar App
- El diagrama representa como es que se inicializa la aplicación y los módulos necesarios para el funcionamiento de la aplicación [SATMI](/Diseño/1.%20Propósito/Propósito.md), representa de forma simbólica los módulos involucrados y como se comunican entre sí para realizar la operación.

![DS  001 iniciarApp](https://github.com/amezcua04s/FCA-Proyecto-OO-01/assets/119078847/dd979541-8e9d-4dd1-86fc-a2ab5d5e1a0e)

<!-- @startuml 

title DS - 001: Iniciar App

Orchestator -> Initializer: Iniciar app 
Initializer -> CapaAPI: Inicializar modulos
CapaAPI-->  
<!--Initializer: returnStatus
alt Modulos API iniciados
CapaAPI -> CapaDAO: Inicializar modulos
CapaDAO --> 
<!--CapaAPI : returnStatus()
alt Modulos DAO iniciados
CapaDAO -> SQLite: Inicializar
SQLite --> 
<!--CapaDAO: returnStatus()
alt SQLite inicializada
CapaDAO --> 
<!--CapaAPI: returnStatus()
CapaAPI -->
<!-- Initializer: ExcecuteSATMI()
Initializer --> 
<!--Orchestator: Iniciar app
else SQLite no inicializado
SQLite -->
<!-- Initializer: returnError()
end
else Modulos DAO no iniciados
CapaDAO -->
<!-- Initializer: returnError()
end
else Modulos API no iniciados
Initializer -->
<!-- Orchestator: returnError()
end
@enduml