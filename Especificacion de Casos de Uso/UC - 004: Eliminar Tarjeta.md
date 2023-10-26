# ID
- UC - 004
  
# Caso de uso
- Eliminar Tarjeta
   
## Actores
- UC - 005
- UC - 007
    
## Tipo 
- Terciario
   
## Intereses:
- El profesor eliminara todo el registro de un alumno o modificara el valor de la tarjeta
  
## Breve descripción
- El sistema borrara de forma definitiva el valor de la tarjeta, por consecuencia del cambio de valor de esta o por baja real del alumno del sistema

## Disparador
- El profesor decide eliminar de forma total a un alumno
- El profesor modifica la información de la tarjeta del alumno

## Relaciones
- **Incluye**: ModificarTarjeta
- **Extiende**: EliminarAlumno

## Flujo normal de eventos
1. El sistema llama al caso de uso
2. El sistema elimina el valor de la tarjeta seleccionada del sistema
3. El sistema continua en el caso de uso externo

