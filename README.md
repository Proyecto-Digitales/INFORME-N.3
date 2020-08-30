                                 CONTADOR ASINCRONICO MEDIANTE LA IMPLEMENTACION DE FIP FLOPS TIPO D


1.PLANTEAMIENTO DEL PROBLEMA

Una de las aplicaciones de los flip flops son los contadores asincrónicos los cuales pueden ser implementados mediante el uso de flip flops tipo D, para ello deben estar conectados en cascada, así obtendremos
en cada salida de los flip flops un bit del conteo, esta implementación planea como reto principal la visualización de una secuencia no consecutiva de números decimales en dos Displays, para ello se deberá 
diseñar un circuito el cual nos permita observar en dos displays de 7 segmentos el conteo de 0 a 15,. Al añadir dicho circuito ¿Afectara el funcionamiento de nuestro contador?


2.OBJETIVOS

Objetivo general

-Implementar y comprobar el funcionamiento de un circuito contador ascendente asíncrono, implementado con flip-flop tipo D.

Objetivo específicos

-Investigar en funcionamiento de flip flops tipo D.

-Comprobar el funcionamiento del diseño del contador mediante la simulación en proteus e implementada en Tinkercad (laboratorio virtual).

-Convertir las salidas de cada flip flop de código BCD a decimal y mostrarlo en dos displays de 7 segmentos.


3.ESTADO DEL ARTE

