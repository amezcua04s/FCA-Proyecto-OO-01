# ID
- UC - 000
  
# Caso de uso
 * Borrar alumno
   
## Actores
 * Profesor
    
## Tipo 
 * Secundario
   
## Stakeholders and Interests:
- El profesor desea dar de baja un alumno
  
## Bried Description
El profesor podra dar de baja algun alumno que exista en el sistema o quitandolo del grupo (baja parcial), 
eliminando todos los elementos que esten asociados con el alumno (nombre y tarjeta MI) esto en caso de baja real

## Trigger
El profesor ingresara a la opcion de "Eliminar alumno"

## Relationships
- **Generalización**: Modificar Alumno

## Normal Flow of Events
1. El profesor ingresa al apartado de eliminar alumno
2. El profesor indica el alumno que desea eliminar
3. El sistema muestra los datos de los alumnos
4. El sistema pregunta que tipo de baja sera (parcial o real)
5. El sistema pregunta si quiere continuar la operacion
6. El sistema muestra el mensaje del resultado de la operación
   
## Sub-Flows
- S-1 En el paso 4
  1. El profesor decide baja parcial del alumno
  1. Se muestran los datos del alumno y se pregunta si desea continuar
  1. El sistema simplemente eliminara la asociacion del alumno con el grupo (Sin borrar la información del alumno del sistema)
  1. El caso de uso se reanuda en el paso 6 del flujo normal
  
- S-2 En el paso 5
  1. El profesor decide cancelar la operación
  1. El sistema cancela la operación
  1. El caso de uso se reanuda en el paso 6 del flujo normal

## Alternate / Exceptional Flows
