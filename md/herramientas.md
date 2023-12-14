## **PROCESOS**

* **ps**: Muestra información de los procesos activos.

* **top**: Proporciona una visión en tiempo real de los procesos que consumen más recursos,como la CPU y la memoria.

* **htop**: Similar a top, pero con una interfaz más visual y funciones adicionales, como la capacidad de desplazarse y filtrar procesos de manera más intuitiva.

* **atop**: Registra e informa de la actividad de todos los procesos del servidor. Guarda estadísticas del sistema. Empieza a tomar datos desde el momento que se instala. systemctl status atop. Fichero de configuracion /etc/default/atop. Dentro de default LOGINTERVAL=600 (cada tiempo que recoge datos en segundos). /var/log/atop (atop -r /var/log/atop/atop_[fecha]).

## **MEMORIA, ESPACIO Y RENDIMIENTO DEL DISCO**

* **free**: Muestra la cantidad de memoria libre y utilizada en el sistema.

* **df**: Muestra el espacio utilizado y disponible en los sistemas de archivos montados.

* **du**: Muestra el espacio ocupado por un fichero o directorio.

* **iostat**: Se utiliza para rastrear los problemas de rendimiento de los dispositivos de almacenamiento.

## **TRÁFICO DE LA RED**

* **tcpdump**: Analiza el tráfico que circula por la red.
  
* **tcptrack**: Nos muestra las conexiones establecidas, su origen, destino, estado, el tiempo de iddle y la velocidad de transferencia.
  
* **iptraf**: Intercepta paquetes en la red y muestra información sobre el tráfico.
  
* **bandwidthd**: una herramienta específica de monitorización del ancho de banda

## **PUERTOS**

* **netstat (ss)**: Muestra las conexiones activas de una computadora, tanto entrantes como salientes.