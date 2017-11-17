# python-datetime

# Conversiones Datetime <-> String

- La clase **datetime** del paquete **datetime** contiene los métodos **strptime** y **strftime** que pueden emplearse para realizar conversiones de tipos _datetime_ y _string_.

## strptime

- El método **strptime** crea un objeto _datetime_ a partir de:
    - una cadena de texto que representa una fecha y hora,
    - una cadena de texto que representa el formato de entrada.

- Ejemplo:
    ```
    from datetime import datetime
    obj_fecha = datetime.strptime('03/05/2017', '%d/%m/%Y')
    print obj_fecha
    ```
    Resultado:
    ```
    2017-05-03 00:00:00
    ```

## strftime

- El método **strftime** crea un objeto _string_ a partir de:
    - un objeto datetime que representa una fecha y hora,
    - una cadena de texto que representa el formato de salida.

- Ejemplo:
    ```
    import datetime
    str_fecha = datetime.datetime.strftime(datetime.datetime(2017, 5, 3), '%d %b %Y')
    print str_fecha
    ```
    Resultado:
    ```
    03 May 2017
    ```

- Más información:
    - [8.1. datetime - Basic date and time types](https://docs.python.org/2/library/datetime.html)