El circuito asincrónico realizado por los Ingenieros Rubén González; Marco Bardón y José Antonio Salcines; primero nos define que es un contador de la siguiente manera: 
Un contador es un circuito en el que sus salidas siguen una secuencia fija que cuando acaba vuelve a empezar, o circuitos que reciben sus datos en forma serial ordenados en distintos intervalos de tiempo. Los pulsos de entrada pueden ser pulsos de reloj u originarse en una fuente externa y pueden ocurrir a intervalos de tiempo fijos o aleatorios. El número de salidas limita el máximo número que se puede contar. En nuestro estudio y para nuestro análisis se estudiará los contadores asincrónicos que en el contexto de los autores nos explica que son: Las salidas de cada flip-flop sirven de entrada CP para disparar otro flip-flop. El primer biestable tendrá una entrada de tipo asíncrono, es decir que se acertará de forma aleatoria y cuando lo haga el circuito realizará una cuenta. El resto del tiempo, los flip-flops no cambiarán su estado presente. En su diseño ellos pusieron como ejemplo lo siguiente; un contador asíncrono modulo 10: y los pasos para resolver son los siguientes. Paso 1: elegir un contador ascendente de 4 bits (de 0 a 15); paso 2: Detectar el 10 (1010 en binario) con una compuerta NAND y como ultimo paso Reset de todos los biestables cuando ocurra la detección.
(González, Bardón, & Salcines. (2019). Contadores. Manzanom. https://personales.unican.es/manzanom/Planantiguo/EDigitalI/CONTG5.pdf)

El sitio web Wilaeba Electrónica nos dan muchos puntos a tomar en cuenta además de ejemplos para lograr trabajar con distintos flip-flops incluido con el flip-flop que se desea trabajar que es el 74hc74. Los puntos a tomar que nos otorga este sitio web para nuestros diseños son los siguientes puntos: 
- Un contador asíncrono tiene como principal característica que cada flip flop que lo compone tiene diferente señal de reloj (clk).
- El temporizador 555 está configurado a una frecuencia de 1 Hz, es decir que el contador aumentará de valor cada segundo.
- Los integrados usados para los contadores con flip flops JK serán el cd4027 y 74hc112, y para los contadores con flip flops D serán el cd4013 y el 74hc74. Los integrados cd40 son tecnología cmos, y los integrados 74hc son tecnología ttl. Wilaeba Electrónica. (2017, 24 septiembre). Contador asíncrono de 4 bits ascendente.https://wilaebaelectronica.blogspot.com/2017/08/contador-asincrono-de-4-bits-ascendente.html

4.MARCO TEÓRICO


![alt text](https://github.com/Proyecto-Digitales/INFORME-N.2/blob/master/Img/marco%20teorico%201.png)

![alt text](https://github.com/Proyecto-Digitales/INFORME-N.2/blob/master/Img/marco%20teorico%203.png)

![alt text](https://github.com/Proyecto-Digitales/INFORME-N.2/blob/master/Img/marco%20teorico%202.png)

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

-Simulador Proteus version 8.9.

-Laboratorio virtual Tinkercad.


7.MAPA DE VARIABLES

Este punto hace referencia a las variables que se emplean dentro de un programa, las cuales deben ser indicadas en la captura de una pantalla si son componentes visuales o especificados en una taba sin no son visibles en una interface. Se debe hacer referencia al tipo y la función que desempeñan en la aplicación.


8.EXPLICACIÓN DEL DISEÑO

Contador en código binario.

En esta etapa es necesario indicar que se utilizará un generador de señal de reloj (CLK) para los FLIP FLOP (FF), de igual forma usaremos una frecuencia aproximada de 1 Hz dados los valores de las resistencias R1 y R2 (330 Ohmios ).
Tomaremos en cuenta que:
- Un contador asíncrono tiene como principal característica que cada flip flop que lo compone tiene diferente señal de reloj (clk).
- El temporizador está configurado a una frecuencia de 1 Hz, es decir que el contador aumentará de valor cada segundo.
- Los integrados usados para los contadores con flip flops D serán el CD4013 y el 74hHC74. En nuestro caso usaremos el integrado 74HC74.

Para empezar nuestro análisis tendremos que plantear los estados, en este caso de 4 bits será de 0000 a 1111 es decir un conteo de de 0 a 15.

En esta parte vemos como se pasa de un estado al otro nuestra cuenta, lo que nos indica que las salidas de nuestros fip flops tendran una salida de 0 o 1. 

![alt text](https://github.com/Proyecto-Digitales/INFORME-N.2/blob/master/Img/Tablas%20de%20transicion.PNG)

                     Tabla de verdad de cambio de estados 

Tabla de excitación del flip flop D

Ya que estamos usando un flip flop tipo D, tenemos la siguiente tabla, la cual nos muestra la respuesta a los cambios de estado que sufre el flip flop.

![alt text](https://github.com/Proyecto-Digitales/INFORME-N.2/blob/master/Img/Tabla%20de%20exitacion.PNG)

          Tabla de exitacion de un flip flop tipo D
 
 Analizando el cambio de estado de cada columna tenemos el siguiente diagrama:
 
 ![alt text](https://github.com/Proyecto-Digitales/INFORME-N.2/blob/master/Img/Cambio%20de%20estados.png)
 
Una vez analisado los cambios de estado procedemos a implementar el circuito en el simulador proteus, para implementar nuestro circuito debemos tomar en cuenta lo siguiente:

-Necesitaremos 4 flip flops, uno por cada bit requerido en este caso seran 4 flip flops, seguido conectaremos la señal de reloj a nuestro primer flip flop, la salida de este significa el bit menos significativo de nuestro conteo.

-Cada entrada de reset y clear deberá estar conectada a Vcc, ya que se activan en bajo y nos las utilizaremos.

-Conectamos cada terminal D a Q’ y también a los clock’s. Con esto haremos que la salida anterior se duplique hacia la entrada del siguiente flip flop.

Implementación en proteus:

![alt text](https://github.com/Proyecto-Digitales/INFORME-N.2/blob/master/Img/dise%C3%B1o%201.PNG)

                            Simulación en proteus
                  
Ahora veremos la implementación en tinkercad                 
                  
![alt text](https://github.com/Proyecto-Digitales/INFORME-N.2/blob/master/Img/dise%C3%B1o%202.png)

                                                                  Simulación en Tinkercad
                
                 
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

![alt text](https://github.com/Proyecto-Digitales/INFORME-N.2/blob/master/Img/Cronograma.PNG)


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
