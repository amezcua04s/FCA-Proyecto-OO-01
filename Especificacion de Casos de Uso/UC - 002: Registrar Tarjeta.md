# ID
- UC - 002
  
# Caso de uso
* Registrar Tarjeta "Mi"
   
## Actores
* Profesor
  
## Tipo 
* Escencial
   
## Partes interesadas e intereses:
- El profesor asignara la información de un alumno en la tarjeta de "MI" del propio alumno
  
## Breve descripcion
- Al momento de registrar un nuevo alumno el profesor le asignara su propio NFC desde la tarjeta "MI" del alumno
  
## Disparador
- Caso de uso registro de alumno

## Flujo normal de eventos
1. El caso de uso RegistrarAlumno extiende a este
2. El sistema solicita acercar el NFC para asociar los datos
3. El sistema verifica que no haya un registro previo de una tarjeta relacionada con un alumno
4. El sistema muestra mensaje de exito
5. El flujo continua en el paso correspondiente de caso de uso RegistrarAlumno

   
## Subflujos
- S-1 En el paso 3
    1. El NFC que se desea registrar esta asociado a otro alumno
    2. El sistema muestra la información del alumno que tiene asociado ese NFC
    3. El caso de uso termina

