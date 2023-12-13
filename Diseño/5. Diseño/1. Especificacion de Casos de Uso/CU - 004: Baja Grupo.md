# ID: 
- CU - 004: Baja grupo
   
## Actores
- Profesor
    
## Tipo
- Secundario

## Relaciones
- **Incluye**: CU - 005: Eliminar Alumno

## Partes interesadas e intereses:
- El profesor eliminará de forma definitiva todos los datos de un grupo
  
## Breve descripción
- El profesor elimina todos los registros que esten asociados a un grupo, así como la información de los alumnos que esten asociados al grupo.

## Pre condiciones
- El profesor debe de tener al menos un grupo registrado dentro del sistema.

## Flujo de eventos
1. El profesor seleccionará el grupo que desea eliminar.
2. El profesor seleccionará la opción "Baja de grupo".
3. El sistema mostrará un "pop-up" de advertencia, pues si elimina el grupo, se eliminan todos los registros asociados a este.
4. El sistema mostrará toda la lista de los alumnos registrados en formato de tabla.

| Análisis y Diseño de Sistemas | Nombre del alumno| Valor de la tarjeta|
|:----:|:----:|:----:|
|1391|Amezcua Arévalo Santiago|7C5CD480|
|1391|Ada Lovelaceo|9F132A21|
|1391|Amezcua Arévalo Santiago|1EC843F0|
> * Tomar tabla como referencia

5. El sistema preguntará si desea continuar con la operacion.
6. El sistema continuará en el caso de uso "CU - 005: Eliminar Alumno" y elimina de forma individual a  cada alumno asociado al grupo.
7. El sistema eliminará todos los informes que encuentre del grupo seleccionado.
8. El sistema mostrará mensaje del resultado de la operación en forma de "Pop-up".

## Sub-flujo       
* S-2 En el paso 5 (En caso de rechazar la realización)
    2. El caso de uso continuará en el paso 8