# ID
- UC - 005 : Borrar alumno
   
## Actores
 * Profesor
    
## Tipo 
 * Secundario
   
## Interesados:
- El profesor desea dar de baja un alumno y los registros asociados a este dentro del sistema
  
## Breve descripción
El profesor podra dar de baja algún alumno que exista en el sistema y con ello todos los registros que se relacionen con este

## Pre condiciones
El profesor debe de tener registrado al menos a un alumno dentro del sistema

## Disparador
- El profesor ingresara a la opcion de "Eliminar alumno" 
- EL  caso de uso "UC - 004: Baja Grupo" llama a caso de uso

## Relaciones
- **Incluye**: UC - 006: Eliminar Tarjeta

## Flujo normal de eventos
1. El profesor ingresa al apartado de eliminar alumno
2. El profesor indica el alumno que desea eliminar
3. El sistema muestra los datos del alumno
4. El sistema pregunta si quiere continuar la operación
5. El sistema muestra el mensaje del resultado de la operación
   
## Subflujos
- S-1 En el paso 4 (Caso de aceptar)
  1. El profesor decide continuar con la operación
  2. El sistema utiliza el caso de uso UC-006: Eliminar Tarjeta
  3. Elimina todos los elementos que conformen al alumno en el sistema
  4. El caso de uso se reanuda en el paso 5 del flujo normal

- S-2 En el paso 4 (Caso de cancelar)
  1. El profesor decide cancelar la operación
  1. El sistema cancela la operación
  1. El caso de uso se reanuda en el paso 5 del flujo normal

## Alternativa / Flujos excepcionales
- Si el caso de uso es llamado por el caso de uso baja grupo
   1. El sistema selecciona a todos los alumnos del grupo
   2. El sistema elimina todos los registros asociados a los alumnos
   3. El caso de uso continua en el flujo del otro caso de uso
