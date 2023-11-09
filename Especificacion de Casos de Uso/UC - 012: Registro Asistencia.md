# ID 
- UC - 012

## Caso de Uso
- Registro Asistencia
  
## Actores
- Profesor

## Tipo
- Secundario

## Partes interesadas e intereses
- El profesor desea llevar un control de los

## Breve descripción 
El profesor registrara la asistencia de los alumnos del grupo en la hora indicada

## Disparador
El profesor ingresa al apartado de pase de asistencia del grupo correspondiente a la hora

## Flujo normal de eventos
1. El profesor ingresa a la aplicación
2. El profesor selecciona pasar asistencia
3. El sistema informa que esta esperando a leer tarjeta
4. El profesor lee la tarjeta de todos los alumnos
5. El sistema cierra el modulo de pase de asistencia 20 minutos (1,200 segundos) despues de ser iniciada
6. El sistema informa que el periodo termino

## Sub-flujo  
S-1 En el paso 2 ( Cuando ya haya realizado la operación anteriormente en ese modulo)
1. El sistema avisa que aquellas asistencias que se leeran serán "retardos"
1. El profesor lee las tarjetas de los alumnos que deseen
1. El caso de uso continua en el flujo 5
   
S-2 En el paso 4 (Cuando se disponga a leer por segunda vez la tarjeta del mismo alumno)
1. El sistema mostrara el error
1. El caso de uso continua en el flujo 4

## Excepciones
Si el profesor no tiene un grupo registrado en la hora que desea pasar asistencia, el sistema le dara la posibilidad de registrar un nuevo grupo, y en caso de ser así se extiende al caso de uso UC-001

  
