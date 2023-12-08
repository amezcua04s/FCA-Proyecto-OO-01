# ID
- UC - 008 : Modificar alumno
   
## Actores
 * Profesor
    
## Tipo 
 * Secundario

## Relaciones
**Extiende:** UC - 007: Modificar Tarjeta

## Partes interesadas e intereses:
- El alumno desea modificar un dato erroneo en el sistema 
- El profesor podrá llevar control preciso de la información
  
## Breve descripcion
- El profesor podrá modificar un alumno que ya exista en el sistema, cambiando el nombre del alumno o el id de la tarjeta "MI" asociada al alumno

## Pre condiciones
- El alumno el cuál desea modificar un dato, debe de estar previamente registrado en el sistema

## Disparador
El profesor ingresará a la opcion de "Modificar alumno"

## Flujo normal de eventos
1. El profesor ingresa al apartado de modificar alumno
2. El profesor indica el alumno que desea modificar
3. El sistema muestra los datos del alumno en formato de tabla

| Grupo | Nombre del alumno| Valor de la tarjeta|
|:----:|:----:|:----:|
|1391|Amezcua Arevalo Sntigo|4F3CD120|

4. El sistema avisa que en caso de que algún campo de la modificación se deje vacío, no se modificará ese campo
5. El sistema solicita el dato del alumno que se modificará (Nombre o tarjeta o grupo)
 - En caso de modificar tarjeta
    1. El sistema extiende al caso de uso "UC -007: Modificar Tarjeta"
6. El sistema muestra los nuevos datos en formato de tabla y pide que se confirme

| Grupo | Nombre del alumno| Valor de la tarjeta|
|:----:|:----:|:----:|
|1391|Amezcua Arévalo Santiago|7C5CD480|

7. El sistema muestra mensaje del resultado de la operación