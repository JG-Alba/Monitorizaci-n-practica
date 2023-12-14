## **ps** :

**ps -aux**
```
La opción **a** muestra todos los procesos en ejecución de todos los usuarios del sistema.

La opción **u** proporciona información adicional como el porcentaje de uso de memoria y CPU, el código de estado del proceso y el propietario de los procesos.

La opción **x** lista todos los procesos que no se ejecutan desde el terminal. Un ejemplo perfecto de esto son los daemons, que son procesos relacionados con el sistema que se ejecutan en segundo plano cuando se inicia el sistema.
```

|COMANDO    | USO |
|-------|----------|
|ps -U nombre_usuario|  lista todos los procesos en ejecución de un determinado usuario.  |
|ps -A |  muestra los procesos Linux activos en el formato genérico UNIX |
|ps -T|  imprime los procesos activos que se ejecutan desde el terminal.  |
|ps -C nombre_proceso|  filtra la lista por el nombre del proceso. Además, este comando también muestra todos los procesos hijos del proceso especificado.  |

---


## **top**:


|COMANDO    | USO |
|-------|----------|
| k | Finaliza un proceso  |
| M | Ordena la lista por uso de memoria.  |
| N | Ordena la lista por PID.  |
| r | Cambia la prioridad de un proceso.  |
| h | Muestra la ventana de ayuda. |
| z | Muestra los procesos en ejecución en colores.  |
| d | Cambia el intervalo de tiempo de actualización.  |
| c | Muestra la ruta absoluta de un proceso.  |
| CTRL+C | Detiene el comando superior.  |
| P  | Ordena la lista por CPU.   |
| f  | Seleccionar lo que quieres, espacio para señalar o quitar, q para salir.   |
| top -b -n [Nº secuencias]>[archivo] |  Para enviar la secuencia o secuencias de procesos a un archivo.  |
| R  | Para ordenarlo de menos a mas.   |

---

## **htop**:

```
sudo apt install htop
```

|COMANDO    | USO |
|-------|----------|
| F9 | Finaliza un proceso. |
| F8 | Aumenta la prioridad de un proceso. |
| F7 | 	Disminuye la prioridad de un proceso. |
| F6 | Ordena procesos por cualquier columna. |
| F5 | Muestra los procesos en una vista de árbol. |
| F4 | Filtra los procesos por nombre. |
| F3 | Busca un proceso. |
| F2 | Abre htop setup. |
| F1 | Muestra el menú de ayuda. |

---


## **atop**:


```
sudo apt install atop
```


|COMANDO    | USO |
|-------|----------|
| man atop | Muestra la página del manual del comando atop. |
| atop -l | Muestra los valores totales medios por segundo. |
| atop -a | Muestra los procesos activos durante los últimos intervalos. |
| atop -c | Muestra la línea de comandos por proceso. |
| atop -m | Muestra la información relacionada con la memoria. |
| atop -d | Muestra la información relacionada con el disco. |
| atop -n | Muestra la información de la red. |
| atop -s | Muestra los detalles de la programación. |
| atop -v | Muestra información diversa (por ejemplo, PPID, usuario u hora). |
| atop -y | Muestra los hilos individuales. |

|CLAVES    | FUNCIONES |
|-------|----------|
| a |  Clasifica por orden los recursos más activos. |
| c |  Vuelve a la ordenación por consumo de CPU (por defecto). |
| d |  Clasifica por orden de actividad del disco. |
| m | Clasifica por orden de uso de memoria.  |
| n | Clasifica por orden de actividad en la red.  |
