# ID
- UC - 003: Registrar Tarjeta "MI"
   
## Actores
* Profesor
  
## Tipo 
* Escencial
   
## Partes interesadas e intereses:
- El profesor asignara la información de un alumno en la tarjeta de "MI" del propio alumno
  
## Breve descripción
- Al momento de registrar un nuevo alumno el profesor le asignara su propio NFC desde la tarjeta "MI" del alumno

## Pre condiciones
- El alumno debe de tener una tarjeta de "MI" propia
  
## Disparador
- Caso de uso "Registrar Alumno"

## Flujo normal de eventos
1. El caso de uso "Registrar Alumno "extiende a este
2. El sistema solicita acercar el NFC para asociar los datos
3. El sistema verifica que no exista la tarjeta en el sistema
4. El sistema muestra mensaje de éxito
5. El flujo continua en el paso correspondiente de caso de uso "Registrar Alumno"

   
## Subflujos
- S-1 En el paso 3 (En caso de que se encuentre la tarjeta registrada en el sistema)
    1. El sistema muestra el error en forma de "Pop-up"
    2. El sistema muestra la información del alumno que tiene asociado ese NFC
    3. El caso de uso termina