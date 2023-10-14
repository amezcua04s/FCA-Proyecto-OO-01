# ID
- UC - 000
  
# Caso de uso
- Modificar Tarjeta
   
## Actores
- Profesor
    
## Tipo 
- Secundario
   
## Stakeholders and Interests:
- El profesor modificara la tarjeta que esta registrada a un alumno, transfiriendo todos los registros del alumno a la nueva tarjeta
 y borrando la tarjeta pasada, esto en caso de que el alumno lo solicite
  
## Bried Description
- El profesor cambiara el valor de la tarjeta que esta asociado a algún alumno

## Trigger
- El profesor selecciona "Modificar tarjeta"

## Relationships
- **Extends**: Borrar Tarjeta
- **Exends**: Registrar Tarjeta

## Normal Flow of Events
1. El profesor selecciona el alumno al cual se le modificara la tarjeta MI
2. El profesor acerca la nueva tarjeta para que el sistema la asocie al alumno
3. El sistema compara si esta tarjeta no existe en el sistema
4. El sistema registra la nueva tarjeta a la información del alumno
5. El sistema borra la tarjeta previamente registrada para el alumno
6. El sistema regresa un mensaje del resultado de la operación
   
## Sub-Flows
- S-1 En el paso 3
    1. Si se encuentra la tarjeta 
    2. El sistema mostrara el error
    3. El flujo del sistema se reanuca en el paso 6 del flujo normal

## Alternate / Exceptional Flows
