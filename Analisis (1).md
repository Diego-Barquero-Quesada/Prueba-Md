# Analisis del proyecto
## Descripcion Genral
El proyecto consiste en en crear una red de comunicacion entre diferentes maquinas la cual va a permitir que las maquinas puedan tanto enviar mensajes a las demas maquinas que se encunetran en la red o recibir mensajes. Las maquinas van a estar conectadas mediante un protocolo demonidao UDP(User Datagram Protocol) el cual es un protocolo para el itercambio de mensajes de minimo nivel, en otras palabras es facil de implementar.Cuando se inicaliza una nueva maquina esta va a ejecutar un proceso secundario el cual va a ser el encargado de leer unos archivos que van a describir caracteristicas de la respectiva maquina como el numero de identificacion,el numero de direccion ip y a cuales otras maquinas estan conectadas la misma.También la maquina va a ejecutar un servidor web el cual va a ser el encargado de manejar los mensajes que se van a enviar o los que se reciben. Los usuarios van a ser los encargados de generar los mensajes y escoger sus destinatarios,estos mediante el uso de un navegador web van a poder establecer una conexion con el servirdor web para interactuar on las maquinas conectadas en la red.
## Analisis Fase 1
En la primera fase se va a contruir la estructura basica del red, se va a contruir maquinas que sean capaces de arrancar el proceso secundario para obtener sus caracteristicas y ademas van a inicializar el servidor web asi como tener una conexion basica con las otras maquinas.Las maquinas solo van a ser capaces de comunicarse con sus vecinos directos, en otras palabras con los cuales tengan una conexion directamente.En esta primera fase no se van a redireccionar los mensajes en el caso de que una maquina reciba un mensaje que no es para ella el mensaje se va a dscartar y se va a mostrar una alerta.

## Linea temporal

![Linea temporal](temporal.svg)

En la imagen se aprecia como se ejecutan los procesos,primero se inicializa la maquina principal la cual es determinada por el color verde y después se ejecuta el proceso secundario el cual lee los rachivos para indicarle las caracteristicasa su respectiva maquina el cual esta representado por el color amarillo.Luego se inicializa el servidor web el cual es el representado con la flecha azul,este es el que permite el intercambio de mensajes y al final se realizan las conexiones con los vecinos de la maquina.

## Ejemplo de conexión de la red
![Ejemplo de conexión](Red.svg)

La imagen muestra un ejemplo de como seria la conexión de red entre las computadoras.




## Dudas sobre el proyecto
¿En las siguiente fases se va a cambiar el protocolo?

¿Por que el nodo verde no puede leer los archivos el mismo?
