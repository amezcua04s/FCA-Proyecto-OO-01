# ID: 
- UC - 004: Baja grupo
   
## Actores
- Profesor
    
## Tipo
- Secundario

## Relaciones
- **Incluye**: UC - 005: Eliminar Alumno

## Partes interesadas e intereses:
- El profesor eliminara de forma definitiva todos los datos de un grupo
  
## Breve descripción
- El profesor elimina todos los registros que esten asociados a un grupo, así como la información de los alumnos que esten asociados al grupo

## Pre condiciones
- El profesor debe de tener al menos un grupo registrado dentro del sistema

## Flujo de eventos
1. El profesor entra al apartado de eliminar grupo
2. El profesor ingresa el número del grupo y el sistema le muestra la información del mismo
3. El sistema pregunta si desea continuar con la operacion
4. El sistema continua en el caso de uso "UC - 005: Eliminar Alumno" y elimina de forma individual a  cada alumno asociado al grupo
5. El sistema elimina todos los informes que encuentre del grupo seleccionado
6. El sistema muestra mensaje del resultado de la operación en forma de "Pop-up"

## Sub-flujo       
* S-2 En el paso 4 (En caso de rechazar la realización)
    1. El profesor cancela la operación
    2. El flujo continua en el paso 4

## Excepciones
- El profesor ingresa un número de grupo incorrecto, por lo que el sistema no lleva a cabo ninguna operación
