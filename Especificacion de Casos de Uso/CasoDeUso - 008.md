# ID
- 008
  
# Caso de uso
 * Modificar alumno
   
## Actores
 * Profesor
    
## Tipo 
 * Secundario
   
## Partes interesadas e intereses:
- El profesor desea registrar un nuevo alumno 
- El alumno podrá utilizar una nueva tarjeta de MI para el registro de asistencia
  
## Breve descripcion
El profesor podra modificar un alumno que ya exista en el sistema, cambiando el nombre del alumno o la tarjeta MI asociada al alumno

## Disparador
El profesor ingresara a la opcion de "Modificar alumno"

## Relaciones
- **Extiende**: Modificar Tarjeta

## Flujo normal de eventos
1. El profesor ingresa al apartado de modificar alumno
2. El profesor indica el alumno que desea modificar
3. El sistema muestra los datos del alumno
4. El sistema pregunta que se modificara (Nombre o tarjeta)
5. El sistema pide al profesor el nuevo nombre
6. El sistema verifica que el nombre no exista en el sistema
7. El sistema muestra los nuevos datos y pide que se confirme
8. El sistema muestra mensaje del resultado de la operacion


## Subflujos

S-1 En el paso 4 (En caso de querer modificar la tarjeta del alumno)
  1. Si el profesor selecciona que se modificara la tarjeta se extiende el caso de uso a "ModificarTarjeta"
  2. El caso de uso reanuda el flujo en el paso 7

S-2 En el paso 6 (En caso de ya encontrar el nombre en el sistema)
  1. El sistema hacer saber al profesor este error
  2. El sistema cancela la operación y continua el flujo en el paso 8
