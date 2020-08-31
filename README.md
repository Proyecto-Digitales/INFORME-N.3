                                       ENTRADA Y SALIDA DE DATOS PARA UNA RASPBERRY PI


1.PLANTEAMIENTO DEL PROBLEMA

La Raspberry Pi es un ordenador de bajo coste y tamaño reducido, hoy en día es muy popular su venta para diversos proyectos ya que es fácil conectarle un televisor y un teclado para interactuar con ella exactamente igual que cualquier otra computadora. Pero una de las grandes dificultades cuando se es principiante en su uso, es como interactuar tanto en entrada como en salida de datos, y aquí surge una pregunta, ¿Cómo reconocer cada puerto o pin de entrada y salida de datos?, además de su respectiva función y ¿cómo poder utilizarlas? 


2.OBJETIVOS

Objetivo general

Implementar un ejemplo que explique cómo funciona el proceso de entrada y salida de datos en una raspberry pi.

Objetivos específicos

-Investigar el hardware de la raspberry pi.

-Comprobar el funcionamiento del ejemplo mediante el simulador en línea BrainBox.

-Implementar como aporte un circuito en físico que explique salida y entrada de datos en una raspberry.



3.ESTADO DEL ARTE

En 2019 Alberto Montón Cuartero de la UNIVERSIDAD POLITECNICA DE CATALUÑA DE INGENIERÍA EN SISTEMAS TIC diseño La idea de desarrollar un vehículo basado en Lego con un hardware determinado, diferente a lo que actualmente podemos encontrar a la hora de montar un coche comandado por una cpu Mindstorm, que es la más utilizada normalmente en los diseños con piezas Lego. Así pues, gracias al aprendizaje basado en programación de software, y de los conocimientos puestos en práctica basados en el hardware Mindstorm y Lego, hemos querido realizar un proyecto donde poder integrar todo lo asimilado. Debido a las limitaciones que presentaba Mindstorm, nos decantamos por sustituir esta cpu por un componente hardware llamado Raspberry Pi. El objetivo del proyecto consiste en diseñar un sistema inalámbrico controlado con un Smartphone que funcione como un coche teledirigido integrado en un conjunto entre Raspberry Pi, BrickPi y motores de Lego Mindstorms NXT, todo alimentado por una pila de 9V y envuelto en una estructura de piezas Lego (Alberto Montón Cuartero, 2019, p.1) [1].

Carlos Andrés González Godoy Estudiante de Ingeniería de Sistemas, Universidad Distrital Francisco José de Caldas proveer un sistema para prevenir robos en locales comerciales, utilizando un ordenador de placa Raspberry Pi 2 modelo B, una cámara y un sensor de infrarrojos, los cuales permiten conocer si existe movimiento en la puerta del local comercial en periodos de 10 segundos. Esta información se envía por medio de un mensaje de correo electrónico, adjuntando la captura de la imagen; de esta manera, el propietario toma una decisión de acuerdo a la situación. Para la integración de este sistema es necesario el uso del sistema operativo Raspbian y configuración de un servidor de SMTP para el envío de la foto capturada al correo electrónico. El sistema garantiza la detección en un 90 % bajo los parámetros de distancia y grados del sensor respecto al sospechoso, pero es dependiente de la iluminación que se tenga para la captura de la imagen; de esta manera, es una alternativa de seguridad funcional. (Carlos Andrés González Godoy, 2019, p.1) [2].

Banerjee, Sethia, Mittal, Arora y Chauhan (2013) hablan de un sensor de movimiento seguro, mediante la introducción de una conexión por cable entre el Raspberry Pi y el sensor y utilizando una clave de cifrado enviado desde el teléfono móvil a través de Bluetooth. En comparación al trabajo mencionado, el presente proyecto utiliza el correo electrónico como mecanismo para observar que ocurre con una foto, dando un valor agregado el no tener que estar enviando confirmaciones y simplemente acceder para ver la captura en caso de que haya sospechoso y no estar revisando en todo momento lo que ocurre. (Banerjee, Sethia, Mittal, Arora y Chauhan, 2013, p.1) [3].


4.MARCO TEÓRICO


