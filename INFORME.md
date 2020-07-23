# Informe

### Tutorial para simular en línea Raspberry Pi a Azure IoT Hub.
**1. PLANTEAMIENTO DEL PROBLEMA**

El avance de la tecnología ha tenido un crecimiento enorme de tal forma que siempre se debe seguir aprendiendo y a su vez seguir experimentando. Un ejemplo de ello es la virtualización de objetos, es decir, diseñar artefactos en una computadora y dotar las mismas características y funcionalidades tal como lo es un objeto físico. Al final, estos elementos se interconectan entre sí y se obtienen resultados muy cercanos a los reales. La demanda de produción, los precios de comercialización y el tiempo de uso de ciertos productos son las razones que motivaron a la implementación por medio de Software. La internet se ha convertido parte de nuestra rutina de tal forma que su uso se ha hecho más eficiente y se han añadido más funcionalidades, siendo que la conexión de red no solo se estrablece de computadora a computadora, sino con otros objetos como un interruptor, un automóvil. Gracias a ello, se ha facilitado la adquisición del software o sin necesidad de adquirirlo se pueden realizar las simulaciones en línea. La plataforma en la nube a utilizarse es Microsoft con lo que se creará un servicio IoT (Internet of Things) para simular la conexión con un Rasperry PI virtual.

**2. OBJETIVOS**

2.1 Objetivo general

Desarrollar un tutorial basado en la conexión del ordenador, Rasperry PI, por medio del proveedor de servicios de IoT de Microsoft Azure para los estudiantes de Tercer nivel de la carrera de Ingeniería en Telecomunicaciones, de la Universidad de las Fuerzas Armadas ESPE, en la sede Sangolquí, en el periodo mayo – septiembre de 2020.

2.2 Objetivos Específicos

Crear un servicio IoT en Microsoft Azure.

Mostrar las caracteristicas principales de comunicación de una Rasperry PI.

Grabar un videotutorial mostrando la instancia realizada.

**3. ESTADO DEL ARTE**

*Un estudio sobre la posibilidad de usar Raspberry Pi como un servidor de consola para el acceso remoto a dispositivos en entornos de aprendizaje virtual*

Diyana Kyuchukova, Georgi Hristov, Plamen Zahariev y Svilen Borisov, miembros del Department of Telecommunications of University of Ruse “Angel Kanchev” en Bulgaria; manifiestan su principal preocupación en el desarrollo de los laboratorios virtuales debido a que no se han adaptado a las necesidades de aprendizaje de los estudiantes, siendo susceptible a cometer errores en el manejo de la interfaz gráfica provocando una pérdida en la conexión del acceso remoto. Las conexiones se dan por el protocolo Telnet/SSH pero requieren al menos uns interfaz activa y un buen conociminto en el manejo de redes ya que es susceptible a errores. Así que para solucionar el problema, los Rasberry PI serán configurados como servidores de consola. Una mejor solución para proporcionar acceso remoto a dispositivos de laboratorio especializados es utilizar un servidor de consola de middleware, pero se accede indirectamente a través de una interfaz gráfica de usuario (GUI). Así que, el laboratorio desarrollado por los autores es un completo entorno de aprendizaje virtual que proporciona los materiales de aprendizaje más recientes, video tutoriales, herramientas interactivas y recursos en el área de las redes de comunicación locales y globales, desarrollando de forma simultánea ejercicios prácticos en dispositivos reales de forma remota. Con la configuración de los puertos seriales, siendo puertos GPIO o USB, se puede establecer un acceso directo a los dispositivos utilizando el shell del sistema operativo Raspbian. Si se desea un número mayuor de puertos de conexión se necesitaran más de esos dispositivos. (Kyuchukova, Hristov, Zahariev, & Borisov, 2015).

*Raspberry PI como un servidor de video*

