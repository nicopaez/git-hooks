Git Hooks
=========

Agregar a cada commit que ocurre fuera del branch master el mismo prefijo que el branch.
O sea, dado un commit:

* Si el commit es en el branch master, entonces no hacer nada
* Si el commit es en un branch distinto de master entonces agregar al commit el prefijo del branch.

Ejemplo:

* Commit con mensaje original "Actualización de readme" en branch master, entonces el mensaje de commit resultante es "Actualización de readme"
* Commit con mensaje "Agregado de valición de valor" en branch dev-30/validacion, entonces el mensaje de commit resultante es: "dev-30: Agregado de valición de valor"

Hook: commit-msg

* Recibe el nombre de un archivo temporal con el mensaje de commit
* Si devuelve un código disinto de 0 el proceso de commit es abortado



