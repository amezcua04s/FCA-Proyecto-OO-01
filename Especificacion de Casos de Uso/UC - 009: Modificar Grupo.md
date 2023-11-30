# ID
- UC - 009 : Modificar grupo
   
## Actores
 * Profesor
    
## Tipo 
 * Secundario
   
## Intereses:
- El profesor desea cambiar la información de un grupo 
  
## Breve descripción
El profesor cambiará algún dato o datos de algún grupo registrado en el sistema

## Pre condiciones
- El profesor debe tener en el sistema al menos un grupo registrado, para poder modificar la información de este

## Disparador
El profesor ingresará a la opcion de "Modificar grupo" en el grupo correspondiente

## Relaciones
- **Extiende**: Eliminar grupo

## Flujo normal de eventos
1. El profesor ingresa al apartado de modificar grupo en el grupo correspondiente
2. El profesor indica el cambio a realizar (Nombre/Horario)
3. El profesor ingresa los datos que se registrarán
4. El sistema verifica que la información nueva no coincida con ningún otro registro
5. El sistema actualiza la información del grupo
6. El sistema muestra mensaje del resultado de la operación

## Subflujos
- S-1 En el paso 4
1. La información que ingreso el profesor ya existe en otro registro
2. El sistema pregunta si desea en su lugar eliminar el grupo actual o no modificarlo
  - En caso de eliminarlo
    1. El caso de uso se extiende al caso de uso Eliminar Grupo
3. El caso de uso continua en el paso 6

## Alternativo / Flujos excepcionales
- Los datos que se desean cambiar mantienen en el mismo valor, por lo que el sistema arrojara un mensaje de error indicando la redundancia del cambio
