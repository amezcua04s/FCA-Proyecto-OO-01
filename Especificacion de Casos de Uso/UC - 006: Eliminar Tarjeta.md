# ID
- UC - 004 : Eliminar Tarjeta
   
## Actores
- UC - 005: Borrar Alumno
- UC - 007: Modificar Tarjeta
    
## Tipo 
- Secundario
   
## Intereses:
- El profesor eliminará todo el registro de un alumno o modificara el valor de la tarjeta "MI" 
  
## Breve descripción
- El sistema borrará de forma definitiva el valor de la tarjeta, como consecuencia del cambio de valor del registro o por baja real del alumno del sistema

## Disparador
- El profesor decide eliminar de forma total a un alumno
- El profesor modifica la información de la tarjeta del alumno

## Relaciones
- **Incluye**: UC - 013: Leer Tarjeta "MI"

## Flujo normal de eventos
1. El sistema llama al caso de uso
2. El sistema elimina el valor de la tarjeta seleccionada del sistema
3. El sistema continua en el caso de uso externo

