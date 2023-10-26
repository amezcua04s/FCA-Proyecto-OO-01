# ID
- 007
  
# Caso de uso
- Modificar Tarjeta
   
## Actores
- Profesor
    
## Tipo 
- Secundario
   
## Intereses:
- El profesor modificara la tarjeta que esta registrada a un alumno, transfiriendo todos los registros del alumno a la nueva tarjeta
 y borrando la tarjeta pasada, esto en caso de que el alumno lo solicite
  
## Breve Descripción
- El profesor cambiara el valor de la tarjeta que esta asociado a algún alumno

## Disparador
- El profesor selecciona "Modificar tarjeta"

## Relaciones
- **Inlcuye**: Borrar Tarjeta
- **Incluye**: Registrar Tarjeta

## Flujo normal de eventos
1. El profesor selecciona el alumno al cual se le modificara la tarjeta MI
2. El sistema pregunta si se desea continuar con la operación
3. El sistema solicita leer la nueva tarjeta MI
4. El sistema compara si esta tarjeta no existe en el sistema
5. El sistema regresa un mensaje del resultado de la operación
   
## Subflujos

- S-1 En el paso 4
    1. Si se encuentra la tarjeta 
    2. El sistema mostrara el error
    3. El flujo se reanuda en el paso 5 del flujo normal

- S-1 En el paso 4
    1. El sistema no encuentra la tarjeta
    2. El sistema extiende al caso de uso de borrar tarjeta
    3. El sistema extiende al caso de uso de registrar tarjeta
    4. El flujo se reanuda en el paso 5 del flujo normal
