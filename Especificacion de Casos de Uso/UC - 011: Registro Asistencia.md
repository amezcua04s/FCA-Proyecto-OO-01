# ID 
- UC - 011 : Registro Asistencia
  
## Actores
- Profesor

## Tipo
- Secundario

## Partes interesadas e intereses
- El profesor desea llevar un control de las asistencias de sus alumnos 

## Breve descripción 
El profesor registrará la asistencia de los alumnos del grupo en la hora indicada

## Disparador
El profesor ingresa al apartado de pase de asistencia del grupo correspondiente a la hora

## Flujo normal de eventos
1. El profesor selecciona pasar asistencia
2. El sistema informa que esta esperando a leer tarjeta
3. El profesor lee la tarjeta de cada alumno
4. Por cada vez que se lea la tarjeta, el sistema hará un sonido que indique que se leyo, y mostrara la información del alumno que se cerrara de forma automática 5 segundos después
5. El sistema cierra el modulo de pase de asistencia 20 minutos (1,200 segundos) despues de ser iniciada
6. El sistema informa que el periodo termino

## Sub-flujo  
S-1 En el paso 3 (En caso de querer leer por segunda ocasión una tarjeta que ya leyo en esta sesión)
1. El sistema mostrará el error
1. El caso de uso continua en el flujo 3