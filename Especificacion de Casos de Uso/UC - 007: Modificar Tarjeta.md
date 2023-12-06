# ID
- UC - 007 : Modificar Tarjeta
   
## Actores
- UC - 008: Modificar Alumno
    
## Tipo 
- Secundario
   
## Intereses:
- El profesor modificará la tarjeta que esta registrada a un alumno
- El alumno desea cambiar la tarjeta en la que están asociados sus datos
  
## Breve Descripción
- El sistema cambiará el valor de la tarjeta que esta asociado a algún alumno, transfiriendo todos los registros del alumno a la nueva tarjeta y borrando la tarjeta pasada del almacenamiento

## Pre condiciones
- El alumno al que se le desea modificar la tarjeta debe de existir registrado previamente en el sistema

## Disparador
- El profesor selecciona "Modificar tarjeta" en el apartado de modificar alumno

## Relaciones
- **Inlcuye**: UC - 006: Eliminar Tarjeta
- **Incluye**: UC - 003: Registrar Tarjeta "MI"

## Flujo normal de eventos
1. El caso de uso "UC - 008: Modificar Alumno" extiende a este
2. El sistema muestra los datos y pregunta si se desea continuar con la operación
3. El sistema solicita leer la nueva tarjeta "MI"
4. El sistema compara si esta tarjeta no existe en el sistema
5. El sistema extiende al caso de uso "UC - 006: Eliminar Tarjeta"
6. El sistema extiende al caso de uso "UC - 003: Registrar Tarjeta "MI""
7. El sistema muestra un "pop-up" con la nueva tarjeta asociada
8. El sistema regresa un mensaje del resultado de la operación
   
## Subflujos

- S-1 En el paso 4 (En caso de que se encuentre la tarjeta registrada en el sistema)
    1. El sistema mostrara el error
    1. El sistema muestra la información del alumno que tiene registrada esta tarjeta
    1. El flujo se reanuda en el paso 5 del flujo normal