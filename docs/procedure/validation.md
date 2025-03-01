# Validaciones de entrada de datos

<br>

<h2 id="general">Validaciones generales</h2>

Aplican para cualquier tipo de dato. Siempre se deben tener en cuenta.

- ¿Tiene un valor predeterminado?
- ¿Es digitado por el usuario o está oculto?
    - ¿Puede autocompletarse?
- ¿Es requerido o puede ser nulo?
- ¿Está protegido contra XSS?
- ¿Está protegido contra CSRF?

<br>

<h2 id="index-field">Para campos de código único</h2>

- ¿Es un valor único?

### Si es un UUID

- ¿Está en un formato de UUID válido?

### Si es un slug

- ¿Está en un formato de slug válido?

<br>

<h2 id="numeric-field">Para campos numéricos</h2>

### Si es un booleano

- ¿Debe aceptar "Falso"?
- ¿Debe aceptar "Indeterminado"?
- ¿Debe aceptar "Verdadero"?

### Si es un número

- ¿Debe aceptar números negativos?
- ¿Debe aceptar números positivos?
- ¿Debe aceptar el número cero?
- ¿Cuál es el número mínimo aceptado?
- ¿Cuál es el número máximo aceptado?
- ¿Debe aceptar números decimales?
    - ¿Cuál es el separador decimal?
    - ¿Cuántos dígitos decimales debe aceptar?
    - ¿Debe aceptar números con ceros a la derecha después del separador decimal?
- ¿Debe aceptar números enteros?
- ¿Debe aceptar números con ceros a la izquierda?
- ¿Debe aceptar notación científica? (Ejemplo: 21e4)

### Si es un texto

- ¿Cuál es la longitud mínima aceptada del texto?
- ¿Cuál es la longitud máxima aceptada del texto?
- ¿Cuál es la cantidad mínima de palabras aceptadas?
- ¿Cuál es la cantidad máxima de palabras aceptadas?
- ¿Debe aceptar espacios en blanco?
    - ¿Debe aceptar sólo espacios en blanco?
    - ¿Debe aceptar espacios en blanco al inicio?
    - ¿Debe aceptar espacios en blanco al final?
- ¿Debe aceptar saltos de línea?
    - ¿Debe aceptar sólo saltos de línea?
    - ¿Debe aceptar saltos de línea al inicio?
    - ¿Debe aceptar saltos de línea al final?
- ¿Debe aceptar números?
    - ¿Debe aceptar sólo números?
- ¿Debe aceptar letras?
    - ¿Debe aceptar sólo letras?
    - ¿Debe aceptar letras con tílde?
    - ¿Debe aceptar letras mayúsculas?
    - ¿Debe aceptar letras minúsculas?
    - ¿Debe aceptar letras en otros idiomas?
- ¿Debe aceptar caracteres especiales?
    - ¿Cuáles caracteres especiales debe aceptar?
    - ¿Debe aceptar caracteres invisibles?
    - ¿Debe aceptar sólo caracteres especiales?
    - ¿Debe aceptar caracteres especiales al inicio?
    - ¿Debe aceptar caracteres especiales al final?
    - ¿Debe aceptar emojis?

### Si es la ruta de un archivo

- ¿Debe aceptar rutas relativas?
- ¿Debe aceptar rutas absolutas?
- ¿Está en un formato de ruta válido?

### Si es un JSON

- ¿Está en un formato de JSON válido?
- ¿Debe aceptar un JSON con un objeto vacío?
- ¿Debe aceptar un JSON con una lista vacía?

### Si es una contraseña

- ¿Está en un formato de contraseña válido?
- ¿Sigue los criterios de contraseñas fuertes?

### Si es un número de teléfono

- ¿Está en un formato de número de teléfono válido?
- ¿Debe aceptar números de teléfono con código de país?

### Si es una URL

- ¿Está en un formato de URL válido?
- ¿Qué protocolos debe aceptar?

<br>

<h2 id="select-and-radio-field">Para campos de selección</h2>

- ¿Debe aceptar el valor predeterminado?
- ¿Debe aceptar un valor nulo?
- ¿Debe aceptar múltiples valores?
- ¿Puede quitar valores seleccionados?
- ¿Debe aceptar valores que no están en las opciones?

<br>

<h2 id="date-or-time-field">Para campos de fecha o tiempo</h2>

- ¿Está en un formato de fecha válido? (ISO 8601)
- ¿Debe aceptar una fecha o tiempo anterior?
- ¿Debe aceptar una fecha o tiempo posterior?
- ¿Debe aceptar la fecha o tiempo actual?

<br>

<h2 id="file-field">Para campos de archivo</h2>

- ¿Debe aceptar cualquier nombre de archivo?
- ¿Cuál es el tamaño mínimo de archivo aceptado?
- ¿Cuál es el tamaño máximo de archivo aceptado?
- ¿Qué formatos de archivo debe aceptar?

### Si es un CSV

- ¿Está en un formato de CSV válido?
- ¿Debe aceptar un CSV con encabezados?
- ¿Reconoce una estructura de datos válida?

### Si es una imagen

- ¿Qué tamaño de imágen debe aceptar?
- ¿Qué resolución de imágen debe aceptar?