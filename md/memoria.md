## **free**:

|COMANDO    | USO |
|-------|----------|
| -b |  Muestra la salida en bytes.  |
| -k |  Muestra la salida en kilobytes (KB). Es el resultado por defecto.  |
| -m |  Muestra la salida en megabytes (MB).  |
| -g |  Muestra la salida en gigabytes (GB). |
| -l |  Muestra información detallada acerca de la utilización baja y alta de memoria.  |
| -o |  Muestra el formato antiguo, sin -/+ buffers/cache.  |
| -t |  Muestra un resumen del total de memoria física y swap. |
| -c n |  Refrescará la información n veces y luego saldrá del programa.  |
| -s n |  Repetición, pausando n segundos entre una y otra  |
| -V |  Muestra la versión de free y sale.  |
| -help |  Muestra la ayuda y sale.   |

---

## **df**:

|COMANDO    | USO |
|-------|----------|
| -h |  Te mostrará el resultado en un formato legible por humanos |
| -m |  Esta línea de comando se utiliza para mostrar la información del uso del sistema de archivos en MB.  |
| -k |  Para mostrar el uso del sistema en KB. |
| -T | Esta opción mostrará el tipo de sistema de archivos (aparecerá una nueva columna).  |
| -ht | Te permite ver información de un sistema de archivos específico en un formato legible (en este caso el sistema de archivos /home).  |
| --help | Listará otros comandos útiles que puedes usar, con sus descripciones.  |

---

## **du**:

|COMANDO    | USO |
|-------|----------|
| du /home/user/Desktop/  | Permite a los usuarios ver el uso del disco de los archivos y las carpetas que están en el directorio Desktop (los subdirectorios se incluyen también).  |
| du -h /home/user/Desktop/ | Al igual que con df, la opción -h la opción -h muestra información en un formato legible por humanos. |
| du -sh /home/user/Desktop/ | La opción -s nos da el tamaño total de una carpeta especifica (en este caso, el directorio Desktop). |
| du -m /home/user/Desktop/ | La opción -m nos proporciona los tamaños de carpetas y archivos en Megabytes (podemos usar -k para ver la información en Kilobytes). |
| du -h –time /home/user/Desktop/ | Esto informa la última fecha de modificación de los archivos y carpetas mostrados. |
| df –help | Muestra una lista de opciones disponibles y para qué se pueden utilizar. |

```
. du -h /home/user/Desktop/ | sort –rn   (Ordenará todos los archivos y carpetas de mayor a menor para comprobar el uso de espacio de disco en Linux)

. du -h /home/user/Desktop | grep '^\s*[0-9\.]\+G'  (Quieres ver todos los archivos que superan un determinado tamaño, devolverá todos los archivos mayores a 1 GB.)

. du -h /home/user/Desktop/ --exclude="*.txt"   (Excluir un formato de archivo concreto de los resultados de la búsqueda)
```

---

## **iostat**:

|COMANDO    | USO |
|-------|----------|
| iostat | obtiene informes y estadísticas |
| iostat -x | muestra información estadística más detallada |
| iostat -c | muestra solo la estadística de la CPU. |
| iostat -d | muestra solo el informe del dispositivo |
| iostat -xd | muestra estadísticas de E/S (operaciones de inicio)ampliadas únicamente para el dispositivo. |


