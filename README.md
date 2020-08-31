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

![alt text](https://github.com/Proyecto-Digitales/INFORME-N.2/blob/master/Img/diagrama1.jpg)

•Diagramas UML. (casos de uso-clase)

![alt text](https://github.com/Proyecto-Digitales/INFORME-N.2/blob/master/Img/diagrama2.jpg)

•Diagramas eléctricos.

![alt text](https://github.com/Proyecto-Digitales/INFORME-N.2/blob/master/Img/diagrama3.jpg)


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

Este punto hace referencia a las variables que se emplean dentro de un programa, las cuales deben ser indicadas en la captura de una pantalla si son componentes visuales o especificados en una taba sin no son visibles en una interface. Se debe hacer referencia al tipo y la función que desempeñan en la aplicación.


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

                
                 
9.- DESCRIPCIÓN DE PRERREQUISITOS Y CONFIGURACIÓN

EL diseño de nuestro contador asincróno de 4 bits se lo realizó mediante el uso de flip flops tipo D. Es por ello que se tomó en cuenta la revisión de nuestro circuito integrado, en este caso es el modelo 74HC74, el cual presentamos un fragmento a continuación:

![alt text](https://github.com/Proyecto-Digitales/INFORME-N.2/blob/master/Img/Data1.PNG)


Es necesario que el usuario revise el datasheet de todos los circuitos integrados utilizados para que tenga una idea de que voltajes o corrientes soportan cada integrado, ademas de poder reconocer cada pin y cual es su función.
En el datasheet podemos obervar todas las especificaciones que se tomó en cuenta en el diseño, todo esto con el objetivo de no mostrar errores en la simulación del circuito, y tomando en cuenta a una posible implementación con integrados reales en un futuro,

Si el ususario desea comprobar el diseño del circuito lo puede hacer abriendo el archivo de la simulación en proteus o entrando a la plataforma Tinkercad en la cual se encuentra guardado el diseño implementado, tomando en cuenta que no prodrá modificar ninguna parte del circuito ya que ello conllevaria a fallas del circuito.

Nota: Es necesario tener instalado la versión 8.9 de proteus ya que si se desea abrir la simulación en versiones antiguas puede ocurrir errores o no abrir el archivo.

10.APORTACIONES

Conversión de código binario de cuatro (4) bits a BCD.
Al tener cuatro bits es posible manejar quince (15) combinaciones de entrada e igual número de combinaciones de salida. La tabla de valores para las posibles combinaciones es la siguiente:


![alt text](https://github.com/Proyecto-Digitales/INFORME-N.2/blob/master/Img/Binario%20a%20BCD.PNG)

Mediante estas tablas es posible observar que los valores de las salidas son iguales hasta el número nueve (9) decimal y de ahí en adelante el código de salida aparece incrementado en seis (6) decimal respecto al código de entrada. Dado lo anterior es posible concebir un sumador que reciba como entradas A los valores del código binario y como entradas B el número seis (6) en binario (0 1 1 0) pero solo cuando la salida B4 tenga un valor de uno (1). Para obtener la expresión que brinde esta posibilidad se realizó el mapa de Karnaught para la salida B4, con el siguiente resultado:

![alt text](https://github.com/Proyecto-Digitales/INFORME-N.2/blob/master/Img/Karnauth.PNG)

Por lo tanto, se obtiene para B4 la siguiente expresión:

B4 = A3A2 + A3A1 = A3(A2 + A1)

El resultado de esta implementación se llevará a las entradas B3 y B2 del sumador con el fin de obtener el resultado deseado.

Nota: Es necesario recordar que en la anterior descripción no tiene significado el hecho de no tener una secuencia consecutiva de valores. Así mismo en los valores de las entradas A serán ubicados los valores de salida de cada FF.

“Decodificación” y presentación del resultado.
Cada una de las salidas del sumador deben ser las entradas del decodificador/manejador que en este caso es el circuito 4511. A su vez este circuito arroja las salidas a, b, c, d, e, f  y g  a nivel alto que representan los siete (7) segmentos de un Display y específicamente uno de cátodo común. El Display utilizado es de la serie 5161 que tiene la siguiente distribución:

![alt text](https://github.com/Proyecto-Digitales/INFORME-N.2/blob/master/Img/display.PNG)

Simulación.
Para llevar a cabo la simulación de la implementación del circuito se utilizó la herramienta proteus. Como se muestra a continuación:

![alt text](https://github.com/Proyecto-Digitales/INFORME-N.2/blob/master/Img/Aporte1.png)


Para la demostración también se implemento en la plataforma Tinkercad como se muestra a continuación:


![alt text](https://github.com/Proyecto-Digitales/INFORME-N.2/blob/master/Img/aporte2.png)





11.CONCLUSIONES

•	Para la implementación en primera instancia se realizó el análisis de la secuencia de números asignada y se obtuvieron las expresiones necesarias para llevar a cabo la implementación del contador en código binario. Luego se implementó un circuito que ya era conocido como lo es el conversor de código binario a BCD y por último se realizó una actividad conocida como es la decodificación y posterior visualización en Displays de siete segmentos.

•	Teniendo en cuenta la investigación que se realizó y los resultados obtenidos teóricamente y en prácticamente podemos decir que una de la característica principal de los flip flop asíncronos, es que no comparten toda la misma entrada de reloj, algo muy importante ya que no cambian todos de estado al mismo tiempo. 


•	En la realización de la simulación se pudo ratificar que los tiempos de retardo en la propagación de datos entre un FF y otro que se presentaban en la implementación asíncrona se vieron disminuidos y que éstos no se presentaban en secuencias de 30ns por cada FF sino que el retraso de 30ns ocurre una vez en cada cambio de estado.

•El circuito se lo verificó mediante la implementación en el simulador proteus y el lab virtual Tinkercad, lo que nos indicó que la combinación de integrados de tegnología Cmos con TTL no trabajan como se esperaria que trabajen. 



12.RECOMENDACIONES

•	Es importante conocer cuál es la lógica de funcionamiento de los flip flops tipo D para futuros diseños. 

•	Se recomienda no mezclar integrados de tecnología TTL con tecnología Cmos ya que sus diseños admiten diferentes valores de voltajes y corriente, en este diseño de lo realizo debido a la escasez de modelos de integrados en la plataforma de Tinkercad. 

•	Se recomienda tener conocimientos previos sobre contadores y sus tablas de verdad para futuros diseños. 

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

Para poder usar el contador sincrónico se debe tener instalado si es posible la versión más actual de proteus.
Abriremos el archivo de la simulación

![alt text](https://github.com/Proyecto-Digitales/INFORME-N.2/blob/master/Img/manual1.png)

Nos presenta la interfaz de usuario del simulador:

![alt text](https://github.com/Proyecto-Digitales/INFORME-N.2/blob/master/Img/manual2.png)

Procedemo a realizar la simulación hacuendo click en el botón de la parte inferior izquierda.

![alt text](https://github.com/Proyecto-Digitales/INFORME-N.2/blob/master/Img/manual3.png)


Nota: tomar en cuenta que no se debe cambiar la frecuencia de la entrada de reloj. Ni cambiar el voltaje de entrada Vcc ya que podemos quemar los integrados.

Si queremos usar la implementación en tinkercad procederemos a entrar al siguiente link:

https://www.tinkercad.com/things/jxkNseHqJ4V-contador-asincronico/editel?sharecode=qnTRplA-JvCfeY6Auv5toNln4Gi4wd6hVyGVvV7Ki40

![alt text](https://github.com/Proyecto-Digitales/INFORME-N.2/blob/master/Img/manual4.png)


Nos presenta la interfaz de usuario

Ahora procedemos a simular para observar nuestro circuito:

![alt text](https://github.com/Proyecto-Digitales/INFORME-N.2/blob/master/Img/manual5.PNG)

Nota: tomar en cuenta que es debido registrarse antes en la plataforma Tinkercad para poder tener acceso, no se debe cambiar la frecuencia de la entrada de reloj. Ni cambiar el voltaje de entrada Vcc ya que podemos quemar los integrados. Evitar mover las conexiones ya que dañaría el diseño.


15.2 HOJAS TÉCNICAS

Datasheet 74HC293

https://github.com/Proyecto-Digitales/INFORME-N.2/blob/master/Hojas%20tecnicas/Datasheet74283.pdf

Datasheet 74HC32

https://github.com/Proyecto-Digitales/INFORME-N.2/blob/master/Hojas%20tecnicas/Datasheet7432.pdf

Datasheet 74HC74

https://github.com/Proyecto-Digitales/INFORME-N.2/blob/master/Hojas%20tecnicas/Datasheet7474.pdf

Datasheet 74HC08

https://github.com/Proyecto-Digitales/INFORME-N.2/blob/master/Hojas%20tecnicas/datasheet7408.pdf

Datasheet 4511

https://github.com/Proyecto-Digitales/INFORME-N.2/blob/master/Hojas%20tecnicas/Datasheetcd4511b.pdf
