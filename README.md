### Desencriptación de Tráfico SSL/TLS con Key Log File

#### Descripción
El tráfico SSL/TLS asegura la comunicación entre cliente y servidor, protegiendo los datos contra posibles interceptores. Sin embargo, si se dispone de un archivo de registro de claves generado durante la captura de un archivo pcap, es posible descifrar el tráfico HTTPS y analizar su contenido. Este archivo contiene las claves de sesión necesarias para realizar la desencriptación del tráfico capturado.

- Antes de poner el archivo del **key log file**, vemos como está encriptado el tráfico en el archivo pcap.

![alt text](/ANEXOS/image.png)

- Vamos a utilizar el archivo **key log file** para desencriptar el tráfico HTTPS. Para ello nos vamos al apartado de "Edit" y seleccionamos "Preferences", acto seguido nos vamos a la pestaña de "Protocols" y seleccionamos "TLS". En esta pestaña, activamos la opción "Pre-Master-Secret log filename" y añadimos la ruta del archivo **key log file**. Una vez hecho esto, el tráfico HTTPS se desencriptará automáticamente.

![alt text](/ANEXOS/image_1.png)

![alt text](/ANEXOS/image_2.png)





