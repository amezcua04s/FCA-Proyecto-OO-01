# ID
- UC - 000
  
# Caso de uso
* Registrar Tarjeta
   
## Actores
* Profesor
* Alumno
  
## Tipo 
* Escencial
   
## Stakeholders and Interests:
- El profesor asignara la información de un alumno en la tarjeta de MI del propio alumno
  
## Bried Description
- Al momento de registrar un nuevo alumno el profesor le asignara su propio NFC desde la tarjeta MI del alumno
  
## Trigger
- Caso de uso registro de alumno

## Relationships
- **Extends**: Caso de uso RegistrarAlumno

## Normal Flow of Events
1. El caso de uso RegistrarAlumno extiende a este
2. El sistema pide acercar el NFC para asociar los datos
3. El sistema muestra mensaje de exito
4. El flujo continua en el paso correspondiente de caso de uso RegistrarAlumno

   
## Sub-Flows
- S-1 En el paso 2
    1. El NFC que se desea registrar esta asociado a otro alumno
    2. El sistema muestra la información del alumno que tiene asociado ese NFC
    3. El caso de uso termina

## Alternate / Exceptional Flows