Fatma Salih y Mysoon Omer, miembros del departamento de Computer Engineering of University of GeziraWad en Madani, Sudan, utilizaran una Raspberry PI para que sea un servidor de transmisión de audio y video en tiempo real. El video se captura a través del puerto del módulo de cámara Raspberry PI y se comprime y envía utilizando un estándar especial que aplica HTTP (Protocolo de Transferencia de Hipertexto) para que pueda recibirse desde la red, mientras que, el audio se captura con un micrófono y se envía con el protocolo de transmisión en tiempo real (RTP). Primero, la Raspberry pi se conecta a la red. Despues, la entrada de audio comienza a funcionar. Luego, e audio del Raspberry PI se procesa y es enviado a los clientes. Entonces, la conexión de los dispositivos de video tiene lugar y por último, la cámara comienza a capturar y envía la transmisión de video en vivo. La parte de la programación es controlado por la ventana de comandos del sistema operativo propio de la Raspberry PI, Raspian. (Salih & Mysoon Omer, 2018).

*Evaluación de QoS de VPN en dispositivos Raspberry Pi a través de red inalámbrica*

Caldas-Calle, Jara, Huerta y Gallegos, miembros del club de la IEEE de la Universidad Politécnica Salesiana, presentan la evaluación de los parámetros de QoS de VPN a través de una WLAN, utilizando los modelos Raspberry Pi: Pi Zero v1.3 (RPZ), Modelo B Rev 2 (RPB), Pi 2 Modelo B v1.1 (RP2) y Pi3 Modelo B (RP3), y analizaron los parámetros de QoS con diferentes condiciones de tráfico y el consumo de CPU en la VPN. Últimamente las redes WLAN (Redes de área local inalámbricas) se han vuelto populares debido a su disponibilidad y a su rápida y sencilla conexión. Sin embargo, está propensa a ataques por lo que han optado al uso de la VPN (Red Privada Virtual), siendo más segura en su navegación. En ella también existen desventajas como la sobrecarga de VPN reflejada en efectos en el rendimiento, la latencia, la tasa de pérdida de tramas, entre otros parámetros, que afectan la calidad de servicio (QoS) de la red. Diferentes investigadores estudiaron el comportamiento de los parámetros de QoS en una VPN a través de una red inalámbrica y los resultados muestran que el rendimiento más alto es para RP3 y el más bajo para RPB. Los paquetes con un tamaño superior al punto de fragmentación sufren una disminución de la QoS, debido a la necesidad de fragmentar los paquetes. La potencia de la CPU de cada modelo de Raspberry Pi es un factor importante que afecta los parámetros de QoS de una VPN inalámbrica. Introducir VPN para asegurar la comunicación implica un proceso más complejo en la comunicación que requiere más del hardware. (Caldas-Calle, Jara, Huerta & Gallegos, 2017).

**4. MARCO TEÓRICO**

4.1. Raspberry PI

Raspberry Pi es un ordenador constituido en una placa dek tamaño de una libreta de bajo costo desarrollado en el Reino Unido por la Raspberry Pi Foundation, con el objetivo de estimular la enseñanza de informática en las escuelas enfocado en estudiantes, sobretodo en niños. Se puede utilizar como cualquier ordenador y se puede implementar diferentes dispositivos externos como un teclado, un ratón y dispositivos de audio, vendiendose por separado.  

