# ID
- UC - 000
  
# Caso de uso
- Eliminar Tarjeta
   
## Actores
- Profesor
    
## Tipo 
- Terciario
   
## Stakeholders and Interests:
- El profesor eliminara todo el registro de un alumno o modificara el valor de la tarjeta
  
## Bried Description
- El sistema borrara de forma definitiva el valor de la tarjeta, por consecuencia del cambio de valor de esta o por baja real del alumno del sistema

## Trigger
- El profesor decide eliminar de forma real un alumno
- El profesor modifica la información de la tarjeta del alumno

## Relationships
- **Includes**: ModificarTarjeta
- **Includes**: EliminarAlumno

## Normal Flow of Events
1. El sistema llama al caso de uso
2. El sistema elimina el valor de la tarjeta seleccionada del sistema
3. El sistema continua en el caso de uso externo
   
## Sub-Flows

## Alternate / Exceptional Flows
