# ID
 - UC - 001
   
# Caso de uso
 * Registrar grupo
   
## Actores
 * Profesor
   
## Tipo 
 * Primario

## Partes interesadas e intereses:
- El profesor desea registrar un nuevo grupo 

## Breve descripción
El profesor podra dar de alta un nuevo grupo en el sistema, con la posibilidad de asignarle alumnos previemante registrados

## Disparador
El profesor ingresara a la opcion de "Registrar nuevo grupo"

## Flujo normal de eventos
1. El profesor ingresa al apartado de registro de grupo
2. El profesor ingresa el nombre de la materia
3. El profesor ingresa el número de grupo
4. El profesor indica el semestre al que pertenece el grupo
5. El profesor indica el horario de la materia
6. El sistema verifica que no exista otro registro con ese número de grupo
7. El sistema verifica que no exista otro grupo que ya utilice ese horario
8. Se guarda en el sistema la información
9. Se muestran los datos del grupo
10. El sistema muestra mensaje del resultado de la operación

## Sub-flujo
S-1 En el paso 6 (En caso de que se encuentre otro registro)
 1. El sistema señala el error y muestra la información del otro grupo ya existente
 1. El sistema pregunta si desea modificar el número del grupo
   - En caso de que si
     1. El flujo del caso de uso continua el flujo normal en el paso 3
   - De lo contrario
     1. El flujo del caso de uso continua el flujo normal en el paso 10

S-2 En el paso 7 (En caso de no disponibilidad de horario)
 1. Se muestra mensaje de error y se muestra la información del grupo ya existente
 1. El sistema recomienda los horarios disponibles del profesor para el registro del nuevo grupo
 1. Se da la posibilidad de modificar el horario del grupo
 1. Se reanuda en el paso 5

## Excepciones
- El profesor no tiene horarios disponibles para registrar un nuevo grupo 
  
