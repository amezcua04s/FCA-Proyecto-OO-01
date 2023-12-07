# ID
 - UC - 001: Registrar grupo
   
## Actores
 * Profesor
   
## Tipo 
 * Primario

## Partes interesadas e intereses:
- El profesor desea registrar un nuevo grupo 

## Breve descripción
El profesor podrá dar de alta un nuevo grupo en el sistema, con la posibilidad de asignarle alumnos previemante registrados, así como asignarle un horario al grupo

## Disparador
El profesor ingresará a la opcion de "Registrar nuevo grupo"

## Flujo normal de eventos
1. El profesor ingresa al apartado de registro de grupo
2. El profesor ingresa el nombre de la materia
3. El profesor ingresa el número de grupo
4. El profesor ingresa el semestre al que pertenece el grupo
5. El sistema verifica que no exista otro registro con ese número de grupo
6. Se guarda en el sistema la información
7. Se muestran los datos(Nombre de la materia, número de grupo, semestre al que pertenece) del grupo
8. El sistema muestra mensaje del resultado de la operación

## Sub-flujo
S-1 En el paso 5 (En caso de que se encuentre otro registro)
 1. El sistema señala el error y muestra la información del otro grupo ya existente
 1. El sistema pregunta si desea modificar el número del grupo
   - En caso de que si
     1. El flujo del caso de uso continua el flujo normal en el paso 3
   - De lo contrario
     1. El flujo del caso de uso continua el flujo normal en el paso 10

## Excepciones
- El profesor deja algún campo vacio, por lo que el registro no se lleva a cabo
  
