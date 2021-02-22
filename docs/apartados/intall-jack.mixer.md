# Instalación de Jack Mixer
Vamos a realizar la instalación a través de los paquetes debian que encontramos en este [enlace](https://packages.debian.org/stable/jack-mixer), para ello comenzamos por descargar la versión que se adapte a nuestro sistema, en mi caso arquitectura amd64. Esto lo encontramos en el enlacen anterior bajando por la página hasta que veamos algo similar a la imagen 1.

<center>

| Imagen 1 |
|:-:|
| ![Opciones de descarga disponibles](../img/intall-jack/i1.png) |
| Opciones de descarga disponibles |

</center>

Se nos mostrará una lista de servidores desde donde proceder a la descarga. En mi caso elijo uno de Europa.

Hemos podido observar que en la página inicial se da un listado de paquetes relacionados con jack mixer, marcados en rojo están las dependencias, en azul las recomendaciones y en verde las sugerencias, tal y como vemos en la imagen 2.

<center>

| Imagen 2 |
|:-:|
| ![Paquetes relacionados con jack mixer](../img/intall-jack/i2.png) |
| Paquetes relacionados con jack mixer |

</center>

Una vez realizadas las descargas indicadas debemos tener, como vemos en la imagen 3, los tres archivos necesarios para proceder con las instalaciones. Se indica además el orden de instalación que debemos seguir para que se instalen los paquetes y todas las dependencias necesarias.

<center>

| Imagen 3 |
|:-:|
| ![Archivos necesarios para instalar](../img/intall-jack/i3.png) |
| Archivos necesarios para instalar |

</center>

El método que voy a seguir para instalar es a partir de una terminal utilizando `GDebi`, pero también se podría lanzar en modo gráfico tal y como vemos en la imagen 4. De las dos formas vamos a llegar a la ventana gráfica de GDebi que vemos en la imagen 5b.

<center>

| Imagen 4 |
|:-:|
| ![Lanzar GDebi en modo gráfico](../img/intall-jack/i4.png) |
| Lanzar GDebi en modo gráfico |

</center>

En mi caso y para mas claridad he situado los tres archivos en un directorio concreto.

Si procedemos como vemos en la imagen 5a (o en la imagen 4) se nos abrirá la ventana que vemos en la imagen 5b.

<center>

| Imagen 5a | Imagen 5b |
|:-:|:-:|
| ![Lanzamos GDebi desde la terminal](../img/intall-jack/i5a.png) |![Ventana gráfica de GDebi](../img/intall-jack/i5b.png) |
| Lanzamos GDebi desde la terminal | Ventana gráfica de GDebi |

</center>

Desde el menú archivo procedemos a abrir el primer archivo ("python-fpconst_0.7.2-6_all.deb") y se nos mostrará algo similar a lo que vemos en la imagen 6. Si son necesarias algunas dependencias nos informará de ello y por tanto debemos tener conexión a internet para que estas se descarguen de los repositorios oficiales de Ubuntu.

<center>

| Imagen 6 |
|:-:|
| ![Paquete python-fpconst listo para instalar](../img/intall-jack/i6.png) |
| Paquete python-fpconst listo para instalar |

</center>

Es posible que se nos solicite contraseña de superusuario para llevar a cabo la tarea. Transcurridos unos instantes se muestra lo que vemos en la imagen 7 que no indica que el proceso ha finalizado.

<center>

| Imagen 7 |
|:-:|
| ![Paquete python-fpconst instalado](../img/intall-jack/i7.png) |
| Paquete python-fpconst instalado |

</center>

Procedemos a cerrar ambas ventanas para recuperar el usuario, ya que en este momento somos `root`.

Abrimos de nuevo GDebi y vamos a instalar el archivo "python-gtk2_2.24.0-5.1+b1_amd64.deb" tal y como vemos en la imagen 8. En este caso se requieren otros dos paquetes. En la imagen 8 vemos el resultado de la instalación.

<center>

| Imagen 8 |
|:-:|
| ![Paquete python-gtk2 instalado](../img/intall-jack/i8.png) |
| Paquete python-gtk2 instalado |

</center>

Cuando finalice la instalación volvemos a cerrar las ventanas abiertas y procedemos a instalar el programa jack mixer. En este caso se requiere la instalación de otros diez paquetes adicionales, tal y como se observa en la imagen 9.

<center>

| Imagen 9 |
|:-:|
| ![Paquete jack-mixer_10-1+b1_amd64 listo para instalar](../img/intall-jack/i9.png) |
| Paquete jack-mixer_10-1+b1_amd64 listo para instalar |

</center>

En algún momento se va a mostrar la ventana de la imagen 10, donde debemos seleccionar la opción para poder ejecutar a posteriori jack con prioridades en tiempo real.

<center>

| Imagen 10 |
|:-:|
| ![Selección de prioridades en tiempo real](../img/intall-jack/i10.png) |
| Selección de prioridades en tiempo real |

</center>

Una vez finalizada la instalación se muestra la imagen 11 con la información del paquete instalado.

<center>

| Imagen 11 |
|:-:|
| ![Paquete jack-mixer_10-1+b1_amd64 instalado](../img/intall-jack/i11.png) |
| Paquete jack-mixer_10-1+b1_amd64 instalado |

</center>

Ya podemos localizar el programa entre nuestras aplicaciones, tal y como se muestra en la imagen 12.

<center>

| Imagen 12 |
|:-:|
| ![Accesp a Jack Mixer](../img/intall-jack/i12.png) |
| Accesp a Jack Mixer |

</center>

La primera vez que ejecutamos el programa tendrá el aspecto de la imagen 13 dado que no tenemos configuradas ni entradas ni salidas.

<center>

| Imagen 13 |
|:-:|
| ![Programa Jack Mixer](../img/intall-jack/i13.png) |
| Programa Jack Mixer |

</center>

En la imagen 12 observamos también que está disponible QjackCtl, que es una herramienta gráfica para controlar Jack. Tiene como funciones básicas:

* Detectar automáticamente el hardware audio

* Permite al usuario elegir subdispositivos para entradas y salidas desde una lista drop-down

* Incluye opciones comunes para el servidor de sonido.

En la imagen 14a podemos ver el aspecto de QjackCtl gestionando Jack y en la 14b un ejemplo de conexiones.

<center>

| Imagen 14a | Imagen 14b |
|:-:|:-:|
| ![QjackCtl gestionando Jack](../img/intall-jack/i14a.png) | ![Conexiones QjackCtl](../img/intall-jack/i14b.png) |
|QjackCtl gestionando Jack | Conexiones QjackCtl |

</center>
