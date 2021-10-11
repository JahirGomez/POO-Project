# Casos de uso

|Funcionalidad |Actor que realiza la acción |Descripción |
|---|---|---|
|Administración de autenticación |Usuario | Administra el registro de nuevos usuarios, los inicios de sesiones, así como el cierre de sesión del usuario. |
|Realizar consulta |Usuario |Mediante la entrada por teclado, el usuario ingresa caracteres que hacen referencia a las características particulares que a éste le interesan o que, en su defecto, conozca del anime que desea buscar. |
|Administración de la base de datos |Administrador | Permite a las personas admitidas con cuenta de administrador, realizar modificaciones a la base de datos, dichas modificaciones se pueden clasificar en: actualizar, agregar y eliminar contenido. |

|CU01 | 1.0 |
|---|---|
|Dependencias |-Registrar nuevos usuarios -Iniciar sesión -Cerrar sesión |
|Precondición |Tener cuenta de correo(gmail) o una cuenta de Facebook|
|Descripción|El sistema permite al usuario crear una cuenta, iniciar sesión y cerrar sesión|
|Paso |Acción |
|1 |El usuario selecciona con que desea realizar el registro, ya sea Facebook o una cuenta de correo(gmail) |
|2 | Una vez registrado, el usuario debe iniciar sesión con la opción seleccionada|
|3 | Una vez finalizado el usuario puede cerrar la sesión de su cuenta |
|Postcondición |El usuario tendra acceso al sistema |
|Excepciones - Paso |Acción |
 |2 |Si el usuario ingresa datos incorrectos de su cuenta o intenta iniciar sesión con una cuenta no registrada |
 ||E.1 El sistema informa de la problemática que impide iniciar sesión | 
 ||E.2 Se borran los datos ingresados y se le pide al usuario digitar de nuevo sus datos  |
|Comentarios |El número máximo de intentos para iniciar sesión es de 5, despues del quinto intento el sistema no le permite al usuario ingresar sus datos|

|CU02 |1.0 |
|---|---|
|Dependencias |-Realizar consulta -Recibir datos sobre algún anime |
|Precondición |El usuario ha creado una cuenta o a iniciado sesión |
|Descripción|El sistema deberá comportarse como se describe en el siguiente caso de uso cuando el usuario de la API solicité al sistema datos sobre algún anime en especifico |
|Paso |Acción |
|1 |El usuario accede a la interfaz/pantalla principal para comenzar el proceso de búsqueda de un anime |
|2 | El usuario ingresa una cadena de caracteres/enunciados con las características específicas del anime que desea buscar|
|3 | El usuario ingresa una cadena de caracteres/enunciados con las características específicas del anime que desea buscar |
|4 |La API devuelve toda la información encontrada |
|Postcondición |El usuario recibe toda la información acerca del anime buscado |
|Excepciones - Paso |Acción |
 |2 |Si el usuario en lugar de agregar una cadena de caracteres ingresa datos numéricos |
 ||E.1 El sistema informa de la problemática que impide realizar la búsqueda | 
 ||E.2  Se reinicia el buscador |
|Comentarios |El número máximo de búsquedas de anime es ilimitado, siempre que el usuario desee conocer todo acerca de algún anime podrá realizar una búsqueda en la API. |

|CU03 | 1.0 |
|---|---|
|Dependencias |Actualización de contenido |
|Precondición |Para tener acceso a la funcionalidad de poder modificar la información contenida en la base de datos, se deberá haber realizado un previo inicio de sesión con cuenta de administrador |
|Descripción|Mediante esta funcionalidad, se podrá tener autorización para la modificación de la base de datos, es decir, crear, actualizar o borrar uno o más animes |
|Paso |Acción |
|1 |Ingresar a la base de datos |
|2 | Elegir la acción a realizar, ejecutarla y guardar los cambios realizados |
|3 | Salir de la base de datos |
|Postcondición |La base de datos refleja las modificaciones hechas |
|Excepciones - Paso |Acción |
 |2 | Si los cambios realizados no son guardados |
 ||E.1 El sistema no refleja los cambios realizados e ignora todo lo que se haya agregado, modificado o quitado de la base de datos | 
|Comentarios | Los usuarios administradores son los unicos con los permisos necesarios para actualizar la información contenida en la base de datos |

## Diagrama de casos de uso
[![Casos-de-uso-2.png](https://i.postimg.cc/GtrkKQds/Casos-de-uso-2.png)](https://postimg.cc/R6s6Vw3M)
