# ID
- CU - 009 : Modificar grupo
   
## Actores
 * Profesor
    
## Tipo 
 * Secundario
   
## Intereses:
- El profesor desea cambiar la información de un grupo. 
  
## Breve descripción
El profesor podrá cambiar algún dato o datos de un grupo registrado en el sistema (Nombre de la materia ó número de grupo).

## Pre condiciones
- El profesor debe tener en el sistema al menos un grupo registrado, para poder modificar la información de este.

## Disparador
El profesor seleccionará la opción de "Modificar grupo" en el grupo correspondiente.

## Relaciones
- **Extiende**: CU : 004: Baja Grupo

## Flujo normal de eventos
1. El profesor seleccionará el apartado de "Modificar grupo" en el grupo correspondiente.
2. El sistema avisará que en caso de que algún campo de la modificación se deje vacío, no se modificará ese campo.
3. El sistema mostrará los datos del grupo en forma de tabla.

| Número de grupo | Materia |
|:----:|:----:|
|1190| Análisis y Diseño de Sistemas|
>* Tomar tabla como referencia

3. El profesor ingresará los datos que se registrarán

| Número de grupo | Materia |
|:----:|:----:|
|1391| *Se deja vacío pues no se modificará el valor*|
>* Tomar tabla como referencia

4. El sistema actualizará la información del grupo.

| Número de grupo | Materia |
|:----:|:----:|
|1391| Análisis y Diseño de Sistemas|
>* Tomar tabla como referencia

5. El sistema mostrará un mensaje del resultado de la operación en forma de pop-up.
