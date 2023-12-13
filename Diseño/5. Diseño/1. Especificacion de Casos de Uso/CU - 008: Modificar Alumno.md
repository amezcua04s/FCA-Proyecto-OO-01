# ID
- CU - 008 : Modificar alumno
   
## Actores
 * Profesor
    
## Tipo 
 * Secundario

## Relaciones
**Extiende:** CU - 007: Modificar Tarjeta

## Partes interesadas e intereses:
- El alumno desea modificar un dato erroneo en el sistema.
- El profesor podrá llevar control preciso de la información.
  
## Breve descripción
- El profesor podrá modificar un alumno que ya exista en el sistema, cambiando el nombre del alumno o el id de la tarjeta "MI" asociada al alumno.

## Pre condiciones
- El alumno el cuál desea modificar un dato, debe de estar previamente registrado en el sistema.

## Disparador
- El profesor seleccionará a la opcion de "Modificar alumno" dentro del grupo al que pertenece.

## Flujo normal de eventos
1. El profesor ingresará al apartado "Moificar Alumno".
2. El profesor seleccionará el alumno que desea modificar.
3. El sistema mostrará los datos del alumno en formato de tabla.

| Grupo | Nombre del alumno| Valor de la tarjeta|
|:----:|:----:|:----:|
|1391|Amezcua Arevalo Sntigo|4F3CD120|
> * Tomar tabla como referencia

4. El sistema avisará que en caso de que algún campo de la modificación se deje vacío, no se modificará ese campo.
5. El sistema solicitará el dato del alumno que se modificará (Nombre o tarjeta o grupo)
 - En caso de modificar tarjeta
    1. El sistema extiende al caso de uso "CU -007: Modificar Tarjeta"
6. El sistema mostrará los nuevos datos en formato de tabla y pide que se confirme.

| Grupo | Nombre del alumno| Valor de la tarjeta|
|:----:|:----:|:----:|
|1391|Amezcua Arévalo Santiago|7C5CD480|
> * Tomar tabla como referencia

7. El sistema mostrará mensaje del resultado de la operación en forma de mensaje "pop up".