![](https://github.com/deyder73/Simulador-en-l-nea-de-Raspberry-Pi-a-Azure-IoT-Hub./blob/master/img/WhatsApp%20Image%202020-07-23%20at%2009.03.22.jpeg)

La Raspberry Pi fue diseñada para ejecutar programas simples, desde la edición de documentos de texto hasta la implementación de juegos de video de los años 90. Gracias a su arquitectura y a su software libre, se puede controlar otros dispositivos por medio de la microcomputadora, siendo eficiente para aprender domótica. La arquitectura de este producto permite que no solo funcione en nmodo software, sino también controlar dispositivos electrónicos como un conjunto de LEDs, pantalla LCD, sensores de luz y movimiento hasta cámaras y micrófonos.

![](https://github.com/deyder73/Simulador-en-l-nea-de-Raspberry-Pi-a-Azure-IoT-Hub./blob/master/img/WhatsApp%20Image%202020-07-23%20at%2009.03.28.jpeg)

4.1.1. Modelos

Los siguientes modelos desarrollados hasta la actualidad son los siguientes:
- Raspberry Pi 1 modelo A (descontinuada): fue el primer modelo de Raspberry, donde su procesador fue un Broadcom BCM2835, Single-Core a 700MHz, RAM de 256 MB y una gráfica Broadcom VideoCore IV.
- Raspberry Pi 1 modelo B (descontinuada) y B+: sus mejoras con respecto al primet modelo es el doble de memoria RAM, un puerto USB más y un conector Ethernet (RJ-45)
- Raspberry Pi 2 modelo B: el procesador se sustituye por uno de la misma marca, pero de modelo BCM2836; pasa de ser de un núcleo a cuatro, y de 700MHz a 900MHz. Dobla la cantidad de memoria RAM con respecto al modelo 1B. También incluye 40 pines GPIO y suprime la conexión RCA.
- Raspberry Pi 3 modelo B: renueva procesador, una vez más de la compañía Broadcom, una vez más un Quad-Core, pero pasa de 900MHz a 1.20GHz. Incluyó de Wi-Fi y Bluetooth (4.1 Low Energy) sin necesidad de adaptadores.
- Raspberry Pi 3 modelo B+: cuenta con un nuevo procesador, pasando de tener 1.2Ghz a tener 1.4Ghz, y mejor conectividad, incorporando a doble banda a 2,4GHz y 5GHz, y su nuevo puerto Ethernet se triplica, pasa de 100 Mbits/s en el modelo anterior a 300 Mbits/s en el nuevo modelo, también cuenta con Bluetooth 4.2 (Low Energy).
- Raspberry Pi 3 modelo A+: cuenta con 512 MB de RAM (compartidos con la GPU VideoCore IV), un solo puerto USB y sin puerto de conexión de red por cable (RJ-45).
- Raspberry Pi 4 modelo B: se han cambiado los puertos HDMI de tamaño completo por dos puertos microHDMI. Cuenta con la capacidad de manejar dos pantallas 4K a 60 Hz. Se ha incluido por primera vez USB 3.0, y el puerto Ethernet ya no está limitado a 300 Mbps. Tiene un procesador Broadcom nuevo hasta tres veces más eficiente que el anterior.

![](https://github.com/deyder73/Simulador-en-l-nea-de-Raspberry-Pi-a-Azure-IoT-Hub./blob/master/img/WhatsApp%20Image%202020-07-23%20at%2009.03.36.jpeg)

4.1.2. Hardware

Su placa, de forma general, está constituido por los siguientes elementos:
- Un Chipset Broadcom BCM2835, que contiene un procesador central (CPU) ARM1176JZF-S a 700 MHz.
- Un Procesador gráfico (GPU) VideoCore IV
- Un módulo de 512 MB de memoria RAM
- Un conector de RJ45 conectado a un integrado lan9512 -jzx de SMSC que  conectividad a 10/100 Mbps
- Dos buses USB 2.0
- Una salida analógica de audio estéreo por Jack de 3.5 mm.
- Una Salida digital de video + audio HDMI
- Una salida analógica de video RCA
- Pines de entrada y salida de propósito general (GPIO)
- Conector de alimentación microUSB
- Lector de tarjetas SD

![](https://github.com/deyder73/Simulador-en-l-nea-de-Raspberry-Pi-a-Azure-IoT-Hub./blob/master/img/WhatsApp%20Image%202020-07-23%20at%2009.03.42.jpeg)

Además, se describen los accesorios que se venden por separado. Inclusive, algunos sirven para personalizar las placas.
- Cámara de vídeo: la dimensión actual del módulo son 25 x 20 x 9 mm. Para poder hacer uso de él, se tiene que activar en el menú raspi-config de Raspbian.108.
- Reloj: permite a cada dispositivo consultar la fecha, hora de arranque y luego cada cierto tiempo durante su funcionamiento, ya que los Raspberry Pi no poseen un reloj interno que conserve la hora y fecha al ser apagados.
- Periféricos
- Carcasas
- Controlador para Arduino

4.1.3. Software

Los sistemas operativos disponibles son:
- Raspbian
- Arch Linux
- RaspBMC
- Pidora 
- OpenELEC
- Windows 10

4.1.4. Descripción de uso

Para trabajar con un Raspberry Pi se requiere almacenamiento que en este caso específico debe ser una tarjeta de memoria SD o microSD, donde en ella deberá estár una copia del sistema operativo. Conecta tu teclado y ratón en los puertos USB de la Raspberry Pi, además de un cable de alimentación  que suministe como máximo "5[V]" y "3[A]". Una vez que la placa esté conectada a una fuente de alimentación, deberá iniciar sesión, donde usted escribira su nombre de usuario pi y contraseña raspberry. También puede luego cámbielas.

![](https://github.com/deyder73/Simulador-en-l-nea-de-Raspberry-Pi-a-Azure-IoT-Hub./blob/master/img/WhatsApp%20Image%202020-07-23%20at%2009.03.46.jpeg)

Una vez ingresada a la sesión, se encontrará con una colección de aplicaciones y herramientas, incluso una copia personalizada de Minecraft, para ayudar a empezar, incluyendo LibreOffice, el navegador Chromium y varias utilidades de programación. Adempas se dispone de la herramienta de configuración de la Raspberry Pi Configuration, raspi-config, recomendado para los usuarios recientes. Además se conectar tu Raspberry Pi a tu red local o directamente a Internet por medio de un cable Ethernet o por WiFi

4.2. Internet de las cosas (IoT)

Se describe como un sistema en la cual controla objetos reales por medio de internet. Esto se da gracias a los sistemas embebidos, donde ejecutan tareas específicas en sistemas complejos. Cada uno de estos objetos se consideran como dispositivos, cada uno con una IP específica donde puede ser accedido para que reciba instrucciones.

Hasta ahora, no ha existido un gran enfoque pero cada vez va creciendo, donde empresas orientadas al público en general están desarrollando sus implementaciones transformando los dispositivos manuales en automáticos. Adempas, estos objetos se los pueden virtualizar y muchas plataformas se han estado desarrollando para el diselo de sistemas, sobretodo plataformas que operan en la nube.

![](https://github.com/deyder73/Simulador-en-l-nea-de-Raspberry-Pi-a-Azure-IoT-Hub./blob/master/img/WhatsApp%20Image%202020-07-23%20at%2009.03.51.jpeg)

4.2.1. Plataformas IoT

Según Link-labs, una plataforma web integrada al Internet of Things (IoT) es el software que conecta hardware, puntos de acceso y redes de datos a lo que generalmente suele ser la aplicación de la que disfruta el usuario. Las propiedades de una verdadera plataforma Iot estpan descritas en 8 importantes bloques como:
1. Conectividad y normalización: con diferentes protocolos y diferentes formatos de datos en una interfaz de «software» garantiza la precisa transmisión de datos y la interacción con todos los dispositivos.
2. La gestión de dispositivos: asegura que todas las «cosas» conectadas están funcionando correctamente.
3. Base de datos: almacenamiento escalable de datos del dispositivo basados en la nube a un nuevo nivel en términos de volumen de datos, variedad, velocidad y veracidad.
4. Procesamiento y gestión de la acción: aporta datos basados en reglas de acción de evento-disparadores que permitan la ejecución de las acciones «inteligentes» basados en datos específicos del sensor.
5. Analítica: lleva a cabo una serie de análisis complejo de la agrupación de datos básicos y de aprendizaje automático.
6. Visualización: permite a los seres humanos observar las tendencias de cuadros de mando de visualización de datos, donde se retrata vívidamente a través de gráficos.
7. Herramientas adicionales: la IoT permiten a los desarrolladores de prototipos, probar y comercializar para visualizar, gestionar y controlar los dispositivos conectados.
8. Interfaces externas: se integran con los sistemas de 3ª parte y el resto del ancho de TI en los ecosistemas a través de una función de interfaces de programación de aplicaciones (API), kits de desarrollo de software (SDK), y puertas de enlace.

4.2.2. Azure IoT Hub

Según Microsoft, el servicio lo descirbe como un centro de mensajes central para la comunicación bidireccional entre su aplicación IoT y los dispositivos que administra. IoT Hub admite comunicaciones tanto del dispositivo a la nube como de la nube al dispositivo, además de múltiples patrones de mensajería, como telemetría de dispositivo a nube, carga de archivos desde dispositivos y métodos de solicitud-respuesta para controlar sus dispositivos desde la nube. El monitoreo de IoT Hub lo ayuda a mantener el estado de su solución al rastrear eventos como la creación de dispositivos, fallas de dispositivos y conexiones de dispositivos. Azure IoT Hub ofrece un back-end de solución hospedado en la nube para conectarse prácticamente a cualquier dispositivo. 

![](https://github.com/deyder73/Simulador-en-l-nea-de-Raspberry-Pi-a-Azure-IoT-Hub./blob/master/img/WhatsApp%20Image%202020-07-23%20at%2009.03.56.jpeg)

4.2.3. Raspberry Pi Azure IoT Online Simulator
Un simulador en línea de Raspberry Pi permite a los usuarios escribir código para controlar el hardware emulado. El simulador muestra un gráfico de un Raspberry Pi conectado a un sensor combinado de humedad, temperatura, presión y un LED rojo a través de una placa de prueba , una placa de enchufe que permite que los circuitos se conecten rápidamente. Este simulador está en 'vista previa' y es bastante rudimentario, lo que significa que la imagen incrustada del Pi es estática y el simulador se limita a interactuar con el sensor y el LED.

![](https://github.com/deyder73/Simulador-en-l-nea-de-Raspberry-Pi-a-Azure-IoT-Hub./blob/master/img/WhatsApp%20Image%202020-07-23%20at%2009.04.01.jpeg)

**5. EXPLICACIÓN DEL FUNCIONAMIENTO**

**6. DESCRIPCIÓN DE PRERREQUISITOS Y CONFIGURACIÓN**

**7.	CONCLUSIONES**

**8.	RECOMENDACIONES**

**9.	CRONOGRAMA**

**10.	BIBLIOGRAFÍA**

Kyuchukova, D., Hristov, G., Zahariev, P., & Borisov, S. (2015). A study on the possibility to use Raspberry Pi as a console server for remote access to devices in virtual learning environments. 2015 International Conference on Information Technology Based Higher Education and Training (ITHET).

Salih, F., & Mysoon Omer, S. A. (2018). Raspberry pi as a Video Server. 2018 International Conference on Computer, Control, Electrical, and Electronics Engineering (ICCCEEE). doi:10.1109/iccceee.2018.8515817 

Caldas-Calle, L., Jara, J., Huerta, M., & Gallegos, P. (2017). QoS evaluation of VPN in a Raspberry Pi devices over wireless network. 2017 International Caribbean Conference on Devices, Circuits and Systems (ICCDCS).

https://culturacion.com/raspberry-pi-que-es-caracteristicas-y-precios/

https://es.wikipedia.org/wiki/Raspberry_Pi

https://hipertextual.com/archivo/2014/10/internet-cosas/

https://docs.microsoft.com/en-us/azure/iot-hub/about-iot-hub

https://www.techrepublic.com/article/raspberry-pi-simulator-lets-you-start-tinkering-without-even-owning-a-pi/
