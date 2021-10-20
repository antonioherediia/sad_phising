# Práctica Phising Antonio Heredia 2ºASIR

- Lo primero que tenemos que hacer es copiar el código fuente de la web a hacer el ataque y guardarlo como index.html.
![captura1](https://pruebas.nuevomarketing.es/wp-content/uploads/2021/10/Captura.png)


- Ahora vamos a editar ese index.html y tenemos que editar primero cambiamos el method lo cambiamos de POST a GET, ya que POST oculta los datos y GET no, por lo que lo necesitaremos para recopilar los datos de incio.

- Seguidamente editamos el cambio action que apunta a Facebook y lo tenemos que cambiar para que apunte a un archivo que vamos a crear llamado next.php.
![captura2](https://pruebas.nuevomarketing.es/wp-content/uploads/2021/10/2.png)&nbsp;


- El código Script que vamos a usar es el siguiente:
![captura3](https://pruebas.nuevomarketing.es/wp-content/uploads/2021/10/4.png)


- Este código lo que hace redirige los datos de acceso a un archivo llamado yaeremio.txt y seguidamente lo manda de nuevo a Facebook.com para no levantar demasiadas sospechas.

- Ese archivo yaeresmio.txt irá vacio ya que es donde se almacenarán los datos del phising.
- Ahora subimos los tres archivos al servidor, el index, el next y el txt.
- Realizaré una prueba en mi propio servidor.

- Como vemos en el dominio de prueba accede perfectamente a el clon.
![captura4](https://pruebas.nuevomarketing.es/wp-content/uploads/2021/10/5.png)


- Introducimos un correo de prueba y una contraseña
![captura5](https://pruebas.nuevomarketing.es/wp-content/uploads/2021/10/6.png)


- Luego accedemos al archivo victima.txt (que fue el nombre que yo le puse en vez de yaeresmio.txt)
Vemos que deja los datos de forma correcta.	
![captura6](https://pruebas.nuevomarketing.es/wp-content/uploads/2021/10/7.png)







- Nombre y apellidos del estudiante
- Nombre del módulo: Seguridad y Alta Disponibilidad
- Fecha de creación
- Título del vídeo
- [Logo de la Junta de Andalucía](https://github.com/jemole/SAD_2122/blob/main/IdentidadGrafica/Logo_CED_Junta.png)
- [Logo del PdV](https://github.com/jemole/SAD_2122/blob/main/IdentidadGrafica/logo_pdv.png)

Aquí se incluye una portada de ejemplo:
![Ejemplo de portada de vídeo](https://github.com/jemole/SAD_2122/blob/main/IdentidadGrafica/Ejemplo_portada.png)

