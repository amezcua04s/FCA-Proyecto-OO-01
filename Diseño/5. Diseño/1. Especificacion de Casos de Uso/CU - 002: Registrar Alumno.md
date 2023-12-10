# ID
- CU - 002: Registrar alumno
   
## Actores
 * Profesor
    
## Tipo 
 * Primario
   
## Partes interesadas e intereses:
- El profesor desea registrar un nuevo alumno.
- El alumno podrá utilizar su tarjeta de "MI" para el registro de asistencia.
  
## Breve descripción
- El profesor podrá dar de alta un nuevo alumno en el sistema, asignandole un grupo y materia, además de asignarle un número de identificador único, según el NFC de la tarjeta de "MI" del Alumno.

## Pre condiciones
- El alumno debe de tener una tarjeta de "MI" (Movilidad Integrada) propia.

## Disparador
- El profesor ingresará a la opción de "Registrar nuevo alumno".

## Relaciones
- **Inclusión**: CU - 003: Registro Tarjeta "MI"

## Flujo normal de eventos
1. El profesor seleccionará el grupo al que registrará el alumno.
2. El profesor ingresará al apartado de "Registrar nuevo alumno".
3. El profesor ingresará el nombre del alumno.
4. El sistema extiende al caso de uso "CU - 003: Registro Tarjeta "MI"".
5. El sistema verificará que no exista un registro previo del alumno que se desea agregar.
6. Se dará de alta el NFC con los datos asignados.
7. El sistema mostrará un mensaje del resultado de la operación.

## Subflujos
- S-1 En el paso 5 (En caso de que el sistema encuentre un registro de ese mismo alumno)
  1. El sistema mostrará en pantalla el error y los datos del alumno ya registrado en forma de tabla. 

  | Grupo | Nombre del alumno| Valor de la tarjeta|
  |:----:|:----:|:----:|
  |1391|Amezcua Arévalo Santiago|7C5CD480|
  > * Tomar tabla como referencia.

  3. El flujo continua en el paso 7.
