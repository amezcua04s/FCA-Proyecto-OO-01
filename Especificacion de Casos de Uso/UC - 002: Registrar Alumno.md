# ID
- UC - 003
  
# Caso de uso
 * Registrar alumno
   
## Actores
 * Profesor
    
## Tipo 
 * Primario
   
## Partes interesadas e intereses:
- El profesor desea registrar un nuevo alumno 
- El alumno podrá utilizar su tarjeda de "MI" para el registro de asistencia
  
## Breve descripcion
- El profesor podrá dar de alta un nuevo alumno en el sistema, asignandole un grupo y materia, además de asignarle un número de identificador único, según el NFC de la tarjeta de "MI" del Alumno

## Pre condiciones
- El alumno debe de tener una tarjeta de "MI" (Movilidad Integrada) propia

## Disparador
- El profesor ingresara a la opción de "Registrar nuevo alumno"

## Relaciones
- **Inclusión**: UC - 003: Registro Tarjeta "MI"

## Flujo normal de eventos
1. El profesor selecciona el grupo al que registrara el alumno
2. El profesor ingresa al apartado de registro de alumno
3. El profesor ingresa el nombre, número de cuenta y NFC de la tarjeta de "MI" (Movilidad Integrada) del alumno que se desea agregar
4. El sistema verifica que no exista un registro previo del alumno que se desea agregar
5. El flujo continua en el caso de uso Registro Tarjeta
6. Se da de alta el NFC con los datos asignados
7. El sistema muestra mensaje de éxito con los datos que se le asignaron

## Subflujos
- S-1 En el paso 4 (En caso de que el sistema encuentre un registro de ese mismo alumno)
  1. El sistema muestra en pantalla los datos del alumno
  2. El sistema pregunta si desea modificar la información del alumno
  3. El flujo continua en el caso de uso Modificar Alumno