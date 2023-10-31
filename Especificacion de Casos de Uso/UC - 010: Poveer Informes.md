# ID
 - UC - 010
   
# Caso de uso
 * Proveer Informes
   
## Actores
 * Profesor
   
## Tipo 
 * Primario

## Partes interesadas e intereses:
- El profesor desea obtener informes de un periodo de tiempo

## Breve descripción
El profesor podra obtener informes de asistencia de sus alumnos de un cierto periodo de tiempo

## Disparador
El profesor ingresara a la opcion de "Informes"

## Flujo normal de eventos
1. El profesor ingresa al apartado de Informes
2. El sistema le pide al profesor especificar el periodo del que desea los informes
3. El Sistema verfica que el periodo sea válido 
4. El profesor ingresara la opcion "Continuar" 
5. El sistema muestra el informe con toda la informacion en el periodo solicitado por el profesor 

## Sub-flujo
S-1 En el paso 3 (El sistema no valida el periodo que el profesor selecciono)
 1. El sistema mostrara un mensaje de error
 2. El sistema mostrara al profesor un mensaje para que vuelva a indicar el periodo
 3. El flujo del caso de uso continua el flujo normal en el paso 4

## Excepciones
PREGUNTAR
  
