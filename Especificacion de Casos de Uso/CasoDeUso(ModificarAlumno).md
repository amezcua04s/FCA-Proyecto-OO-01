# ID
- UC - 000
  
# Caso de uso
 * Modificar alumno
   
## Actores
 * Profesor
    
## Tipo 
 * Secundario
   
## Stakeholders and Interests:
- El profesor desea registrar un nuevo alumno 
- El alumno podrá utilizar su tarjeda de MI para el registro de asistencia
  
## Bried Description
El profesor podra modificar un alumno que ya exista en el sistema, cambiando el nombre del alumno o la tarjeta MI asociada al alumno

## Trigger
El profesor ingresara a la opcion de "Modificar alumno"

## Relationships
- **Extends**: Modificar Tarjeta

## Normal Flow of Events
1. El profesor ingresa al apartado de modificar alumno
2. El profesor indica el alumno que desea modificar
3. El sistema muestra los datos del alumno
4. El sistema pide los datos que se modificaran
5. El sistema asigna el nombre y pregunta si se modificara el NFC
6. El sistema muestra los nuevos datos y pide que se confirme
7. El sistema muestra mensaje de éxito con los datos que se le asignaron

## Sub-Flows

S-1 En el paso 5
  1. El caso de uso le pasa el flujo al caso de uso de modificacion NFC
  2. El caso de uso continua en el paso 6

## Alternate / Exceptional Flows
