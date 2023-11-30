# ID
- UC - 008 : Modificar alumno
   
## Actores
 * Profesor
    
## Tipo 
 * Secundario
   
## Partes interesadas e intereses:
- El alumno desea modificar un dato erroneo en el sistema 
- El profesor podrá llevar control preciso de la información
  
## Breve descripcion
El profesor podrá modificar un alumno que ya exista en el sistema, cambiando el nombre del alumno o el id de la tarjeta "MI" asociada al alumno

## Disparador
El profesor ingresará a la opcion de "Modificar alumno"

## Relaciones
- **Extiende**: Modificar Tarjeta

## Flujo normal de eventos
1. El profesor ingresa al apartado de modificar alumno
2. El profesor indica el alumno que desea modificar
3. El sistema muestra los datos del alumno
4. El sistema pregunta que dato del alumno se modificara (Nombre o correo o tarjeta)
5. El sistema muestra los nuevos datos y pide que se confirme
6. El sistema muestra mensaje del resultado de la operacion


## Subflujos

S-1 En el paso 4 (En caso de querer modificar la tarjeta del alumno)
  1. Si el profesor selecciona que se modificará la tarjeta se extiende el caso de uso a "ModificarTarjeta"
  2. El caso de uso reanuda el flujo en el paso 6

S-2 En el paso 4 (En caso de querer modificar el nombre)
  1. El sistema muestra el nombre actual del alumno
  1. El sistema solicita el nuevo nombre del alumno
  1. El caso de uso reanuda el flujo en el paso 5

S-3 En el paso 4 (En caso de querer modificar el correo del alumno)
  1. El sistema busca que el correo no exista ya registrado en otro alumno
     - En caso de encontrarse
       1. El sistema muestra el error y continua el flujo en el paso 6
  2. El sistema solicita el nuevo correo del alumno
  3. El caso de uso reanuda el flujo en el paso 5
      
