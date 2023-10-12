# Caso de uso

 * UC - 001: Registrar un nuevo grupo
   
## Actores

 * Profesor
   
## Tipo 

 * Primario

## Stakeholders and Interests:

- El profesor desea registrar un nuevo grupo 

## Bried Description

El profesor podra dar de alta un nuevo grupo en el sistema, con la posibilidad de asignarle alumnos previemante registrados

## Trigger

El profesor ingresara a la opcion de "Registrar nuevo grupo"

### Type

Externo

## Relationships

- **Asociacion**: Registro de Alumnos

## Normal Flow of Events

1. El profesor ingresa al apartado de registro de grupo
2. El profesor indica el semestre al que pertenece el grupo
~~3. El profesor asigna alumnos previamente registrados en el sistema¿?~~
4. El sistema asigna el horario de la materia y nombre
5. El sistema verifica que el grupo no exista previamente en el mismo horario
6. Se da de alta el grupo
7. El sistema muestra mensaje de éxito con los datos del grupo

## Sub-Flows

S-1 

## Alternate / Exceptional Flows
