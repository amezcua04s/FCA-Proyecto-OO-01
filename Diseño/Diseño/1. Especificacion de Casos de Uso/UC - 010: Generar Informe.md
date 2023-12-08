# ID
 - UC - 010 : Generar Informe
   
## Actores
 * Profesor
   
## Tipo 
 * Secundario

## Partes interesadas e intereses:
- El profesor podrá obtener informes de asistencia de los alumnos

## Breve descripción
El sistema proveerña los informes del grupo seleccionado hasta el momento de la generación de este (asistencias por alumno y la fecha de la asistencia)

## Pre condiciones
- El profesor debe de tener al menos un grupo registrado en el sistema

## Disparador
El profesor ingresará a la opcion de "Informe" dentro del grupo sobre el cuál exportara el informe

## Flujo normal de eventos
1. El profesor ingresa al apartado de Informes 
2. El sistema muestra la información del grupo en forma de tabla con todos los registros encontrados hasta la fecha de consulta

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

3. El profesor ingresara la opcion "Continuar" 
5. El sistema solicita al profesor guardar el archivo de forma local, y le de un nombre al archivo
6. Una vez seleccionado el formato, el sistema crea un archivo con formato "PDF" y lo exporta al almacenamiento local del celular del profesor
7. El sistema muestra un mensaje de exito de la operación