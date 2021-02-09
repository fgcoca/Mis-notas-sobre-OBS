# El IDE de OBS
La primera vez que abrimos el programa el IDE presenta el aspecto de la imagen 1. Observamos como el área de trabajo está dividida en dos partes principales:

* Parte superior, muestra una ventana que es donde se verá lo que estemos grabando o emitiendo en directo.

* Parte inferior, donde se encuentran todas las ventanas de controles que nos permiten hacer la realización.

<center>

| Imagen 1 |
|:-:|
| ![Aspecto inicial del IDE de OBS](../img/IDE/i1.png) |
| Aspecto inicial del IDE de OBS |

</center>

## Modo de estudio
Si activamos este modo desde la ventana de controles observamos (Imagen 2) como el área de trabajo queda dividida en dos partes separadas por un conjunto de botones que se denomina área de transiciones.

<center>

| Imagen 2 |
|:-:|
| ![Aspecto inicial del IDE de OBS en Modo de estudio](../img/IDE/i2.png) |
| Aspecto inicial del IDE de OBS en *Modo de estudio* |

</center>

En la animación siguiente se han cargado dos escenas para demostrar el uso básico de este modo, una es una imagen fija y la otra corresponde a la entrada de la webcam.

<center>

![Manejo básico de las transiciones](../img/IDE/A1-Modo-estudio.gif)

</center>

Vamos a describir un poco el funcionamiento de este modo, y para ello vamos a utilizar las dos escenas que hemos usado anteriormente en las transiciones. En la imagen 3 tenemos una posible situación de estado en la que vemos a la izquierda previsualizada la webcam y a la derecha una imagen fija. En esta situación esta imagen será lo primero que se vea al iniciar una transmisión en directo o grabación.

<center>

| Imagen 3 |
|:-:|
| ![Estado de escenas para previsualización y emisión](../img/IDE/i3.png) |
| Estado de escenas para previsualización y emisión |

</center>

Estas dos pantallas son las que nos permiten tener a la vista lo que estamos emitiendo y lo siguiente que entrará y así poder llevar a cabo una realización exitosa. Si por ejemplo hacemos una transición por corte (suele ser el tipo mas utilizado) la situación cambiaría a la que vemos en la imagen 4 y ahora se estaría emitiendo la webcam y en previsualización estaría la imagen.

<center>

| Imagen 4 |
|:-:|
| ![Estado de escenas para previsualización y emisión](../img/IDE/i4.png) |
| Estado de escenas para previsualización y emisión |

</center>

El programa lo que hace al pulsar en transición es intercambiar los modos entre las dos últimas escenas utilizadas. En el apartado [Escenas](../apartados/escenas.md) se describen estas con mas detalle. Si añadimos mas escenas en el apartado correspondiente podremos ir creando nuestro programa para emisión o grabación. Para elegir que escena previsualizar hacemos clic en la que queramos en el apartado escenas. En la imagen 5 vemos el resultado después de hacer clic en la escena Inicio-fin partiendo de la situación que tenemos en la imagen 3, donde vemos que se está emitiendo y previsualizando la imagen fija.

<center>

| Imagen 5 |
|:-:|
| ![Estado de escenas para previsualización y emisión](../img/IDE/i5.png) |
| Estado de escenas para previsualización y emisión |

</center>

Las ventanas escenas y fuentes son las mas importantes de OBS ya que con ellas se lleva a cabo toda la realización. La ventana de escenas nos permite configurar lo que queremos emitir y la ventana de fuentes nos muestra los dispositivos y archivos multimedia para mostrar.

## Mezclador de audio
En esta ventana se nos muestra un sencillo pero a la vez útil e intuitivo mezclador de audio. Si accedemos a los ajuste de audio (Imagen 6) podemos ver las opciones de configuración y dispositivos que podemos habilitar y que explicamos brevemente.

<center>

| Imagen 6 |
|:-:|
| ![Opciones de configuración de audio: frecuencia de muestreo](../img/IDE/i6.png) |
| Opciones de configuración de audio: frecuencia de muestreo |

</center>

### Configuraciones

1. **Frecuencia de muestreo**. Nos permite escoger entre 48 kHz, que sería una frecuencia de máxima calidad para posterior edición, y 44.1 kHz que sería una frecuencia normal. Se recomienda 44.1 para cámaras no profesionales Si es conveniente que a todas las fuentes de audio les asignemos la misma frecuencia de muestreo.

