# Segundo Parcial Toria
## La capa Fisica
*HACE QUE A TRAVEZ DE UN VINCULO SE PUEDAN CONECTAR DOS EQUIPOS Y QUE PUEDAN TRANSMITIR DATOS  *
La comunicacion a nivel de la capa fisica entre dos equipos se realiza a travez de interases o buses digitales estandarizados.
La normalizacion permite intercomnectar diferentes equipos de diferentes fabricas.
Intenral o bus estandar: conjunto de normas mecanicas electricas o logicas que permiten que las señales digitales puedan ser transmitidas a travez de un vinculo fisico 

## Normalizacion de las Interfaces FIsicas
-**Mecanico:** Normalizacion en funcion de la forma y las caracteristicas de los materiales utilizados (conectores)
-**Electrico:** Normalizando el nivell electro, tensiones, impedancias, etc
-**Logico:** Los protocolos para detectar la señal de la linea, como sincronizar el bit, etc.

## Tipos de Transmicion
- **Simplex:** Tiene un solo sentido, desde la fuente al sumbidero, en donde uno es el receptor y el otro es el transmisor
- **SemiDuplex:** Tiene dos sentidos, pero no a la vez, seria como usar dos simplex opuestos, donde en un canal uno es la fuente y el otro el sumbidero (uno recive y el otro envia), y en el otro canala uno envia y el otro recive. (no es simultaneo, uno envia y el otro tiene que esperar a que llegue el mensaje para enviar otro).
- **Duplex:** En un unico canal se puede enviar y recivir informacion simultaneamente

## Modos de Transmision
- **En Serie:** Los bits fluyen en una secuenca.
- **En Paralelo:** Cada bits va en un canal diferente, y se presentan en el receptor al mismo tiempo (se requiere un reloj de sincronizacion)

# Interfaces y buses 
## En modo Paralelo
Aumenta la velocidad de Transmision en distancias cortas.

- **Interfaz ATA**: Interfaz en paralelo
- **Interfaz IEE1284 - Centronics:** Interfaz en paralelo, bidireccional, con velocidad mazima de 150 kbyte por segundo.

## En modo Serie
Son los mas eficientes hoy en dia, ya que lograron superar la velocidad de transmision que se venia logrando con los modos en paralelo

- **RS 232-TIA 232:** Esta normalizada por la UIT-T, se sigue usando en algunos equipos, su distnacia maxima es dde 15 metros, y la velocidad maxima de trasnferencia es de 20kbps, 2 usuarios como maximo (enlaces punto a punto)
- **V.24-V.35- M34**
- **V.21-X.21-X.26**: Transmision asimetrica y circuito desbalanceado
- **Interfas USB:**
- **IEEE-1394**

##### USB
Sus principales caracteristicas son:
	- Permite la conexion de distintos dispositivos.
	- Adaptado a distintas pliaciones
	- Interfaz estandarizasa (simple, rapida y economica)
	- Permite la conexion de dispositivos encendidos
	- Plug and Play (el sistema operativo lo detecta ni bien es conectado)
	- Bajo costo
	- Proporciona energia electrica (mando)

Soporta en tiempo real vos, audio y video
Protocolo mixto que trabaja en modo sincronico para la transferencia de datos y en modo asincronico para el envio de mensajes.
Longitud maxima de cables es de 3 a 5 metros 
Las versiones son compatibles entre ellas
Funciona en modo serie y el intercambio de datos es bidireccional

Tiene 4 pines, los cuales 2 son los mas importantes que son los de datos.
Utiliza un codigo NRZI para la transmision de paquetes.
**hub:** es un conector con varios púertos usb. Estos se pueden colocar hasta 5 niveles en cascada

*Nivel logico:*
	El USB tiene un unico controlador dentro del host (los dispositivos no pueden utilizar el bus a menos que su controlador en el host los autorise)
	El controlador permitira que los dispositivos se comuniquen de a uno a la vez

*Version USB 3.0*
Es compatible con las versiones anteriores
Mejora la velocidad maxima de transferencia
Proporciona mas potencia a los dispositivos conectados
Posee una arquitectura de Dual-Buss

##### Interfaz FireWire-IEEE 1394
Su principal ventaja es que no depende de un control centralizado (peer-to-pear), ya que no depende de un procesamiento mayor

Usado para la transferencia de datos en tiempo real de dispositivo multimedia, tales como videocamaras, audio y video.
La comunicacion no depende de un control centralizado
Es un modelo de protocolo *Peer-to-peer*
Puede soportar 64 dispositivos en una red
Soporta ambos modos, el sincronico y el asincronico.

(Similar a los USB, surguieron distintas normas, que aumentaban las velocidad y las prestaciones).

#### Diferencias entre USB y IEEE1394

| Caracteristicas            | USB     | IEEE1394 | 
|-------------------|-------------|---------------|
| Protocolo  | es protocolo maestro-esclavo    | es un protocolo peer-to-peer |
| Costo        |  simple y de muy bajo costo    | Complejo y de costo un poco elevado            | 
| Requisito Hardware         |  requiere un computador para el controlador    | No necesita un procesamiento mayor (no hay necesidad de conectar con un computador)           | 
|  Que dispositivos conecta|  teclados, mouse, impresoras, (dispositivos de baj a capacidad)  | discos rígidos, equipos de audio, filmadoras, equipos de video             | 
| Ancho de banda      | menor ancho de banda y mayor latencia  | mayor ancho de banda y menos latencia            | 
| Voltaje necesario     | 2.5W | 20W           | 

# SINCRONISMO
El receptor debe adquirir una señal de reloj para alienar los bits recibidos.
Es fundamental para que diferentes equipos intercambien  datos sin errores.
El tiempo es medido utilizando relojes atomicos.