![alt text](https://github.com/Proyecto-Digitales/INFORME-N.3/blob/master/Img/marcoteorico1.png)

![alt text](https://github.com/Proyecto-Digitales/INFORME-N.3/blob/master/Img/marcoteorico2.png)

5.DIAGRAMAS

•Diagramas de bloques.

![alt text](https://github.com/Proyecto-Digitales/INFORME-N.3/blob/master/Img/Bloque1.jpeg)

![alt text](https://github.com/Proyecto-Digitales/INFORME-N.3/blob/master/Img/Bloque2.jpeg)

•Diagramas eléctricos.

https://github.com/Proyecto-Digitales/INFORME-N.3/blob/master/Img/4_A.PNG


•Diagramas esquemáticos.

![alt text](https://github.com/Proyecto-Digitales/INFORME-N.2/blob/master/Img/diagrama5.jpg)



6.LISTA DE COMPONENTES

-Simulador BrainBox

-Proto

-Resistencias

-Cables

-Pulsadores

-Raspbery pi modelo B


7.MAPA DE VARIABLES

![alt text](https://github.com/Proyecto-Digitales/INFORME-N.3/blob/master/Img/Mapa.jpeg)



8.EXPLICACIÓN DEL DISEÑO

Uno de los accesorios estrella de la Raspberry Pi es su cámara. Con ella se pueden realizar numerosos proyectos, en este informe se presenta el ejemplo de cómo utilizar este módulo de cámara y que acciones nos permite realizar la raspbery pi .
Para este diseño solo presentaremos la simulación, pero es conveniente que si se requiere realizar el proyecto en físico se necesita un módulo de cámara para la raspberry, la cual debe ser una cámara IP para poder monitorear remotamente mediante la raspberry.


![alt text](https://github.com/Proyecto-Digitales/INFORME-N.3/blob/master/Img/Dise%C3%B1o1.png)


En la imagen se observa un modelo de raspberry en donde encerrado en recuadro rojo observamos la entrada del módulo del cámara conocido como puerto J3.                     


![alt text](https://github.com/Proyecto-Digitales/INFORME-N.3/blob/master/Img/Dise%C3%B1o2.png)

         
 Aquí podemos ver ya un módulo de cámara conectado al puerto J3.
Una vez explicado la ubicación donde se conectaría la cámara nos centraremos en la simulación. 
Para ello utilizamos el simulador BrainBox el cual nos presenta ya un modelo programado de cámara para la raspberry, al modelo de la cámara podemos 
añadirle una dirección IP de cualquier cámara que tengamos acceso y siempre y cuando sea en formato mjpeg. Nosotros utilizaremos la web insecam.com para 
obtener una IP de una cámara pública, la cual representará nuestra entrada de datos.

         
 ![alt text](https://github.com/Proyecto-Digitales/INFORME-N.3/blob/master/Img/Dise%C3%B1o3.png)
 
 
 ![alt text](https://github.com/Proyecto-Digitales/INFORME-N.3/blob/master/Img/Dise%C3%B1o4.png)
 
 Este es el modelo programado de la cámara para nuestra raspberry.
 
  ![alt text](https://github.com/Proyecto-Digitales/INFORME-N.3/blob/master/Img/Dise%C3%B1o5.png)
  
  En donde insertamos la dirección IP de nuestra cámara pública.
  
  ![alt text](https://github.com/Proyecto-Digitales/INFORME-N.3/blob/master/Img/Dise%C3%B1o6.png)
  
  En esta parte podemos ver diferentes bloques ya programados que representan el poder que tiene la raspberry para el proceso de imágenes. Explicaremos cada una de ellas:
  
   ![alt text](https://github.com/Proyecto-Digitales/INFORME-N.3/blob/master/Img/Dise%C3%B1o7.png)
   
   Al inicio cuando entran los datos de las imágenes proporcionadas por nuestra cámara IP, es necesario escalar a una resolución adecuada, dicha resolución dependerá del dispositivo en el que queramos reproducir las imágenes y la calidad de las imágenes que nos da la cámara de la raspberry. También podemos realizar un Histograma de imagen que, en un contexto de procesamiento de imágenes, el histograma de una imagen normalmente se refiere a un histograma de los valores de intensidad de píxeles. Este histograma es un gráfico que muestra el número de píxeles de una imagen en cada valor de intensidad diferente que se encuentra en esa imagen. Para una imagen en escala de grises de 8 bits, hay 256 intensidades posibles diferentes, por lo que el histograma mostrará gráficamente 
   256 números que muestran la distribución de píxeles entre esos valores de escala de grises.
   
   
  ![alt text](https://github.com/Proyecto-Digitales/INFORME-N.3/blob/master/Img/Dise%C3%B1o8.png)
  
  
  Convertidor de escala de grises promedio: El método promedio es el método más simple de color a escala de grises. Solo debes tomar la media de tres colores. Dado que es una imagen RGB, significa que debe agregar r con g con b y luego dividirlo por 3 para obtener la imagen en escala de grises deseada.
Inversión de color: La inversión de color, también conocida como efecto negativo, es uno de los efectos más fáciles de lograr en el procesamiento de imágenes. La inversión de color se logra restando cada valor de color RGB del valor máximo posible (generalmente 255). La inversión puede ser necesaria para realizar algunas operaciones, como operaciones morfológicas. Por ejemplo, la erosión reduce los límites de las regiones de blanco / primer plano, por lo que importa qué píxeles son blancos / primer plano.

  ![alt text](https://github.com/Proyecto-Digitales/INFORME-N.3/blob/master/Img/Dise%C3%B1o9.png)
  
  
  Voltear filtro vertical: Un giro (efecto espejo) se realiza invirtiendo los píxeles horizontal o verticalmente.
Filtro de desenfoque gaussiano: Ejecuta un desenfoque Guassian con el parámetro de nivel que especifica la extensión del desenfoque. Es un efecto ampliamente utilizado en software de gráficos, generalmente para reducir el ruido de la imagen y reducir los detalles.

  ![alt text](https://github.com/Proyecto-Digitales/INFORME-N.3/blob/master/Img/Dise%C3%B1o10.png)
  

 Flip horizontal: Un giro (efecto espejo) se realiza invirtiendo los píxeles horizontal o verticalmente.
Filtro de relieve: La función EMBOSS aplica un operador de convolución a una matriz de imágenes 2D para generar una matriz que contiene valores de diferencia que representan bordes en la imagen original. Este proceso imparte una apariencia en relieve a la imagen. 
Detector de objetos: Modelo de detección de objetos que tiene como objetivo localizar e identificar un objeto en una sola imagen.
               
               
                 
9.- DESCRIPCIÓN DE PRERREQUISITOS Y CONFIGURACIÓN

Para poder ingresar al simulador y revisar la simulación de la cámara de la raspberry ingresamos al siguiente link:

http://www.brainbox-demo.de/circuit/?shared=5eQD@Ogef.brain se nos abrirá directamente la simulación.

En el caso que nos pidiera usuario y contraseña ingresamos estos datos:

Usuario: Digitales

Clave: h5xCbP9V4

Y nos dirigimos al apartado de proyectos guardados:

![alt text](https://github.com/Proyecto-Digitales/INFORME-N.3/blob/master/Img/Manual1.png)

Y elegimos el archivo de nombre raspberry.

![alt text](https://github.com/Proyecto-Digitales/INFORME-N.3/blob/master/Img/Manual2.png)


10.APORTACIONES

En este apartado realizaremos un ejemplo un poco más interactivo en el que revisaremos las dos filas de pines que lleva consigo la raspberry y las usaremos para poder controlar el encendido y apagado de leds.
Para ello utilizamos una raspberry modelo B.


![alt text](https://github.com/Proyecto-Digitales/INFORME-N.3/blob/master/Img/Ap1.png)

Ahora obervamos la distribucion de pines de la raspberry:

![alt text](https://github.com/Proyecto-Digitales/INFORME-N.3/blob/master/Img/Ap2.png)

Para nuestro circuito queremos encender los cuatro leds asi que nuestro diseño quedo asi:


![alt text](https://github.com/Proyecto-Digitales/INFORME-N.3/blob/master/Img/Ap3.png)


Pero el circuito lo concetaremos en el proto asi que tenemos el siguiente esquem:


![alt text](https://github.com/Proyecto-Digitales/INFORME-N.3/blob/master/Img/Ap4.png)

Ahora procedemos a programar en python desde la raspberry para poder controlar el encendido de los leds.
La raspberry cuenta con el sistema operativo Raspbian el cual viene incluido python 3.
Expliacaion del cogido:


![alt text](https://github.com/Proyecto-Digitales/INFORME-N.3/blob/master/Img/Ap5.PNG)

![alt text](https://github.com/Proyecto-Digitales/INFORME-N.3/blob/master/Img/Ap6.PNG)

Ahora armamos nuestro circuito y conectamos a nuestra raspberry.

![alt text](https://github.com/Proyecto-Digitales/INFORME-N.3/blob/master/Img/Ap7.jpg)

Abrimos el terminal de raspbian y ejecutamos nuestro programa:

![alt text](https://github.com/Proyecto-Digitales/INFORME-N.3/blob/master/Img/Ap8.jpg)

Y observamos como comienzan a encenderse los leds:

![alt text](https://github.com/Proyecto-Digitales/INFORME-N.3/blob/master/Img/Ap9.jpg)


11.CONCLUSIONES

•	Entender cómo se distribuyen los diferentes pines o puertos tanto de salida y para qué sirve cada uno resulta muy sencillo. Existen diversos artículos en el internet que lo explican detalladamente y de una manera interactiva, lo cual facilita el proceso de entendimiento para principiantes. 


•	El simulador BrainBox trabaja con dispositivos programados para poder simular circuitos digitales, en el apartado de la raspberry no cuenta con gran variedad en el caso de periféricos, pero los que se encuentran ya en uso trabajan mediante bloques, lo cual resulta interactivo y facilita el aprendizaje a principiantes.


•	Para nuestra aportación en físico observamos que las técnicas de programación en Python pueden ser muy simples o muy sofisticadas (por ejemplo, con la programación orientada a objetos). En este proyecto se trató de reducir la complejidad para ser lo más didácticos posibles. Python, Raspberry y Linux son argumentos muy extensos sobre los cuales pueden encontrar toneladas de artículos en Internet y también tantos libros.



12.RECOMENDACIONES

•	Es importante conocer la estructura de hardware de la raspberry pi, para evitar daños en la realización de proyectos.

•	Se recomienda tener conocimientos en programación de lenguaje Python para poder empezar a trabajar en la raspberry. 

•	Es recomendable al instalar un sistema operativo en la raspberry, contar con un teclado y mouse con conexión usb o inalámbricos. 

•	Es preciso planificar un cronograma con diagramas de Grant en las diferentes aplicaciones que existen y para el desarrollo se recomienda el software Project. 


13.CRONOGRAMA

![alt text](https://github.com/Proyecto-Digitales/INFORME-N.3/blob/master/Img/Cronograma.PNG)


14.BIBLIOGRAFÍA

Alulema, D. (2020). Circuitos Digitales. Quito, Ecuador.

Floyd, T. (2006). Fundamentos de sistemas digitales. Madrid: Pearson.

Ricoy, A. (14 de Junio de 2020). Appinventor en español. Obtenido de https://sites.google.com/site/contadorasincrono/flipflop

Siliceo, R. (2018). Algoritmo de las operaciones aritmeticas aplicadas a los codigos binarios, octal, hexadecimal y BCD con sus respectivas conversiones. Ciudad de Mexico.



15.ANEXOS

15.1 MANUAL DE USUARIO

Una vez abierta la simulación, la podemos simular y observar los diferentes filtros que nos ofrece el simulador, los cuales podemos programar en la raspberry y utilizar las diferentes librerías que nos ayudan a usar dichos filtros. 

Para poder variar los datos y utilizar otra cámar IP nos dirigimos a la siguiente página:

http://insecam.org/en/bycountry/EC/

![alt text](https://github.com/Proyecto-Digitales/INFORME-N.3/blob/master/Img/Manual3.png)

En esta pagina podremos escoger otra dirección IP de cualquier cámara publica, siempre y cuando se transmita en formato mpjeg.

![alt text](https://github.com/Proyecto-Digitales/INFORME-N.3/blob/master/Img/Manual4.png)

Debemos presionar en configuración y podremos pegar el link con una nueva dirección IP.

![alt text](https://github.com/Proyecto-Digitales/INFORME-N.3/blob/master/Img/Manual5.png)


15.2 HOJAS TÉCNICAS

Guía del simulador Brainbox

https://github.com/freegroup/brainbox

Raspberry model B

https://github.com/Proyecto-Digitales/INFORME-N.3/blob/master/Hojas%20tecnicas/Hoja_tecnica_raspberry.pdf
