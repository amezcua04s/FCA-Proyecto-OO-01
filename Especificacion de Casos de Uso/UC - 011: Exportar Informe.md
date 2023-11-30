# ID
- UC - 011 : Exportar Informe
   
## Actores
- Profesor
    
## Tipo 
- Terciario
   
## Intereses:
- El profesor desea exportar el informe solicitado previamente 
  
## Breve descripción
- El sistema permitirá exportar el informe de asistencias solicitado, el sistema podra exportar el informe en los formatos: .xslx / .xls / .xml / .xlw / .txt 
  
## Pre condiciones
- El profesor debe de tener un informe generado

## Disparador
- El profesor indicara la opción de "Exportar Informe" desde "Proveer Informe"
  
## Relaciones
- **Extiende**: Proveer Infomes

## Flujo normal de eventos
1. El sistema llama al caso de uso
2. El profesor indica la opcion de "Exportar Informe"
3. El sistema pregunta en que formato desea exportar el informe (.xslx / .xls / .xml / .xlw / .txt )
4. El sistema pregunta hacia donde se desea exportar el informe (lugar de almacenamiento)
5. El sistema valida que la opcion sea valida
6. El sistema mostrara un mensaje de exito

## Sub-Flujo 
S-1 En caso de que en el paso 5 (El sistema no válida la opcion elegida por el profesor)
  1. El sistema mostrara un mensaje de error 
  2. El sistema mostrara si se desea volver a intentar exportar el informe 
  3. El profesor indicara su repuesta
  1. El caso de uso se reaunda en el paso 5

## Excepciones 
-En caso de que en el paso 3 del sub-flujo 1 el profesor indica que no desea volver a intentar, el sistema vuelve al UC-010
