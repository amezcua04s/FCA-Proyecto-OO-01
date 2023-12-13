# ID
- CU - 004 : Eliminar Tarjeta "MI"
   
## Actores
- CU - 005: Borrar Alumno
- CU - 007: Modificar Tarjeta "MI"
    
## Tipo 
- Secundario
   
## Intereses:
- El sistema eliminará de forma total a un alumno.
- El profesor modifica la información de la tarjeta del alumno.
  
## Breve descripción
- El sistema borrará de forma definitiva el valor de la tarjeta, como consecuencia del cambio de valor del registro o por baja real del alumno del sistema.

## Pre condiciones
- El alumno al cual se le eliminará la tarjeta debe de estar previamente registrado en el sistema.

## Disparador
- UC - 005: Borrar Alumno
- UC - 007: Modificar Tarjeta "MI"

## Flujo normal de eventos
1. El caso de uso externo llamará al caso de uso.
2. El sistema eliminará los registros asociados a esta tarjeta.
3. El sistema eliminará el valor de la tarjeta seleccionada del sistema.
4. El sistema continuará en el caso de uso externo.
