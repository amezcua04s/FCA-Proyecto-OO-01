# ID: 
- UC - 006 : Baja grupo
   
## Actores
  - Profesor
    
## Tipo
- Secundario

## Relaciones
- **Incluye**: Eliminar Alumno

## Flujo de eventos
1. El profesor entra al apartado de eliminar grupo
2. Selecciona el grupo y el sistema le muestra la información del grupo
3. El sistema pregunta si desea continuar con la operacion
4. El sistema muestra mensaje del resultado de la operación

## Sub-flujo
* S-1 En el paso 3
    1. El profesor acepta la operacion
    2. El sistema elimina a todos los alumnos que conformen el grupo de forma total
    3. El flujo continua en el paso 4
       
* S-2 En el paso 3
    1. El profesor cancela la operación
    2. El flujo continua en el paso 4

## Excepciones
- El profesor no tiene registrado ningún grupo de forma activa, por lo que no puede realizar la operación
