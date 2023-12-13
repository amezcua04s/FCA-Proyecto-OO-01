# ID
 - CU - 010 : Generar Informe
   
## Actores
 * Profesor
   
## Tipo 
 * Secundario

## Partes interesadas e intereses:
- El profesor podrá obtener informes de asistencia de los alumnos.

## Breve descripción
- El sistema proveerá los informes del grupo seleccionado hasta el momento de la generación de este (asistencias por alumno y la fecha de la asistencia).

## Pre condiciones
- El sistema deberá tener al menos un grupo registrado en la base de datos.

## Disparador
El profesor seleccionará a la opcion de "Informes" dentro del grupo sobre el cuál exportara el informe

## Flujo normal de eventos
1. El profesor seleccionará el apartado de "Informes".
2. El sistema mostrará la información del grupo en forma de tabla con todos los registros encontrados hasta la fecha de consulta.

 ### La primer página del documento se vería de la siguiente manera
| Grupo  | Nombre del alumno  | 1/12/2023 | 6/12/2023 | 8/12/2023| 8/12/2023 | 8/12/2023| Asistencias (%) | Faltas (%) | 
|:------: |:-------------------:| :----------:| :----------:| :----------:| :----------:| :----------:| :----------:| :----------:|
| 1391   | Pepito perez  | &#10003;  (Asistencia)| &#10003;  (Asistencia)| &#10003;  (Asistencia) | &#10003;  (Asistencia)| &#10005; (Falta)|  4 (80%)   |  1 (25%)   | 
| 1391   |  Julian Gomez| &#10011;  (Justificada)| &#10003;  (Asistencia)| &#10005; (Falta) | &#10003;  (Asistencia) | &#10005; (Falta)  |2 (50%)      | 2 (50%)      | 
| 1391   | Ada Lovelace         | &#10003;  (Asistencia)  | &#10011;  (Justificada)| &#10011;  (Justificada)| &#10003;  (Asistencia) | &#10005; (Falta) |  2 (100%)  | 1 (0%) |
 ### Y la segunda página del documento se vería de la misma manera: 
| Grupo  | Nombre del alumno  | 1/12/2023 | 6/12/2023 | 8/12/2023| 8/12/2023 | 8/12/2023| Asistencias (%) | Faltas (%) | 
|:------: |:-------------------:| :----------:| :----------:| :----------:| :----------:| :----------:| :----------:| :----------:|
| 1391   | Pepito perez  | &#10011;  (Justificada)| &#10005; (Falta)| &#10003;  (Asistencia) | &#10005; (Falta)| &#10003;  (Asistencia)|  6 (67%)   |  3 (33%)   | 
| 1391   |  Julian Gomez|  &#10003;  (Asistencia)| &#10003;  (Asistencia)| &#10003;  (Asistencia) | &#10011;  (Justificada) | &#10003;  (Asistencia)  |6 (75%)      | 2 (25%)      | 
| 1391   | Ada Lovelace         | &#10011;  (Justificada)  | &#10005; (Falta)| &#10003;  (Asistencia)| &#10003;  (Asistencia) | &#10005; &#10003;  (Asistencia) |  5 (71%)  | 2 (29%) |
> * Tomar tablas como referencia

3. El profesor seleccionará la opción "Continuar".
5. El sistema solicitará al profesor guardar el archivo de forma local, y le de un nombre al archivo.
6. El sistema creará un archivo con formato "PDF/A" y lo exporta al almacenamiento local del celular del profesor.
7. El sistema mostrará un mensaje de exito de la operación.
