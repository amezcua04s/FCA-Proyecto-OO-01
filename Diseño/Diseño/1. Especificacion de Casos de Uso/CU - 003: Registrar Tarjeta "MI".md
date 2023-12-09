# ID
- CU - 003: Registrar Tarjeta "MI"
   
## Actores
* Profesor
  
## Tipo 
* Escencial
   
## Partes interesadas e intereses:
- El profesor asignará la información de un alumno en la tarjeta de "MI" del propio alumno
  
## Breve descripción
- Al momento de registrar un nuevo alumno el profesor le asignara su propio NFC desde la tarjeta "MI" del alumno

## Pre condiciones
- El alumno debe de tener una tarjeta de "MI" propia
  
## Disparador
- Caso de uso "CU - 002: Registrar Alumno"

## Flujo normal de eventos
1. El caso de uso "CU - 002: Registrar Alumno " extenderá a este.
2. El sistema solicitará acercar el NFC para asociar los datos.
3. El sistema verificará que no exista la tarjeta en el sistema.
4. El sistema mostrará mensaje de éxito en forma de "pop-up".
5. El flujo continua en el paso correspondiente de caso de uso "CU - 002: Registrar Alumno".

## Subflujos
- S-1 En el paso 3 (En caso de que se encuentre la tarjeta registrada en el sistema)
    1. El sistema mostrará el error en forma de "Pop-up"
    2. El sistema mostrará la información del alumno que tiene asociado ese NFC en forma de tabla.

    | Grupo | Nombre del alumno| Valor de la tarjeta|
    |:----:|:----:|:----:|
    |1391|Amezcua Arévalo Santiago|7C5CD480|
    > * Tomar tabla como referencia 

    3. El caso de uso termina