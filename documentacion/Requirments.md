# Requerimientos 
## Requerimentos de usuario:
Usuario: Persona la cual solicita los datos al sistema.
-El usuario podrá realizar la busqueda de su anime. 
## Requerimientos de usuario adminstrador:
Usuario Administrador: Persona la cual tiene acceso a modificar la base de datos.
-El usuario administrador podrá agregar actualizar o eliminar cualquier registro de anime existente.

## Requerimentos del sistema:

**Funcionales**

|RF001|Búsqueda de animes|
|---|---|
|Prioridad:|Alta|
|Descripción|El sistema permite al usuario la búsqueda de animes, ya sea por el nombre del anime, género y por el personaje |
|Entradas| Busqueda categoría // Cadena caracteres |  
|Salidas| Resultado de la búsqueda.|

|RF002|Reconocimiento de Usuarios|
|---|---|
|Prioridad|Alta|
|Descripción| El sistema permite crear una cuenta e ingresar mediante ella desde cualquier dispositivo en la red mediante un nombre de usuario y una contraseña elegidos, dicha cuenta servirá para que el usuario haga uso de la API|
|Entradas| "Usuario", "Correo/Facebook", "Password"|
|Salidas| "ID de Usuario"|

|RF003|CRUD|
|---|---|
|Prioridad|Alta|
|Descripción| Mediante una cuenta de tipo administrador, se le permite al usuario modificar la información de la base de datos, de tal manera que pueda agregar nuevos animes, modificar la información de animes ya existentes o borrar información|
|Entradas|"Eliminar" "Leer" "Actualizar" "Crear"|
|Salidas| "La opción seleccionada"|

|RF004|Agregar contenido|
|---|---|
|Prioridad|Alta|
|Descripción| Mediante una cuenta de tipo administrador se le permite al usuario agregar a la base de datos nuevos animes con todas las características que este posea|
|Entradas|"Title","Author","Gender","Chapters","Premiere date","Characters","Status","Duration","Language","Summary","Target audience"|
|Salidas| ""|

|RF005|Actualizar contenido|
|---|---|
|Prioridad|Alta|
|Descripción| Mediante una cuenta de tipo administrador se le permite al usuario actualizar la base de datos, podiendo este cambiar u agregar información a ciertos animes para que cuando un usuario clásico realice la busqueda de algún anime, se le presente la información mas adecuada y especifica|
|Entradas|"Title","Author","Gender","Chapters","Premiere date","Characters","Status","Duration","Language","Summary","Target audience"|
|Salidas| ""|

|RF006|Borrar contenido|
|---|---|
|Prioridad|Alta|
|Descripción| Mediante una cuenta de tipo administrador se le permite al usuario borrar parte de la información guardada en la base de datos|
|Entradas|"Title","Author","Gender","Chapters","Premiere date","Characters","Status","Duration","Language","Summary","Target audience"|
|Salidas| ""|


**No Funcionales**

|RNF001|Tiempo de respuesta|
|---|---|
|Descripción|El sistema deberá realizar la busqueda solicitada por el usuario en # segundo o menos|

|RNF002|Historial de busqueda|
|---|---|
|Descripción|El sistema guardará las busquedas realizadas por el usuario mientras este permanezca logueado|

|RNF003|Seguridad|
|---|---|
|Descripción|El sistema deberá ser capaz de resistir ataques de denegación del servicio que intenten saturar los servidores que utiliza el software para su funcionamiento|

|RNF004|Acceso al sistema|
|---|---|
|Descripción|El sistema debe permitir al usuario acceder con éxito a la plataforma en un 99% de las veces en las que intente ingresar al servicio|
