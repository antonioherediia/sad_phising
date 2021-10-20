# Práctica Phising Antonio Heredia 2ºASIR


## PREPARACIÓN Y PRUEBA PHISING

Lo primero que tenemos que hacer es copiar el código fuente de la web a hacer el ataque y guardarlo como index.html.

![captura1](https://pruebas.nuevomarketing.es/wp-content/uploads/2021/10/Captura.png)


Ahora vamos a editar ese index.html y tenemos que editar primero cambiamos el method lo cambiamos de POST a GET, ya que POST oculta los datos y GET no, por lo que lo necesitaremos para recopilar los datos de incio.

![captura2](https://pruebas.nuevomarketing.es/wp-content/uploads/2021/10/2.png)&nbsp;



Seguidamente editamos el cambio action que apunta a Facebook y lo tenemos que cambiar para que apunte a un archivo que vamos a crear llamado next.php.
El código Script que vamos a usar es el siguiente:


![captura3](https://pruebas.nuevomarketing.es/wp-content/uploads/2021/10/4.png)


Este código lo que hace redirige los datos de acceso a un archivo llamado yaeremio.txt y seguidamente lo manda de nuevo a Facebook.com para no levantar demasiadas sospechas.

Ese archivo yaeresmio.txt irá vacio ya que es donde se almacenarán los datos del phising.
Ahora subimos los tres archivos al servidor, el index, el next y el txt.
Realizaré una prueba en mi propio servidor.

Como vemos en el dominio de prueba accede perfectamente a el clon.

![captura4](https://pruebas.nuevomarketing.es/wp-content/uploads/2021/10/5.png)


Introducimos un correo de prueba y una contraseña

![captura5](https://pruebas.nuevomarketing.es/wp-content/uploads/2021/10/6.png)


Luego accedemos al archivo victima.txt (que fue el nombre que yo le puse en vez de yaeresmio.txt)
Vemos que deja los datos de forma correcta.	

![captura6](https://pruebas.nuevomarketing.es/wp-content/uploads/2021/10/7.png)


## INGENIERIA SOCIAL Y ENVIOS DE EMAIL MASIVOS CON KALI

Usaremos una herramienta ya instalada en Kali llamada SET social ingenieria tolkit, eligiremos la opción 1, luego la opción 5 envio masivo de emails, seguido de la opcion 2 Email- Atack mass mailer, seguidamente nos pedirá la tura de la lista de Email.

![captura7](https://www.nuevomarketing.es/wp-content/uploads/2021/10/1.png)

Una vez introduzcamos la lista nos pedirá el tipo de cuenta, yo le diré que es GMAIL para la prueba, introducimos el correo y la contraseña.

![captura8](https://www.nuevomarketing.es/wp-content/uploads/2021/10/2.png)

![captura8](https://www.nuevomarketing.es/wp-content/uploads/2021/10/Captura.png)


Tenemos que tener activado la opcion Acceso de aplicaciones poco seguras en la seguridad del GMAIL de google sino no funcionará.

Una vez introducido esos datos nos pedirá el asunto del correo que pondremos "Inicio de sesión sospechoso en Facebook" y también si queremos adjuntar un texto plano para el mensaje o un html. yo he preparado un html para que el resultado sea el siguiente:


<body>
	<img src="https://upload.wikimedia.org/wikipedia/commons/thumb/7/7c/Facebook_New_Logo_%282015%29.svg/2560px-Facebook_New_Logo_%282015%29.svg.png" width="426.6" height="160.3" />

<h2> Inicio de sesión sospechoso </h2>
  <p>Hola, hemos detectado un inicio de sesión sospechoso procedente de Huelva, Andalucía, España. Si no has sido tu te recomendamos que cambies tu contraseña.</p>
  <img src="https://huelvaya.es/wp-content/uploads/2019/10/google-maps-huelva.jpg"/>
  <p> Accede a tu cuenta para ver los detalles del incio de sesión a través de este enlace: <a href="pruebas.nuevomarketing.es">Acceder a tu cuenta de Facebook</a>
  <p> Si has sido tu quien a iniciado sesión desde esa localización ignora este mensaje.
  <p> Buen día, el quipo de Facebook.


</body>


Como vemos despues de introducir el codigo html, nos dice que los correos se han enviado y nos muestras los correos de la lista.

![captura ](https://user-images.githubusercontent.com/92330266/138097997-d5b0abe7-0874-4170-87d8-1049a4a0824e.png)


