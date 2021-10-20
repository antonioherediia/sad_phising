# Práctica Phising Antonio Heredia 2ºASIR

# PREPARACIÓN Y PRUEBA PHISING

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

Una vez introduzcamos la lista nos pedirá el tipo de cuenta, yo le diré que es GMAIL para la prueba, introducimos el correo y la contraseña.

![captura7](https://www.nuevomarketing.es/wp-content/uploads/2021/10/2.png)


