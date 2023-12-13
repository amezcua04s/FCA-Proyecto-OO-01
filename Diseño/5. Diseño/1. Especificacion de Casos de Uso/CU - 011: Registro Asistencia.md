# ID 
- CU - 011 : Registro Asistencia
  
## Actores
- Profesor

## Tipo
- Secundario

## Partes interesadas e intereses
- El profesor llevará un control de las asistencias de sus alumnos.

## Breve descripción 
- El profesor registrará la asistencia de los alumnos del grupo seleccionado.

## Disparador
- El profesor seleccionará el apartado de "Tomar Asistencia" del grupo correspondiente.

## Flujo normal de eventos
1. El profesor seleccionará "Tomar Asistencia" en el grupo corresponiente.
2. El sistema mostrará que está esperando a leer tarjeta
3. El profesor acercará la tarjeta de cada alumno
4. Por cada vez que se lea la tarjeta, el sistema hará un sonido que indique que se leyó, y mostrará la información del alumno que se cerrará de forma automática 3 segundos después.
5. El sistema cerrará el modulo de pase de asistencia 20 minutos (1,200 segundos) después de ser iniciada.
6. El sistema informará que el periodo terminó.

## Sub-flujo  
S-1 En el paso 3 (En caso de querer leer por segunda ocasión una tarjeta que ya leyo en esta sesión)
1. El sistema mostrará el error.
1. El caso de uso continua en el flujo 6
