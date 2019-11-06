# # Documentación Trabajo Práctico N° 3

**Seminario de Electrónica: Sistemas Embebidos**

**LPC43xx Entradas y Salidas (Digitales) de Propósito General (GPIO) – Diagrama de Estado**

Objetivo:  
• Uso del IDE (edición, compilación y depuración de programas)  
• Uso de GPIO & FreeRTOS (manejo de Salidas y de Entradas Digitales en Aplicaciones)  
• Documentar lo que se solicita en c/ítems

## 1. Estructura de archivos

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

### freertos_examples_1_to_9

El archivo (.c) se puede desglosar así:
* Enumeracion de la variables privadas. Estos son #define que permiten eligir la parte del codigo que queremos ejecutar.
* Funcion privada de setup del hardware.
* Condiciones sobre el valor de una variable que tiene un valor correspondiente al ejemplo que queremos ejecutar.
	* EXAMPLE1
	* EXAMPLE2
	* EXAMPLE3
	* EXAMPLE4
	* EXAMPLE5
	* EXAMPLE6
	* EXAMPLE7
	* EXAMPLE8
	* EXAMPLE9
	
El archivo "readme.txt" permite entender el funcionamiento y los parametricos de la aplicacion.
* Descripcion del ejemplo.
* Configuracion del hardware.
* Como hacer un 'build' del proyecto.

### freertos_examples_10_to_16

El contenido de este archivo es igual al del archivo anterior.

### lcp_chip_43xx

Este archivo contiene los codigos (.c y .h) para el uso de los perifericos del sistema. (gpio, adc, i2c, timer, ...)

### lcp_board_nxp_lpcxpresso_4337

El ultimo archivo contiene los control de driver de la placa EDU-CIAA-NXP, como el lcd o los entradas y salidas.

### Secuencia de funciones del ejemplo 1

| funciones | archivo | descripcion | efecto |
| ----- | ---- | ---- | ---- |
| prvSetupHardware() | freertos_examples_1_to_9.c | Parametra el sistema hardware |  |
| DEBUGOUT(pcTextForMain) | board_api.h | funcion de debug, muestra el estado de debug|  |
| xTaskCreate(vTaskCode, "NAME", STACK_SIZE, &ucParameterToPass, tskIDLE_PRIORITY, &xHandle) | task.c/.h | Crea la tarea, memoriza el handle, asigna prioridades. |  |
| vTaskStartScheduler() | tasks.c/.h | Inicia el procesamiento en tiempo real, tiene control sobre qué tareas se ejecutan y cuándo. |  |

## 2. Ejemplos del 1 al 9

### Ejemplo 1



### Ejemplo 2


### Ejemplo 3


### Ejemplo 4


### Ejemplo 5


### Ejemplo 6


### Ejemplo 7


### Ejemplo 8


### Ejemplo 9


## 3. Ejemplos del 10 al 16

### Ejemplo 10


### Ejemplo 11


### Ejemplo 12


### Ejemplo 13


### Ejemplo 14


### Ejemplo 15


### Ejemplo 16


## 4. Implementación de aplicación 1



## 5. Implementación de aplicación 2



## 6. Implementación de aplicación 3
