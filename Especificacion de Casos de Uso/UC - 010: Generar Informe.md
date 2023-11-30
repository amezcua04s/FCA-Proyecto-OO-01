# ID
 - UC - 010 : Generar Informe
   
## Actores
 * Profesor
   
## Tipo 
 * Secundario

## Partes interesadas e intereses:
- El profesor desea obtener informes de un periodo de tiempo del grupo seleccionado

## Breve descripción
El profesor podrá obtener informes de asistencia de uno de sus grupos de un cierto periodo de tiempo

## Pre condiciones
- El profesor debe de tener al menos un grupo registrado en el sistema, y el registro de un día de asistencia de ese grupo

## Disparador
El profesor ingresará a la opcion de "Informes"

## Relaciones
- **Extiende**: UC - 011: Exportar Informe

## Flujo normal de eventos
1. El profesor ingresa al apartado de Informes 
2. El sistema le pide al profesor especificar el periodo del que desea los informes y el grupo
3. El Sistema verfica que el periodo y el grupo sean válidos 
4. El profesor ingresara la opcion "Continuar" 
5. El sistema muestra el informe con toda la informacion en el periodo solicitado por el profesor 

## Sub-flujo
S-2 En el paso 3 (El sistema no válida el periodo que el profesor selecciono)
 1. El sistema mostrara un mensaje de error
 2. El sistema mostrara al profesor un mensaje para que vuelva a indicar el periodo
 3. El flujo del caso de uso continua el flujo normal en el paso 3
 
S-1 En el paso 3 (El sistema no válida el grupo que el profesor ingreso)
 1. El sistema muestra un mensaje de error
 2. El sistema muestra los grupos que tiene registrados
 3. El sistema pide que ingrese uno de los grupos
 4. El flujo del caso de uso continua el flujo normal en el paso 3

## Excepciones
El profesor selecciona un periodo de tiempo válido, pero no tiene registros en el periodo de tiempo especificado, el sistema mosrara el error, "falta de información" 
  
