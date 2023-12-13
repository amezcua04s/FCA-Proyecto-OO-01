# ID
 - CU - 001: Registrar grupo
   
## Actores
 * Profesor
   
## Tipo 
 * Primario

## Partes interesadas e intereses:
- El profesor desea registrar un nuevo grupo.

## Breve descripción
El profesor podrá dar de alta un nuevo grupo en el sistema, con la posibilidad de asignarle alumnos previamente registrados, así como asignarle un horario al grupo.

## Disparador
El profesor ingresará a la opción de "Registrar nuevo grupo".

## Flujo normal de eventos
1. El profesor seleccionará el apartado de "Registrar Grupo".
2. El profesor ingresará el nombre de la materia.
3. El profesor ingresará el número de grupo.
4. El sistema verificará que no exista otro registro con ese número de grupo.
5. Se guardará en el sistema la información.
6. Se mostrarán los datos del grupo en forma de tabla.

| Nombre de la materia |Grupo|
|:----:|:----:|
|Análisis y diseño de sistemas|1391| 
> * Tomar tabla como referencia

7. El sistema muestra mensaje del resultado de la operación.

## Sub-flujo
S-1 En el paso 4 (En caso de que se encuentre otro registro)
 1. El sistema señala el error y muestra la información del otro grupo ya existente
 1. El sistema pregunta si desea modificar el número del grupo
   - En caso de que si
     1. El flujo del caso de uso continúa el flujo normal en el paso 3
   - De lo contrario
     1. El flujo del caso de uso continúa el flujo normal en el paso 7

## Excepciones
- El profesor deja algún campo vacío, por lo que el registro no se lleva a cabo
