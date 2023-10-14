# ID
- UC - 000
  
# Caso de uso
 * Registrar alumno
   
## Actores
 * Profesor
    
## Tipo 
 * Primario
   
## Stakeholders and Interests:
- El profesor desea registrar un nuevo alumno 
- El alumno podrá utilizar su tarjeda de MI para el registro de asistencia
  
## Bried Description
El profesor podra dar de alta un nuevo alumno en el sistema, asignandole un grupo y enlazando el registro del alumno en la tarjeta de MI (movilidad integrada)

## Trigger
El profesor ingresara a la opcion de "Registrar nuevo alumno"

### Type
Externo

## Relationships
- **Asociacion**: Registro de Tarjetas

## Normal Flow of Events
1. El profesor ingresa al apartado de registro de alumno
2. El profesor indica el grupo en el que desea ser registrado
3. El profesor ingresa los datos del alumno
4. El sistema asigna la informacion del alumno al identificador NFC que lea
5. El sistema verifica que el identificador NFC no este registrado para otro alumno
6. Se da de alta el NFC con los datos asignados
7. El sistema muestra mensaje de éxito con los datos que se le asignaron

## Sub-Flows

S-1 

## Alternate / Exceptional Flows
