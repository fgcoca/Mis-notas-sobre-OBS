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

En la creación de esta escena debemos tener presente que al añadir como fuente un contenido multimedia en nuestro audio de escritorio no vamos a escuchar nada, tan solo va a ser audible en la transmisión. Esto se hace así para no interferir entre la transmisión y el trabajo local que estemos haciendo.

En el video1 podemos ver el proceso de creación de la escena y podemos comprobar que el video no tiene ningún sonido cuando lo reproducimos.

<center>

| Vídeo 1 |
|:-:|
| [Creación de escena con contenido multimedia](https://youtu.be/oqIRJ7HLngA) |

</center>

En el video 2 podemos observar y comprobar que cuando pasamos la escena a la ventana de programa el audio permanece en silencio y parece que la música seleccionada no se está reproduciendo.

<center>

| Vídeo 2 |
|:-:|
| [Escena multimedia puesta en programa](https://youtu.be/zwRwDfFuFIA) |

</center>

Observamos como se reproduce la música añadida pero no podemos oir la música. El ruido de fondo que tiene el video es el de una impresora 3D en funcionamiento muy cerca del ordenador.

El siguiente paso que vamos a dar es ver como cuando el programa se está emitiendo la música que se reproduce en la escena es perfectamente audible y ahora ya si está en el audio de escritorio. La situación que vamos a ver en el vídeo es la que se muestra en la imagen 1 en la que la ventana de la izquierda es la emisión en directo en Youtube y la de la derecha es la OBS. En el video 3 vemos como ocurre esto. Se ha dejado el ruido de fondo de la impresora 3D en funcionamiento y el nivel del audio está bastante alto para que se aprecie bien aunque esté un poco saturado. En la ventana con el enlace de la emisión podemos observar como las cosas no ocurren de inmediato y esto es debido al retardo que existe entre la producción en OBS y la transmisión en Youtube, que si observamos es de unos 40 segundos.

<center>

| Vídeo 3 |
|:-:|
| [Escena multimedia en emisión en Youtube](https://youtu.be/z_wWDbZoyuU) |

</center>

En el video 4 vemos la misma emisión pero esta vez a través de la plataforma Twitch. Se mantienen las mismas condiciones que para Youtube y el resultado es bastante similar.

<center>

| Vídeo 4 |
|:-:|
| [Escena multimedia en emisión en Twitch](https://youtu.be/k5ENK8OAC5g) |

</center>

## Video presentación
En este caso vamos a ver como hacer una escena que contenga un video que se reproduce en bucle y nos presenta información del organizador del evento. Para ello voy a utilizar el video de presentación en sus canales de [Club Robótica Granada](https://clubroboticagranada.github.io/). El proceso para transmitir un video que tengo descargado es muy sencillo porque basta con añadir una fuente multimedia y localizar ese video local.

Vamos a aprovechar para ver también como poner un origen de color como fondo de pantalla en la escena, poner algún texto adicional y finalmente ver la transmisión en directo de la escena creada en las dos plataformas que estamos usando.

En el video 5 podemos ver como poner color de fondo, texto y como añadir la fuente multimedia. Al final del video se 

<center>

| Vídeo 5 |
|:-:|
| [Escena multimedia con video local](https://youtu.be/0krY1gXpBMQ) |

</center>

De nuevo observamos como se escuchan ruidos de fondo y que aunque se ve claramente que el video tiene un audio incorporado en cuanto se activa la fuente *video con musica*. Previamente se observa que el color de fondo tapa al cuadro del video y aunque se cambie el orden de las fuentes no se consigue visualizar. Esto ocurre a veces y se soluciona en cuanto hacemos una transición o corte a la ventana de programa.

El problema de ausencia de sonido es el mismo que se explicó anteriormente y vamos a ver como se soluciona cuando estamos transmitiendo.

En el video 6 vemos como funciona la escena de video transmitida en directo en Youtube.

<center>

| Vídeo 6 |
|:-:|
| [Escena multimedia con video emitiendo en directo](https://youtu.be/2PCJa6hnp70) |

</center>
