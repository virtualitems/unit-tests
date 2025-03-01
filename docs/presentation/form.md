# Pruebas de UI / UX para formularios

# Campos de tipo numérico

- ¿Sólo se pueden digitar números?
- ¿Acepta números con ceros a la izquierda?
- ¿Acepta números decimales?
    - ¿Cuál es el separador decimal?
    - ¿Acepta ceros a la derecha después del separador decimal?
    - ¿Cuántos dígitos decimales debe aceptar?
    - ¿Debe aceptar números con ceros a la derecha después del separador decimal?

<br>

# Pruebas de UI / UX para formsets








**After submit**

- create saved new items
- delete non saved existing items
- update saved existing items

**Existing items**

- remove an existing item
- shows existing items in correct order
- shows existing items with correct values
- update value in existing item

**New items**

- create a new item
- remove a new item
- shows new items in correct order
- update value in new item

<br />

<h2 id="submit">Submit</h2>

**Event**

- submits the form pressing intro key
- submits the form pressing submit button
- submits the form after complete all fields

**Routes**

- submits the form to the correct route
- redirects to the correct route after submit

**Method**

- submits the form using the correct http method
- submits the form using the correct enctype
