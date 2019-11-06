# TP3 - LPC43xx Entradas y Salidas (Digitales) de Propósito General (GPIO) – FreeRTOS

Practica n°3 de sistemas embebidos.

## 1. Uso del IDE (Integrated Development Environment) LPCXpresso

### Documentacion de los proyectos importados

#### freertos_examples_1_to_9
Las carpetas de cada proyectos importados tienen la misma estructura.

| Archivo | funcion |
| ----- | ---- |
| Project settings | Parametros del proyecto segun el "project.mk". |
| Binaries |  Un archivo ".axf" que incluye informaciones de debug y de codigo objeto. |
| Includes | Incluye los plug-ins para el funcionamiento de la aplicacion.  |
| Example |  En esta archivo tenemos un archivo "inc" que incluye una libraria RTOS y un archivo "src" que incluye el codigo fuente de la aplicacion (.c), un codigo "sysinit.c" que permite la inicialisacion del sistema segun el core (core-M3 o M4) y la placa, y un codigo que es un código de inicio del microcontrolador para su uso con LPCXpresso IDE. Para terminar tenemos el archivo que define las opciones de configuración de OpenOCD) y el "readme" que nos indicamos el funcionamiento de la aplicacion.|
| FreeRTOS |  Aca tenemos todas la librerias para el funcionamiento de freeRTOS. |
| Debug |  En este archvio estan los codigos objetos (.o), los archivos de debug y de configuracion. |

```
codes examples
```
#### freertos_examples_10_to_16

#### lcp_chip_43xx

#### lcp_board_nxp_lpcxpresso_4337


## 2. A partir del proyecto freertos_examples_1_to_9 => Example 1 - Creating tasks



## 3. A partir del proyecto freertos_examples_10_to_16 => Example 10 - Blocking when receiving from a queue



## 4. Implementacion de aplicación 1



## 5. Implementacion de aplicación 2



## 6. Implementacion de aplicación 3
