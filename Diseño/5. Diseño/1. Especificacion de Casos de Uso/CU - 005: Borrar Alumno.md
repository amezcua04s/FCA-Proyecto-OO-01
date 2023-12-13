# ID
- CU - 005 : Borrar alumno
   
## Actores
 * Profesor
    
## Tipo 
 * Secundario
   
## Interesados e intereses:
- El profesor desea dar de baja un alumno y los registros asociados a este dentro del sistema a causa de baja de grupo.
  
## Breve descripción
- El sistema eliminará a un alumno y todos los registros que estén asociados al alumno a causa de baja de grupo.

## Pre condiciones
- El profesor debe de tener registrado al menos a un alumno dentro del sistema.

## Disparador
- El caso de uso "CU - 004: Baja Grupo" llama a caso de uso.

## Relaciones
- **Incluye**: CU - 006: Eliminar Tarjeta "MI"

## Flujo normal de eventos
1. El caso de uso "CU-004: Baja Grupo" se extenderá a este caso de uso.
2. El sistema seleccionará a todos los alumnos del grupo.
3. El sistema eliminará todos los registros asociados a los alumnos.
4. El sistema mostrará el mensaje del resultado de la operación.
5. El caso de uso continuará en el flujo del otro caso de uso.
