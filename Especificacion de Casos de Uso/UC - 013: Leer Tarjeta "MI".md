# ID
- UC - 013: Leer Tarjeta "MI"
   
## Actores
* Sistema
  
## Tipo 
* Escencial
   
## Partes interesadas e intereses:
- El aplicativo podrá leer el identificador único de una tarjeta NFC

## Breve descripcion
- El aplicativo será capaz de leer una tarjeta "MI" con tecnología NFC mediante el API de lectura NFC del sistema Android

## Pre Condiciones
- El sistema Android debe contar con tecnología de lectura NFC
- Debe de existir una tarjeta "MI" cerca del teléfono celular para que la pueda leer

## Disparador
- Caso de uso Registrar Tarjeta
- Caso de uso Modificar Tarjeta
- Caso de uso Registro Asistencia

## Flujo normal de eventos
1. Algun disparador inicializa este caso de uso
2. El sistema lee la tarjeta "MI" mediante la tecnología NFC
3. El sistema regresa el resultado de la operación de lectura

   
## Subflujos
- S-1 En el paso 2 (En caso de no lograr leer después de 3 segundos)
    1. El sistema muestra el error
    2. El sistema solicita al usuario que aleje y acerque de nuevo la tarjeta
    3. El caso de uso continua en el paso 2 del flujo de eventos