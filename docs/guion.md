# Ejemplo de guión y colección de recursos
Sección en la que vamos a establecer un posible guión de un taller con dos ponentes en remoto compartiendo cámaras y pantallas producido por una tercera persona y visualizado en directo a modo de control. El programa será también grabado. Para ello se van a utilizar una serie de recursos creados que se ponen a disposición en esta misma sección.

## Guión para taller
* Creamos y seleccionamos el perfil para Youtube y/o Twitch. 1280x720 a 30 FPS y Bitrate 2500
* Creamos nuestra colección de escenas que va a contener las siguientes:
    * **1-Video-espera**. Video de presentación que se estará reproduciendo durante los minutos de cortesía hasta que los inscritos se unan a la transmisión. La grabación se iniciará justo después de poner el video y la espera no durará mas de cinco minutos.
    * **2-Patrocinadores**. Antes de iniciar la presentación se dará paso a la escena que va a contener una vista de la cámara del presentador, letreros junto al logo del club que indique quien organiza, el nombre de los ponentes y quien ejerce el control del chat del directo.
    * **3-Presenta**. El presentador realiza la presentación o inauguración del taller o acto. Se muestra un cartel de fondo y en una esquina la cámara del presentador.
    * **4-Camara-Pantalla-1**. Aquí vamos a poner un fondo con espacio de 240x135px para la cámara del primer ponente, uno de 1680x945px para la pantalla compartida y una zona para un letrero deslizante en la parte inferior ocupando todo el ancho que utilizaremos para mostrar información relevante. Esta misma situación se va a repetir para cada ponente y debemos tener abiertas las salas de control para cada caso y ponente y también tenemos que recordar a los ponentes que deben mantener abiertas las dos pestañas con los enlaces suministrados. Es buena idea tener archivado un listado de enlaces, guardar las pestañas en los marcadores del navegador y hacer pruebas de configuración previas. Justo debajo de la cámara vamos a poner un gif animado que indique que estamos emitiendo en directo.
    * **4bis-4-Camara-Pantalla-1**. Se  trata de las mismas escenas que las descritas en 4, una para cada número, pero esta vez no aparece el texto que se desliza. En la edición del programa se irán intercambiando las escenas 4 y 4bis para no recargar la transmisión con el texto deslizándose.
    * **5-Camara-pantalla-local**. Igual que las escenas 4 pero utilizando cámara y pantalla local, por ejemplo para la persona que está llevando la edición del programa.
    * * **5bis-Camara-pantalla-local**. Igual que las escenas 4bis pero utilizando cámara y pantalla local, por ejemplo para la persona que está llevando la edición del programa.
    * **6-Control-directo**. Escena creada por si la persona encargada de l control de la emisión en directo debe intervenir. Debemos tener en cuenta que el directo tiene un retardo de casi un minuto respecto a lo que está ocurriendo en directo.
    * **7-Final**. Simplemente se pone la imagen de despedida con el logo y un letrero. Desde aquí se hará un fundido a negro justo antes de detener la emisión y la grabación del programa.
    * **PROBLEMAS**. Escena prevista por si existe algún problema en la transmisión en directo. Se muestran códigos QR de enlaces a web, twitter y únete, junto a la presentación de patrocinadores y un texto indicativo de que hay problemas en la emisión. Suena música de fondo

## Listado de recursos
Todos  están disponibles en el directorio *Recursos* del repositorio. A continuación se da un listado de los mismos con los nombres de los archivos.

<center>

| Para la escena | Utilizado en OBS | Fuente | Detalles |
|---|---|---|---|
| 1-Video-espera | Video-corporativo.mp4 | --- | Color de fondo #FF5500 <br>Texto *Comenzamos en breve*</br> |
| 2-Patrocinadores | patrocinio.png <br>Imágenes</br><br>Música de fondo</br> | patrocinio.svg <br>*/Patrocinadores*</br><br>*/Music* | La galería de imágenes se mostrará en bucle cada 3 segundos con una velocidad de transición de 400 |
| 3-Presenta | inicio-fin.png | inicio-fin.svg | --- |
| 4-Camara-Pantalla | camara_pantalla_ninja.png <br>emitiendo.gif</br> | camara_pantalla_ninja.svg | Se repite para cada ponente |
| 4bis-Camara-Pantalla | camara_pantalla_ninja-bis.png <br>emitiendo.gif</br> | camara_pantalla_ninja-bis.svg | Se repite para cada ponente |
| 5-Camara-Pantalla-local | camara_pantalla_ninja.png <br>emitiendo.gif</br> | camara_pantalla_ninja.svg | Se repite para cada ponente |
| 5bis-Camara-Pantalla-local | camara_pantalla_ninja.png <br>emitiendo.gif</br> | camara_pantalla_ninja.svg | Se repite para cada ponente |
| 6-Control-directo | Fondo de color #FFAA00 <br>emitiendo.gif</br> <br>ROBOCILIO-transparente.png</br> | ROBOCILIO-transparente.png | --- |
| 7-Final | inicio-fin.png | inicio-fin.svg | --- |
| PROBLEMAS | Standby.png | Standby.svg | --- |

