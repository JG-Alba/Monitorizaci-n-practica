## **tcpdump:** ## 
Analiza el tráfico que circula por la red.

```
- tcpdump -i eth0                                      Información sobre una tarjeta de red
- tcpdump -D                                           Ver un listado de las interfaces disponibles para capturar tráfico
- tcpdump -i eth0 -w trafico.log                       Capturar tráfico y enviar a un fichero de texto
- tcpdump -i eth0 [udp,tcp, icmp,...]                  Protocolo a capturar
- tcpdump -i eth0 tcp port 80                          Puerto a capturar
- tcpdump -i eth0 tcp port 80 and src 192.168.1.100    Host o IP de origen
- tcpdump -i eth0 tcp port 80 and dst 192.168.1.100    Host o IP de destino
- tcpdump -i eth0 -A                                   Mostrar el contenido de los paquetes en formato ASCII
- tcpdump -i eth0 -XX                                  Capturar paquetes en hexadecimal y ASCII
- tcpdump -i eth0 not icmp
- tcpdump -i eth0 not icmp and not tcp                 Capturar todo el tráfico excepto ciertas condiciones
- man tcpdump
- tcpdump 'dst 192.168.1.100 and (port http or https)'
- tcpdump -r archivo.log                              Leer captura de tráfico almacenada en un archivo
- 
```
---

## **tcptrack:** ##
Nos muestra las conexiones establecidas, su origen, destino, estado, el tiempo de iddle y la velocidad de transferencia.

```
- tcptrack -i eth0                                              Mostrar todo el tráfico TCP en una interfaz de red-
- tcptrack -i eth0 -t                                           Mostrar el tráfico TCP con información detallada
- tcptrack -i eth0 port 80                                      Filtrar el tráfico por puerto
- tcptrack -i eth0 host 192.168.1.1                             Filtrar el tráfico por dirección IP
- tcptrack -i eth0 -p                                           Mostrar el tráfico en modo promiscuo
- tcptrack -i eth0 port 80 and src host 192.168.1.1             Mostrar tráfico en un puerto y con IP de origen
- tcptrack -i eth0 portrange 8000-9000 and dst host 10.0.0.2    Mostrar tráfico rango de puertos y con IP de destino
- tcptrack -i eth0 src net 192.168.1.0/24 -t                    Filtrar por un rango de direcciones IP de origen y mostrar información detallada
```

---

## **iptraf:** ##
Intercepta paquetes en la red y muestra información sobre el tráfico.

```
# Iniciar iptraf en el modo de interfaz gráfica
sudo iptraf

# Iniciar iptraf en el modo de monitorización de tráfico IP
sudo iptraf -i <interfaz>  # Reemplaza <interfaz> con el nombre de tu interfaz, por ejemplo, eth0

# Mostrar información detallada sobre tráfico TCP
sudo iptraf -i <interfaz> -t

# Mostrar información detallada sobre tráfico UDP
sudo iptraf -i <interfaz> -u

# Filtrar tráfico por dirección IP
sudo iptraf -i <interfaz> -s <ip>  # Reemplaza <interfaz> con tu interfaz y <ip> con la dirección IP deseada

# Mostrar tráfico en modo promiscuo
sudo iptraf -i any

# Mostrar tráfico TCP en una interfaz de red específica
sudo iptraf -i eth0 -t

# Filtrar tráfico por dirección IP de origen específica
sudo iptraf -i eth0 -L /tmp/iptraf-filter -B -F -s <ip>

# Filtrar tráfico por puerto de destino específico
sudo iptraf -i eth0 -L /tmp/iptraf-filter -B -F -d <puerto>

```

---

## **bandwidthd:** ##
Una herramienta específica de monitorización del ancho de banda, es decir utiliza la información recopilada para generar gráficos y tablas que muestran qué hosts en la red están utilizando más ancho de banda y qué servicios específicos están generando tráfico.

```
- sudo apt-get install bandwidthd       Instalamos bandwidthd
- sudo bandwidthd
- http://localhost/bandwidthd           Estadísticas sobre el uso del ancho de banda.