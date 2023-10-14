# ID
 - 000
# Caso de uso

 * Registrar un nuevo grupo
   
## Actores

 * Profesor
   
## Tipo 

 * Primario

## Partes interesadas:

- El profesor desea registrar un nuevo grupo 

## Pequeña descripción

El profesor podra dar de alta un nuevo grupo en el sistema, con la posibilidad de asignarle alumnos previemante registrados

## Provocador

El profesor ingresara a la opcion de "Registrar nuevo grupo"

### Tipo

Externo

## Relaciones

- **Asociacion**: Registro de Alumnos

## Flujo normal de eventos

1. El profesor ingresa al apartado de registro de grupo
2. El profesor indica el semestre al que pertenece el grupo
~~3. El profesor asigna alumnos previamente registrados en el sistema¿?~~
4. El sistema asigna el horario de la materia y nombre
5. El sistema verifica que el grupo no exista previamente en el mismo horario
6. Se guarda en el sistema la información
7. El sistema muestra mensaje de éxito con los datos del grupo

## Sub-flujo

S-1 
1. El grupo a asignar ya existe en el sistema
2. Se muestra mensaje de la correspondencia con el grupo ya existente
3. Se da la posibilidad de modificar el grupo
4. Se reanuda en el paso 6

## Excepciones
- El profesor no tiene horarios disponibles para registrar un nuevo grupo
- 
