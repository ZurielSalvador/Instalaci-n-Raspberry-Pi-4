# Instalacion-Raspberry-Pi-4
Se elabora la presente actividad para poder verificar la conexión de nuestro Raspberry Pi 4 (Comunicación con ssh)

Primero se hace la verificación de la camara con el ESP32-CAM
Las conexiones se hacen de la siguiente manera:

[![ESP32-CAM.png](https://i.postimg.cc/K8d6nk5c/ESP32-CAM.png)](https://postimg.cc/K1DpbYVC)

Se siguio los pasos del siguiente curso: https://edu.codigoiot.com/course/view.php?id=850




Posteriormente se habre el programa ARDUINO, y dentro de los examples, seleccionas EPS32, Camara y saldra lo siguiente:

[![CODIGO-ARDUIN-ESP32-CAMARA.png](https://i.postimg.cc/Ls5V6NPn/CODIGO-ARDUIN-ESP32-CAMARA.png)](https://postimg.cc/SX09gLDh)



Se elige que tipo de camra en este caso: #define CAMERA_MODEL_AI_THINKER // Has PSRAM
Y también se le agrega el nombre de tu Red y contraseña

Posteriormente se indica indicara en la terminal que se a conectado correctamente y utilizando la IP, lo buscas en el navegador, le das iniciar stream y saldra lo siguiente:

[![camara-esp32.jpg](https://i.postimg.cc/ydqS4Pyq/camara-esp32.jpg)](https://postimg.cc/8FHCLLYw)



----------------------------------------------------------------------------------------------

Ahora para la instalación de Raspberry Pi 4

Primero instalaremos la versión de Ubuntu.
Segundo, se descara el archivo "Imager" y le das click, este te enviara a la tienda para descargar lo necesario y lo instalas.
Tercero, posteriormente buscas en aplicaciones Imager y lo abres.


Te saldra lo siguiente:
[![interfaz-de-imager.png](https://i.postimg.cc/0QTgC6v0/interfaz-de-imager.png)](https://postimg.cc/Hc9PYkVr)

Seleccionar RaspberryPi OS 32bits

Seleccionar tarjeta MicroSD
	-Insertar la tarjeta en el adaptador
	-Insertar el adaptador 
	-Seleccionar unidad
	
Configuraciones 
	-Enable SSH
	-Username pi
	-Password: ****
	-Configure Wireless LAN
	
    En dado caso que no lo hagas por el metodo ssh, este son sus configuracion default
	Default Password: raspberry
	Defalut User: pi
	
Por ultimo hacer Click en write.

Sacamos la tarjeta microSD y la ponemos en la Raspberry Pi 4

Posteriormente:
-Energizamos
-Obtener la IP de la Raspberry Pi
-Conectarse por SSH de la siguiente manera:

ssh pi@192.168.x.x


Y listo;
[![Comunicacion-por-ssh.png](https://i.postimg.cc/bvLNL9VH/Comunicacion-por-ssh.png)](https://postimg.cc/jWwbSPbL)

Estaremos conectados.