2. **Canales**. En la imagen 7 vemos los canales que podemos configurar y su significado que se ha obtenido de la entrada [Audio multicanal](https://es.wikipedia.org/wiki/Audio_multicanal#:~:text=As%C3%AD%2C%201.0%20corresponde%20al%20sonido,canales%20(2.1%20o%203.0).) de la Wikipedia.

<center>

| Imagen 7 | Significado |
|:-:|---|
| ![Opciones de configuración de audio: canales](../img/IDE/i7.png) | <br> Mono. Canal de audio monoaural </br> <br> Estéreo. Canal de audio estéreo </br> <br>2.1. 2 canales (estéreo) con un canal para efectos de baja frecuencia </br> <br>4.0. Sonido cuadrafónico con dos canales frontales y dos traseros</br> <br>4.1. Sonido cuadrafónico con tres canales frontales y uno trasero</br> <br>5.1. Tres canales frontales mas dos traseros</br> <br>7.1. Tres canales frontales, dos laterales y dos traseros</br> |
| Opciones de configuración de audio: canales ||

</center>

3. **Dispositivos de audio globales**. Nos permite seleccionar las distintas fuente de entrada de audio de las que dispongamos, como micrófonos internos y microfónos auxiliares o dispositivos conectados a las tomas jack. Se recomienda escoger *por defecto* para que la configuración de dispositivos sea heredada del sistema operativo.

4. **Medidores**. El *decaimiento* se refiere al tiempo que mostrará el pico de audio en los medidores. En los *tipos de medidor de pico* es la forma en la que se mostrará el pico de audio. La opción *True peak* es la ideal teniendo en cuenta que utiliza mas recursos de la CPU.

5. **Avanzado**. Nos permite elegir el dispositivo por donde escuchar las fuentes de audio. Se puede dejar la opción por defecto si no se producen loops de audio o bien escoger la monitorización interna.

En la imagen 8 vemos las partes en las que se divide cada entrada del mezclador y su significado o descripción.

<center>

| Imagen 8 | Significado |
|:-:|---|
| ![Visulización canales de audio](../img/IDE/i8.png) | <br> a-volumen. Barras de colores indicadoras del volumen de ese canal </br> <br> b-fader. Control deslizante de volumen </br> <br>c-silencio. Botón que permite silenciar el canal. </br> <br>d-opciones. Opciones adicionales de configuración de la fuente</br> <br>e-nivel de volumen. El valor de ajuste del fader expresado en decibelios</br> |
| Visulización canales de audio ||

</center>

En las opciones adicionales de configuración (rueda dentada) tenemos otras opciones de configuración avanzadas que son:

- **Bloquear volumen**. Cuando tengamos configurado el nivel deseado de volumen podemos bloquear el fader para evitar cambiarlo accidentalmente.

- **Mostrar todos, ocultar y renombrar**. Opciones para mostrar todos los canales de audio, ocultar alguno concreto o cambiar el nombre de los mismos.

- **Copiar filtros y pegar filtros**. Permite copiar y pegar una configuración determinada de filtros.

- **Interfaz vertical**. Pone los controles del visualizados de audio en disposición vertical.

- **Filtros**. Nos da el control sobre elementos de filtrado de audio como puertas, compresores, expansores, eliminación de ruido, etc.

### Zonas del medidor de volumen
El medidor de volumen se divide (imagen 8) en tres zonas representadas en verde, amarillo y rojo.

* **Zona verde**. Es la zona ideal donde deben permanecer todos los niveles.

* **Zona amarilla**. Esta zona queda destinada al habla y es donde debe de permanecer el volumen sin entrar en la zona roja.

* **Zona roja**. Debe evitarse pues el sonido está distorsionado.

Lo ideal siempre es ajustar y bloquear el nivel de volumen entre las zonas verde y amarilla.

### Canales
A cada fuente de audio se asigna al menos un medidor de volumen. En la imagen 9 observamos los canales asignados a dos dispositivos y se observa perfectamente como uno es estéreo y el otro mono.

<center>

| Imagen 9 |
|:-:|
| ![Canales de audio](../img/IDE/i9.png) |
| Canales de audio |

</center>

En la animación siguiente vemos los indicadores en funcionamiento y a continuación se explica el significado de sus partes.

<center>

![Indicadores de audio en funcionamiento](../img/IDE/controles.gif)

</center>

A continuación vemos las distintas partes de estos indicadores.

* A la izquierda podemos ver el indicador de nivel de entrada mediante un punto estático indicando el nivel de volumen del directo en verde, rojo o amarillo. 

* Vemos unos puntos negros (siempre en movimiento) que se corresponden con el Vu-meter, o sea que indican la ‘presión del sonido’.

* La línea principal (siempre en movimiento) es el medidor de programa de picos

* El punto derecho (a veces estático)indica el pico y muestra lo más alto que ha subido el medidor, y es una excelente manera de ver si se está recortando la salida.

## Algunos detalles técnicos

### dBFS
Los niveles de audio se miden en decibelios (dB), que es una escala logarítmica que se adapta muy bien a la forma en que nuestros oídos el volumen de audio.

Pero dB es una medida relativa y podemos establecer el valor 0 dB en cualquier lugar del medidor. En audio digital, la convención es usar 0 dBFS (el sufijo FS se usa justamente para indicar esta convención) como el volumen máximo que la tarjeta de sonido, la interfaz de audio y el convertidor DA/AD pueden manejar. Los niveles de volumen más bajos se muestran siempre con valores dBFS negativos.

### PPM (Peak Programme Meter)
El PPM es la característica visual principal del medidor OBS y se ilumina como parte del medidor de volumen general.

El medidor se divide en tres secciones de colores diferentes. A -20 dBFS tenemos el nivel de alineación y a -9 dBFS tenemos el nivel máximo permitido.

### Nivel de entrada
El nivel de entrada es el indicador cuadrado pequeño en el extremo izquierdo del medidor. Este es el mejor lugar para ver si el audio es demasiado alto para la interfaz de audio que captura su micrófono.

Los colores se corresponden a los siguientes valores:

* Verde oscuro. Inferior a -50 dBFS

* Verde claro. Entre -50 y -20 dBFS

* Amarillo. Entre -20 y -9 dBFS

* Rojo. Entre -9 dBFS y -0,5 dBFS
  
* Blanco. Superior a -0,5 dBFS

seguir por minuto 6:22
