# ID
 - UC - 010 : Generar Informe
   
## Actores
 * Profesor
   
## Tipo 
 * Secundario

## Partes interesadas e intereses:
- El profesor desea obtener informes de un periodo de tiempo del grupo seleccionado

## Breve descripción
El profesor podrá obtener informes de asistencia de los alumnos

## Pre condiciones
- El profesor debe de tener al menos un grupo registrado en el sistema

## Disparador
El profesor ingresará a la opcion de "Informes"

## Flujo normal de eventos
1. El profesor ingresa al apartado de Informes 
2. El sistema le pide al profesor ingresar el grupo del cuál desea obtener el informe
3. El sistema busca al grupo 
4. El sistema muestra la información del grupo en forma de tabla con todos los registros encontrados hasta la fecha de consulta

| Grupo  | Nombre del alumno  | 1/12/2023 | 6/12/2023 | 8/12/2023 | Asistencias (%) | Faltas (%) | 
|:------: |:-------------------:| :----------:| :----------:| :----------:| :----------:| :----------:|
| 1391   | Pepito perez  | &#10003;  (Asistencia)| &#10003;  (Asistencia)| &#10003;  (Asistencia)|  3 (100%)   |  0 (0%)   | 
| 1391   |  Julian Gomez| &#10011;  (Justificada)| &#10003;  (Asistencia)| &#10005; (Falta)  |1 (50%)      | 1 (50%)      | 
| 1391   | Ada Lovelace         | &#10003;  (Asistencia)  | &#10011;  (Justificada)| &#10011;  (Justificada)| 1 (100%)  | 0 (0%) |

4. El profesor ingresara la opcion "Continuar" 
5. El sistema solicita al profesor guardar el archivo de forma local, y le de un nombre al archivo
6. El sistema preguntara si desea exportar el archivo en formato "PDF" o ".csv"
7. Una vez seleccionado el formato, el sistema crea un archivo y lo exporta al almacenamiento local del celular del profesor

## Sub-flujo 
S-1 En el paso 3 (En caos de que el sistema no encuentre el grupo ingrsado)
 1. El sistema muestra un mensaje de error
 2. El sistema muestra los números de los grupos que tiene registrados
 3. El sistema pide que ingrese uno de los grupos
 4. El flujo del caso de uso continua el flujo normal en el paso 3

 ## Excepciones
 - En caso de que el profesor decida exportar en formato de pdf, el sistema creara los informes de máximo 5 días de largo, para poder llevar un orden visual
 ### La primer página del documento se vería de la siguiente manera
 | Grupo  | Nombre del alumno  | 1/12/2023 | 6/12/2023 | 8/12/2023 | Asistencias (%) | Faltas (%) | 
|:------: |:-------------------:| :----------:| :----------:| :----------:| :----------:| :----------:|
| 1391   | Pepito perez  | &#10003;  (Asistencia)| &#10003;  (Asistencia)| &#10003;  (Asistencia)|  3 (100%)   |  0 (0%)   | 
| 1391   |  Julian Gomez| &#10011;  (Justificada)| &#10003;  (Asistencia)| &#10005; (Falta)  |1 (50%)      | 1 (50%)      | 
| 1391   | Ada Lovelace         | &#10003;  (Asistencia)  | &#10011;  (Justificada)| &#10011;  (Justificada)| 1 (100%)  | 0 (0%) |
 ### Y la segunda página del documento se vería de la misma manera: 
| Grupo  | Nombre del alumno  | 1/12/2023 | 6/12/2023 | 8/12/2023| 8/12/2023 | 8/12/2023| Asistencias (%) | Faltas (%) | 
|:------: |:-------------------:| :----------:| :----------:| :----------:| :----------:| :----------:| :----------:| :----------:|
| 1391   | Pepito perez  | &#10011;  (Justificada)| &#10005; (Falta)| &#10003;  (Asistencia) | &#10005; (Falta)| &#10003;  (Asistencia)|  6 (67%)   |  3 (33%)   | 
| 1391   |  Julian Gomez|  &#10003;  (Asistencia)| &#10003;  (Asistencia)| &#10003;  (Asistencia) | &#10011;  (Justificada) | &#10003;  (Asistencia)  |6 (75%)      | 2 (25%)      | 
| 1391   | Ada Lovelace         | &#10011;  (Justificada)  | &#10005; (Falta)| &#10003;  (Asistencia)| &#10003;  (Asistencia) | &#10005; &#10003;  (Asistencia) |  5 (71%)  | 2 (29%) |