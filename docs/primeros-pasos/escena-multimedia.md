# Escenas con contenido multimedia
En la emisión en directo o grabación de eventos es importante tener previstos ciertas circunstancias, como por ejemplo estar emitiendo una cabecera con información del evento que contenga música, emitir un video de información sobre el organizador del evento, etc. En definitiva vamos a necesitar escenas con contenido multimedia ya sea de audio, de video o de ambos.

Antes de continuar con este apartado es muy conveniente, por no decir totalmente necesario, que veamos la sección [Perfil de retransmisión](../apartados/perfiles.md) y que tengamos claros los temas de configuraciones y ajustes que se explican en la sección [Configuraciones-Ajustes]().

En mi caso estos son los parámetros de configuración elegidos:

* Resolución para emisión: 1280x720 - 720p
* Resolución del lienzo por defecto: 1920x1080 - 1080p
* Resolución del lienzo adoptada para emisión: 1280x720 - 720p
* Filtro de escalado bicúbico
* 30 FPS
* Bitrate de video: 2500 a 3500 kb/s para 1280x720 y 4500 a 6000 kb/s para 1920x1080
* Bitrate de audio: 128 ó 160
* Con ancho de banda muy limitado: emitimos a 720p, bitrate de 1500 kb/s y bitrate de audio 128

## Standby
En este caso vamos a ver como se crea una escena que contenga una imagen fija y que se escuche una determinada música de fondo. Este tipo de escena va a resultar útil para ponerla previo comienzo del acto en si mismo, de manera que, por decirlo de alguna manera, estamos emitiendo en directo con información fija. Veamos como se hace.

## Video presentación evento
En este caso vamos a ver como hacer una escena que contenga un video que se reproduce en bucle y nos presenta información del organizador del evento.
