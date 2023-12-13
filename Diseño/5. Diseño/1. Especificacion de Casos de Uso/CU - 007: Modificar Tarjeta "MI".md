# ID
- CU - 007 : Modificar Tarjeta "MI"
   
## Actores
- CU - 008: Modificar Alumno
    
## Tipo 
- Secundario
   
## Intereses:
- El profesor modificará la tarjeta que está registrada a un alumno.
- El alumno desea cambiar la tarjeta en la que están asociados sus datos.
  
## Breve Descripción
- El sistema cambiará el valor de la tarjeta que está asociado a algún alumno, transfiriendo todos los registros del alumno a la nueva tarjeta y borrando la tarjeta pasada del almacenamiento.

## Pre condiciones
- El alumno al que se le desea modificar la tarjeta debe de existir registrado previamente en el sistema.

## Disparador
- El profesor seleccionará "Modificar tarjeta" en el apartado de modificar alumno.

## Relaciones
- **Incluye**: CU - 006: Eliminar Tarjeta "MI"
- **Incluye**: CU - 003: Registrar Tarjeta "MI"

## Flujo normal de eventos
1. El caso de uso "CU - 008: Modificar Alumno" se extenderá a este caso de uso.
2. El sistema mostrará los datos y preguntará si se desea continuar con la operación.
3. El sistema solicitará leer la nueva tarjeta "MI".
4. El sistema se extenderá al caso de uso "CU - 003: Registrar Tarjeta "MI"".
5. El sistema se extenderá al caso de uso "CU - 006: Eliminar Tarjeta "MI"".
6. El sistema mostrará un "pop-up" con la nueva tarjeta asociada.
7. El sistema regresará un mensaje del resultado de la operación.
   
## Subflujos
- S-1 En el paso 4 (En caso de que se encuentre la tarjeta registrada en el sistema)
    1. El sistema mostrará el error.
    1. El sistema mostrará la información del alumno en forma de tabla que tiene registrada esta tarjeta.
    
    | Grupo | Nombre del alumno| Valor de la tarjeta|
    |:----:|:----:|:----:|
    |1391|Amezcua Arévalo Santiago|7C5CD480|
     > * Tomar tabla como referencia.
    
    1. El flujo se reanudará en el paso 8 del flujo normal.