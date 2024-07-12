<h1 align="center"> Challenge ForoHUB API </h1>

<h2>Descripcion del proyecto</h2>
<p> Creacion de una API REST para realizar tareas CRUD utilizando el framework Spring de Java, asi como el uso de las buenas practicas de creacion y proteccion de APIs </a> </p>

## :hammer:Funcionalidades del proyecto

- `Funcionalidad General`: El usuario realiza llamadas a una URL y dependiendo del tipo de requisicion, se realiza la tarea correspondiente.
- Las peticiones del usuario se guardan, actualizan o eliminan de la base de datos (en este caso se utilizo MySQL) con base en la peticion solicitada
- `Otras funcionalidades`: La aplicacion contiene la dependencia Security para poder validar y autenticar a los usuarios que sean registrados en la base de datos.

## ✔️ Tecnologias utilizadas
- `Java 17`
- `Programacion Orienrtada a Objetos`
- `API REST`
- `Spring Framework`
- `Jackson Databind`
- `JPA`
- `MySQL`
- `Spring Security`
- `JWT`
- `MySQL`
- `Lombok`
  
## ▶️ Imagenes del programa

<p> 1) <em> Iniciacion de la API en IntelliJ </em></p>
<img src=IniciacionAPI.png width = 800px height = 400px>

<p> 2) <em> Validacion del usuario al momento de registrarse </em></p>
<p> Se valida que el usuario contenga las mismas credenciales que las guardadas en la base de datos </p>
<img src=registroUsuario.png width = 800px height = 400px>

<p> 3) <em> Generacion de Token.</em> </p>
<p> Una vez validado el usuario,se devuelve el token para que pueda autenticarse y tener acceso a las demas peticiones de la API </p>
<img src=generacionToken.png width = 800px height = 400px>

<p> 4) <em> Registro del Topico </em></p>
<p> Ya que el usuario es autenticado, puede realizar la peticion para registrar el topico deseado con sus propiedades </p>
<img src=Autenticacion.png width = 800px height = 400px>
<img src=registroTopico.png width = 800px height = 400px>

<p> 5) <em> Autenticacion de las demas peticiones de la API  </em></p>
<p> Se coloca el token en las demas peticiones y se valida que se puedan realizar las peticiones despues de la autenticacion del usuario </p>
<img src=validacionGET.png width = 800px height = 400px>
<img src=validacionPUT.png width = 800px height = 400px>
<img src=validacionDELETE.png width = 800px height = 400px>
<img src=validacionFuncionDelete.png width = 800px height = 400px>

<p> 6) <em> Respuesta 403 'Forbidden' cuando el token es invalido o nulo </em></p>
<p> Se regresa una respuesta 403 para indicar que el usuario no tiene las credenciales o accesos correspondientes para autenticarse y usar las peticiones de la API </p>
<img src=ValidacionTokenInvalido.png width = 800px height = 400px>

<p> 7) <em> Persistencia de las peticiones y usuarios dentro de la base de datos </em></p>
<p> La base de datos guarda las peticiones realizadas a la API para su persistencia </p>
<img src=DBTopicos.png width = 800px height = 400px>
<img src=DBUsuarios.png width = 800px height = 400px>
